# Reset a branch in forked repo to be the same as the original repo

## Example 1. 
I have made  modification in forked main repo. I want to remove all the changes.

In other words, I want my main in forked the same as the main in original repo.

```
git fetch upstream
git checkout main
git reset --hard upstream/main
git push origin main --force
```

## Example 2.
Similar as example 1, but if remote upstream is not added, add 1st line.
```
git remote add upstream /url/to/original/repo
git fetch upstream
git checkout main
git reset --hard upstream/main
git push origin main --force 
```

Found this method at: https://stackoverflow.com/questions/9646167/clean-up-a-fork-and-restart-it-from-the-upstream
