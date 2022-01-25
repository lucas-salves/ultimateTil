# Status porcelain flag

The default git status output its very verbose. So, we can use the -s (--short) flag to tells git that we want to see only the files that we updated. But, the --short flag its useful only to readability, because it returns color formated text. If we want to use the output of the status in a script, we need to use the --porcelain flag.
The --porcelain flag return only the files status, and we don't need to care about lost this in future updates:
```
git status --porcelain
```
The 2.35 relase added the v2 output type to the porcelain flag:
```
git status --porcelain=v2
```

### References
- [The short version of git status and the close but different porcelain mode](https://www.stefanjudis.com/today-i-learned/the-short-version-of-git-status-and-the-close-but-different-porcelain-mode/)
