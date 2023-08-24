# Git Stash
## When to use git stash
Has made changes on the ```main``` branch but haven't committed them yet.

Want to transfer all those changes to a new branch without committing them to the main branch.

## How to use git stash
Follow below steps:

1. Stash your current changes on the main branch using the following command:

   ```
   git stash
   ```

   This command will temporarily save your changes, allowing you to switch to a new branch without committing them.

2. Create a new branch from the main branch. You can choose any name for the new branch. For example:

   ```
   git branch new-branch
   ```

3. Switch to the newly created branch:

   ```
   git checkout new-branch
   ```

4. Apply the changes you stashed earlier from the main branch to the new branch:

   ```
   git stash apply
   ```

   This command reapplies the changes you stashed onto the new branch.

Note: 
Now you have a new branch, "new-branch," that contains all the changes you made on the main branch without committing them. The main branch remains in its previous state. You can continue working on the new branch and make commits as needed.

Remember that if you want to bring the changes from the new branch back to the main branch, you will need to merge or rebase the new branch into the main branch once you are satisfied with the changes.
