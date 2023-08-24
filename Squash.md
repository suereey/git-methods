# How to squash multiple commits

For example: I was working in ```main``` branch. I have past 4 commits and want to squash to 1.

```
git checkout main
git reset --soft HEAD~4
git commit -m "update on ---"
git push --force origin main
```

Found this method at: https://stackoverflow.com/questions/5667884/how-to-squash-commits-in-git-after-they-have-been-pushed
