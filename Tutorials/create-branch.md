# GitHub Branching Tutorial

## Introduction
Working with branches in GitHub is crucial when collaborating in a team. Branches allow multiple people to work on different features without affecting the main codebase. It ensures that the `master` or the `main` branch always has production-quality code.

## Creating a Branch
Here are the steps to create a new branch in GitHub:

1. Go to your project repository on GitHub.
2. Click on the dropdown menu labeled `Branch: master` or `Branch: main`.
3. Type a unique name for your new branch, then press `Enter`. Your new branch is now created and active.

![Create a branch](./assets/create-branch.png)

## Keeping Your Branch Up-to-Date
To ensure your branch is up-to-date with the `master` branch, you need to pull the changes from `master` into your branch. Here's how:

1. Switch to the `master` or `main` branch by clicking on the `Branch` dropdown and selecting `master`.
2. Switch back to your branch using the `Branch` dropdown.
3. Click on `New Pull Request`.
4. In the `base:` dropdown, ensure your branch is selected. In the `compare:` dropdown, select `master`.
6. Review the changes, then click `Create Pull Request`.
7. Add a title and description for your pull request, then click `Create Pull Request`.
8. Click `Merge Pull Request`, then `Confirm Merge`. Your branch is now up-to-date with `master`.

Remember, it's important to regularly update your branch with `master` to avoid merge conflicts. Happy coding!
