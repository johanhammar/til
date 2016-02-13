# Git diff algorithms

Performing a diff in Git is as easy as 

```
$ git diff <filename>
```

There are four different diffing algorithms (from the man page): 

* default, myers:

    The basic greedy diff algorithm. Currently, this is the default.

* minimal:

    Spend extra time to make sure the smallest possible diff is produced.

* patience

    Use "patience diff" algorithm when generating patches.

* histogram
    
    This algorithm extends the patience algorithm to "support low-occurrence common elements".

Invoke them by either 

```
git diff --{myers|minimal|patience|histogram}
```

or

```
git diff --diff-algorithm={patience|minimal|histogram|myers}
```

or via

```
git config --global diff.algorithm {patience|minimal|histogram|myers}
```

## Read more

* [Patience Diff Advantages](http://bramcohen.livejournal.com/73318.html)
* [Difference between Git diff patience and Git diff Histogram](http://stackoverflow.com/questions/32365271/whats-the-difference-between-git-diff-patience-and-git-diff-histogram)
