# Git Stash

Git stash stores changes that you've done on the working copy. This allows you to work on other things, and come back to work later. Stash is useful when you need to toggle the context and work in another thing, but, is in the middle of an code change but it's not ready to make the commit.

```
$ git status
On branch main
Changes to be committed:

    new file:   style.css

Changes not staged for commit:

    modified:   index.html

$ git stash
Saved working directory and index state WIP on main: 5002d47 our new homepage
HEAD is now at 5002d47 our new homepage

$ git status
On branch main
nothing to commit, working tree clean
```

At that point you're free to make changes, create comits, toggle between branches and run other git command. When you're done, comeback and apply your stash.

### Reaply the changes with stash

```
$ git status
On branch main
nothing to commit, working tree clean
$ git stash pop
On branch main
Changes to be committed:

    new file:   style.css

Changes not staged for commit:

    modified:   index.html

Dropped refs/stash@{0} (32b3aa1d185dfe6d57b3c3cc3b32cbf3e380cc6a)
```

Git stash pop delete the changes of stash and reapply into the working copy.
