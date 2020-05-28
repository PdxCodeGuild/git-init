# <a id="trouble"></a>Troubleshooting
[Back to Syllabus](/README.md)

## Error: missing upstream branch

Error:
```
fatal: The current branch master has no upstream branch.
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