# Reset 
Reset a branch in forked repo to be the same as the original repo

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
Similar as Example 1, but if remote upstream is not added, add 1st line.
```
git remote add upstream /url/to/original/repo
git fetch upstream
git checkout main
git reset --hard upstream/main
git push origin main --force 
```

Found this method at: https://stackoverflow.com/questions/9646167/clean-up-a-fork-and-restart-it-from-the-upstream

## Example 3.
Example 3 is the same as Example 1 and 2.

Problem statement: I made 2 changes (change 1 and 2) in my forked repo. The main repo made 3rd chage. Then I fetch upstream to get the udpate from repo.
Then I made the 4th change in my forked repo. Now how to remove all my changes in my forked repo, and make my fork the same as main repo.
Remove change 1 2 and 4.


To remove your changes and make your forked repository identical to the main repository, you can follow these steps:

- Open forked repo in terminal. 
- Go to the correct branch. For example "main"
- Not important: Check the status of your repository to see the modified files and uncommitted changes. Use the command git status if you're using Git from the command line. If there are any uncommitted changes, you can either commit them or discard them, depending on your preference. Use the appropriate command for your Git client or execute git stash if using Git from the command line to save your changes temporarily.
- Reset your branch to the state of the main repository. Run the command ```git reset --hard upstream/main``` 
- After resetting the branch, your local forked repository will match the state of the main repository. However, your remote forked repository still needs to be updated. To do this, force push your local branch to your forked repository using the command ```git push origin <branch-name> --force```

Once the push is complete, your forked repository should now be identical to the main repository, removing the changes you made in steps 1, 2, and 4.
Please note that force pushing will overwrite the remote branch with your local branch, so make sure you don't have any important changes in your fork that you want to keep before performing this operation.

