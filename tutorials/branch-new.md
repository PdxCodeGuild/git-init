# Making a New Branch
[Back to Syllabus](/README.md)

After cloning a repo, make a new branch **IMMEDIATELY**. You should never make changes to the master version a project. If you introduced a bug to the master branch, the whole application can shut down FOR EVERYONE on your team. Don't be that developer!

To avoid conflicts, you should get into the habit of double checking that

- you have the lastest version of master
- there are no stray uncommited files

before creating a new branch. The steps are outlined below:

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

The name of your new branch should be the lab name and your initials. That way it's clear to your teacher.

```
git checkout -b rps-LN
```

The command above will create a new branch AND checkout. You can double check that you're in the new branch by running the command:

```
git branch
```