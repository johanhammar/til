# Show entire history of a file

Sometimes you want to see the entire history of a file. The command below is what you are looking for.

```
$ git log --follow -p -- <file>
```

Use `--follow` to see history even if the file have been renamed.  

via [http://stackoverflow.com/questions/278192/view-the-change-history-of-a-file-using-git-versioning](http://stackoverflow.com/questions/278192/view-the-change-history-of-a-file-using-git-versioning)
