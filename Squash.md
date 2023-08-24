# How to squash multiple commits

For example: I was working in ```main``` branch. I have past 4 commits and want to squash to 1.

```
git checkout main
git reset --soft HEAD~4
git commit -m "update on ---"
git push --force origin main
```
