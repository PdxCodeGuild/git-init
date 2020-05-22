# Making a New Branch
[Back to Syllabus](/README.md)

After cloning a repo, make a new branch **IMMEDIATELY**. You should never work off of the master version of the code. If you were working on a team, and you introduced a bug to the master branch, the whole application can shut down FOR EVERYONE. Don't be that developer!

To avoid conflicts, you should get into the habit of double checking that

- you have the lastest version of master
- there are no stray uncommited files

1. Double check you're on master.
```
git branch
```

2. Double check you don't have any stray files
```
git status
```

3. Double check you have the latest version of master
```
git pull
```

Once we have confirmed that we are on the correct branch and that we have the latest version of master, now we can safely create a new branch.