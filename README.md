# git-treesame-commit

Utility to make new commits that are
[treesame](https://git-scm.com/docs/git-log#_history_simplification)
with others.

Every commit has a _treehash_, or, a specific identifier that represents
the state of the file tree. Two commits that have the exact same file
tree and thus the exact same treehash are called _treesame_.

This tool allows you to create a new commit on your current branch that
is treesame with any arbitrary commit anywhere else. It's basically like
being able to cherry-pick the entire state of a file tree.

This tool has transformed how quickly I am able to figure out and
debug git situations and I can't understand how this isn't built in to
git already.

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

### License

```
MIT License

Copyright (c) 2018 JT Olio

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```
