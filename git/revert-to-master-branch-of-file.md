# Revert local to origins master branch version of file

How to revert a local updated file to the original version from the remote:

Assuming you did not commit the file, or add it to the index, then:

```
git checkout -- filename
```
Assuming you added it to the index, but did not commit it, then:

```
git reset HEAD filename
git checkout -- filename
```

Assuming you did commit it: then:

```
git checkout origin/master filename
```

Assuming you want to blow away all commits from your branch (VERY DESTRUCTIVE):

```
git reset --hard origin/master
```

[Stackoverflow reference](https://stackoverflow.com/questions/1817766/how-to-revert-to-origins-master-branchs-version-of-file)

