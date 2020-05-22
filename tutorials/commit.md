# Making a Commit
[Back to Syllabus](/README.md)

## when, where, why
As you make changes to your file(s), you will need to make commits to save your progress. Let's look at the pseudo code for the [Rock, Paper, Scissors](labs/lab01.md) lab:

```python
'''
Lab: Rock, Paper, Scissors

1. Ask the user for their choice (rock, paper, scissors)
  - input()
  - save to variable because we will use the user's input later
2. computer will randomly choose rock, paper or scissors
  - random.choice
  - list of options: rock, paper or scissors
3. Determine who won and tell the user
  - conditional statement

  List of all the cases:
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

Here are all the commits you can make:

- successfully prompt user for an input and save to variable
- successfully included random module & used random.choice() to selected from a list of options
- catch ties

The last part of the lab is hefty so I would break it up:

Option 1:
- successfully determine outcomes against rock
- successfully determine outcomes against paper
- successfully determine outcomes against scissors

Option 2:
- succefully determine computer wins
- sucessfully determins player wins

In total, we're looking at at least **6 commits** for this itty bitty lab!

## How

1. In VS Code, navigate to the **solutions** folder and create a new file titled **rps-yourintials.py**.

2. Copy the pseudo-code above and paste it into your new file.

3. **GIT COMMIT!** using the workflow below:

Action: Check for all unstaged files.

Result: Unstage files will be in **red**.
```
git status
```

Action: Add files to stage. This tells Git which files you want to include in the commit.

Result: Staged files will be in green.

```
git add <filename>
```
```
git status
```

Action: Commit files.

Result: Changes are saved and commited files are no longer listed.

```
git commit -m "Pseudo-code for rps."
```
```
git status
```
