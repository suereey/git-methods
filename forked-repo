## Work flow on GitHub PR

Normally: Creating a new branch is the recommended approach for collaborating on a project and submitting your changes for review. It helps maintain a clean and organized history, and also allows multiple developers to work on different features simultaneously without conflicts.

However, if you want to create a pull request without creating a new branch, you can follow this approach:

1. Fork the repository on GitHub by clicking the "Fork" button in the top-right corner of the original repository's page.

2. Clone your forked repository to your local machine:

``` 
git clone https://github.com/your-username/repository-name.git
```

3. Add the original repository as a remote to keep your fork updated:

``` 
git remote add upstream https://github.com/original-owner/repository-name.git
```

4. Switch to branch A:

``` 
git checkout branchA # Switch to branch A
```

5. Make your changes to the code and then stage and commit them:

``` 
git add . # Stage all changes for commit
git commit -m "Your commit message" # Commit the changes with a message
```

6. Push your changes to your forked repository:

``` 
git push origin branchA # Push your changes to your fork
```

7. Now, navigate to the GitHub repository page of your fork in your web browser.
8. Click on the "Pull requests" tab.
9. Click on the "New pull request" button.
10. You will be redirected to the original repository's page. Select `branchA` as the base branch (in the original repository) and `branchA` as the compare branch (in your forked repository).
11. Review your changes and, if everything looks good, click on "Create pull request."
12. Add a title and description for your pull request, then click "Create pull request" again.

Your pull request has now been initiated, and your peers will be notified. They can review your changes and provide feedback. Once they have reviewed and approved the changes, they can merge the changes from your fork's `branchA` into the original repository's `branchA`.

Keep in mind that this approach is not ideal for collaboration, as it requires you to maintain a fork of the repository, and it can be more challenging to keep your fork up-to-date with the original repository. Using feature branches is the recommended way to work on projects collaboratively.

