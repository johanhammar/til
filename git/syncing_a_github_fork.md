# Syncing a GitHub fork

After a while a GitHub fork will get outdated. Here's how to keep it up-to-date

Add the upstream remote to your fork
```
$ git remote add upstream https://github.com/ORIGINAL_OWNER/ORIGINAL_REPOSITORY.git
```
Verify upstream have been added
```
$ git remote -v
```

Fetch upstream
```
$ git fetch upstream
```

Check out your forks master branch
```
$ git checkout master
```

Merge upstream with master
```
$ git merge upstream/master
```

Push updated fork to GitHub
```
$ git push origin master
```

from https://help.github.com/articles/syncing-a-fork/
