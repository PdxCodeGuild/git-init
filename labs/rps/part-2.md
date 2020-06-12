# Code Along #1 - Rock Paper Scissors

## Part 2: Coding Solution

- [Back to Syllabus](/README.md)
- [Back to Part 1](part-1.md)

## User Input

Let's get to coding. If you take a look at our pseudo code, the first step is to ask the user to choose between rock paper or scissors. We made a note to ourselves to use ```input()``` let's do that.

![](/resources/rps/code-1.png)

In your file, **rps.py**, write the following under your pseudo code:

```python
# prompt the user to type an input & save the input to a variable
user_choice = input("Rock, paper, or scissors?")
# print variable to make sure the user input is saved correctly
print(user_choice)
```
Now switch to your terminal and run:
```bash
python3 rps.py
```
The terminal will run your code and print the question you wrote inside the input function! It will be stuck here until you **type** in an input:

![](/resources/rps/code-2.png)

I'm going to type **rock**. After I hit enter, my answer will be printed to the screen.

![](/resources/rps/code-3.png)

So far so good! You know what that means!

![](/resources/git-commit.png)

You know the drill:

```bash
git status
git add rps.py
git commit -m "capture user input"
```

Next, let's capture the computer's random choice:
- remove the extra comments
- import the random module so we can use random.choice()
- define a list of choices for the computer to choose from
- update the print statement to check both variables

```python
# Modules
import random

# Variables
choices = ["rock", "paper", "scissors"]

# Capture User Input
user_choice = input("Rock, paper, or scissors?")

# save computer's random choice
comp_choice = random.choice(choices)

# print variables to confirm save
print(f"User: {user_choice}. Comp: {comp_choice}")
```

Switch to the terminal and run the file:

```bash
python3 rps.py
```

![](/resources/rps/code-4.png)

We're good!

![](/resources/git-commit.png)

You know the drill:

```bash
git status
git add rps.py
git commit -m "capture comp input"
```

## Capturing Ties

Now let's write the logic to determine the winner and print the outcome. Under the print statement, let's capture ties first:

```python
if user_choice == comp_choice:
    print("It's a tie!")
```
I ran the file a few times hoping to catch at least one tie. I got three in a row!

In your terminal:
```bash
python3 rps.py
```

![](/resources/rps/code-5.png)

![](/resources/git-commit.png)
You know what to do:
```bash
git status
git add rps.py
git commit -m "catch all ties"
```

## Checking Rock outcomes 

```python
if user_choice == comp_choice:
    print("It's a tie!")
elif user_choice == "rock":
    if comp_choice == "paper":
        print("User wins!")
    else:
        print("Player wins!")
```

Check that your code works then commit.

```bash
python3 rps.py
git status
git add rps.py
git commit -m "logic for rock outcomes"
```
Outcome:

![](/resources/rps/code-6.png)

## Checking Paper Outcomes

Now let's write what happens when the user choose paper:

```python
# code for catching ties
# code for checking when user is "rock"
elif user_choice == "paper":
    if comp_choice == "rock":
        print("User wins!")
    else:
        print("Player wins!")
```

Check that your code works then commit.

```bash
python3 rps.py
git status
git add rps.py
git commit -m "logic for paper outcomes"
```
Outcome:

![](/resources/rps/code-7.png)


[Back to Part 1](part-1.md)

## Checking Scissors Outcomes

Now let's write what happens when the user choose Scissors:

```python
# code for catching ties
# code for checking when user is "rock"
# code for checking when user is "paper"
elif user_choice == "scissors":
    if comp_choice == "paper":
        print("User wins!")
    else:
        print("Player wins!")
```

Check that your code works then commit.

```bash
python3 rps.py
git status
git add rps.py
git commit -m "logic for scissors outcomes"
```
Outcome:

![](/resources/rps/code-8.png)


[Back to Part 1](part-1.md)
