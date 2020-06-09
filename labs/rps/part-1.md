# Code Along #1 - Rock Paper Scissors
## Part 1 - Set up & Pseudo

[Back to Syllabus](/README.md)

## Objective
We are going to solve the infamous Rock, paper, scissors lab from [Programming 101](https://github.com/PdxCodeGuild/Programming101). Follow along as we make **quality** commits whilst solving this lab.

This lab covers how to use git locally on your machine (without Github). The next few labs will cover how to use git locally while interacting with Github.

## Pre-requsites
- exposure to using the command line. For a crash course, please click [here](https://learnrubythehardway.org/book/appendixa.html).

## Lab Challenge
Let's play rock-paper-scissors with the computer.

1. The computer will ask the user for their choice (rock, paper, scissors)
2. The computer will randomly choose rock, paper or scissors
3. Determine who won and tell the user

Let's list all the cases:
- rock vs rock (tie)
- rock vs paper
- rock vs scissors
- paper vs rock
- paper vs paper
- paper vs scissors
- scissors vs rock
- scissors vs paper
- scissors vs scissors

## Directions

### Step 1: set up file & groom instructions

1. Open your terminal, navigate to the folder that you keep all your projects in. For me, it's in:

```bash
/Users/lisaofalltrades/Desktop/projects
```

So my terminal commands were:

```bash
# first command
cd Desktop

# second command
cd projects
```

2. Make a new folder & cd into into:

```bash
# first command
mkdir rps
# second command
cd rps
```

Screenshot of steps 1 & 2:
![Alt Text](/resources/rps/1.png)

3. initialize git in this folder by running the command: 

```bash
git init
```

The success message will read:
![Alt Text](/resources/rps/3.png)

4. Create a python file & verify that it was created:

```bash
# first command
touch rps.py
# second command
ls
```

5. open the **rps** folder in VS Code from the command line:

```bash
code .
```
![Alt Text](/resources/rps/5a.png)

```code . ``` will launch VS Code for you and add the folder you're in.

> **If you don't have this command**, open VS Code how you usually do. Type **COMMAND + SHIFT + P** This will bring up the search bar. Type in **shell** and select **Shell Command: Install 'code' command in PATH**

![Alt Text](/resources/rps/5b.png)

6. Setting up our file & pseudocode
- Now in VS Code, let's close the **Welcome** tab and open **rps.py**
- We will now copy the assignment instructions into the **rps.py** and convert the instructions into pseudo code (a watered down version for ourselves).
- your **rps.py** should look like this:

```python
# rps. py

'''
Let's play rock-paper-scissors with the computer.

1. The computer will ask the user for their choice (rock, paper, scissors)
2. The computer will randomly choose rock, paper or scissors
3. Determine who won and tell the user

Let's list all the cases:
- rock vs rock (tie)
- rock vs paper
- rock vs scissors
- paper vs rock
- paper vs paper
- paper vs scissors
- scissors vs rock
- scissors vs paper
- scissors vs scissors
'''
```

Whenever I start a new assignment, I like to groom the instructions and pull out all the actionables. Great practice for interviews and working with clients! Edit your **rps.py** to this:

```python
# rps. py

'''
Goal: rock-paper-scissors with the computer
Input: user types rock, paper, or scissors
    - input()
Output: tell the user if they won or lost
    - print()

Pseudo
- ask the user for rock, paper, scissors
- user will type in answer
- save user input as a variable to compare later
- computer will randomly choose rock, paper or scissors
    - random.choice()
    - make a list of options for computer to choose from
- Determine who won and tell the user
    - use elif statement

Possible outcomes:
- rock vs rock (tie)
- rock vs paper
- rock vs scissors
- paper vs rock
- paper vs paper
- paper vs scissors
- scissors vs rock
- scissors vs paper
- scissors vs scissors
'''
```

We can break this down even further by taking a closer look at the possible outcomes. At first glance, one may think that there are 9 outcomes. I only see 3. What are they?

1. User wins
2. Computer wins
3. User and Computer Tie

So I will edit the possible outcomes to look like this:

> **Note**: User vs Computer
```python
'''
Possible outcomes

User wins:
- rock vs scissors
- paper vs rock
- scissors vs paper

Computer wins:
- rock vs paper
- paper vs scissors
- scissors vs rock

Ties:
- rock vs rock (tie)
- paper vs paper
- scissors vs scissors
'''
```

WOW! All that work and we haven't even started coding yet. Pseudo code is a great way to design the program. Our thoughts are clearly outlined and now we're set to start.

But before we do that, we're going to GIT COMMIT!

![](https://media.giphy.com/media/gKICHVGdMT2hKbKnES/giphy.gif)

Make sure your file is saved and switch back to the terminal.

[Next: Part 2](part-2.md)