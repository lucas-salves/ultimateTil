# Delete unpushed commits

Delete the most recent commit, keeping the work you've done:

```
git reset --soft HEAD~1
```

Delete the most recent commit, destroyng the work you've done:

```
git reset --hard HEAD~1
```

This command will sync the local repository with the remote repository getting rid of every change you have made on your local. You can also do the following to fetch the exact branch that you have in the origin:

```
git reset --hard origin
```

```
git reset --hard origin/<branch>
```

[Stackoverflow Reference](https://stackoverflow.com/questions/3197413/how-do-i-delete-unpushed-git-commits)
