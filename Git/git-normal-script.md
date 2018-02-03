# Use defaul script From .git

```bash
$ git init
$ git add
$ git commit -m ''
$ git push origin master

$ git clone [url]
$ git remote add origin https://{}:{}@github.com/biezuofei/Daily-learning-records.git
```
```bash
$ git checkout -
```

This is shorthand for `git checkout @{-1}` which is a way of referring to
the previous (or last) branch you were on. You can use this trick to easily
bounce back and forth between `master` and a feature branch.

See `man git` for more details.
