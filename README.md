# git-treesame-commit
Utility to make new commits that are "treesame" with others

```
usage: git-treesame-commit [-h] [-a] [-p] [-m MESSAGE] commit

Make treesame commits

positional arguments:
  commit                the commit to match

optional arguments:
  -h, --help            show this help message and exit
  -a, --keep-author     if set, keep the commit's original author
  -p, --both-parents    if set, commit will have both parents listed
  -m MESSAGE, --message MESSAGE
                        the new commit message
```
