# Pushing to Github

<a id="top"></a>Helpful Links
- [Back to Syllabus](/README.md)
- [Push to Github](#push)
- [Pull Request](#pull)
- [Pull from Master](#master)
- [Troubleshooting](#trouble)

Now that you've completed your work and all your files are commited, let's push your branch up to Github.

## <a id="push"></a>Push to Github

1. Double check that you don't have any stray files.

```
git status
```

2. Double check that you are on the correct branch
```
git branch
```

3. Push up to Github!
```
git push origin <branch-name>
```
[Back to top](#top)

## <a id="pull"></a>Pull Request on Github

**Fun Fact**: Git's push success message is very helpful because it provides a Github link for you to create a pull request!

1. Copy link and paste it into your browser.

2. Edit pull request title.

Make sure it's a clear summary. If you have any other notes, you can add it to the body. If you have any questions or comments for your teacher, you can tag them here.

3. Save

Save the pull request and for now you're done! From here, your teacher or team lead will review your code. If it is satisfactory, they will merge it to Master.

[Back to top](#top)

## <a id="master"></a>Pull from Master

Once a pull request is approved and branches are merged into Master, your teacher or team lead will alert you to pull from master. When that happens, follow the steps below to keep your master up to date.

1. In your terminal, make sure you're on your master branch.

```bash
git branch
```

2. Make sure you don't have any stray files.

```bash
git status
```

3. Pull the latest changes from master.

```bash
git pull
```
[Back to top](#top)

## <a id="trouble"></a>Troubleshooting

1. missing upstream branch

Error:
```
fatal: The current branch solaris has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin master
```

Solution:

The below command
- links the default remote branch tp the current local branch
- moving forward, you can just run **git pull** instead of **git pull origin master**

```bash
# must be on master branch to run
git branch --set-upstream master
# later verions of Git use
git branch --set-upstream-to
```

[Back to top](#top)
