# Source Control

## We love GitHub

We will be heavily relying on Git for version control, using GitHub to host our repositories and GitHub Actions for any automation we might need.

# Guides and Tutorials

- Here are some helpful guides for using GitHub:
  - [Getting Started](https://docs.github.com/en/get-started/quickstart)
  - [Git, GitHub, & GitHub Desktop for Beginners](https://www.youtube.com/watch?v=8Dd7KRpKeaE&t=60s)

# Basic Git workflow

## Useful Commands

Some of the most common commands you will use are:

- `git clone <github remote url>` - This command will copy the repo to your local machine in the current working directory you are in.
- `git pull` - This command pulls any changes from remote repo to your local. PULL OFTEN! Will save you from merge conflicts or the dreaded `git rebase`!
- `git add <filename>` - This will stage the file to be commited to the branch.
- `git commit -m "<insert commit message"` - This command is used commit your changes to your local branch
- `git push origin <branch name>` - This command is used to push your local copy of the branch to GitHub repo copy of your branch

## Branching and Commits

We will following feature branche approach. We will have a main branch per repo that will be the "live" working version. When adding a new feature or fix, we will create a branch. Branching is like taking a copy of main, and being able add and test a new feature without changing the main branch.

Example: To create a feature branch we can use `git checkout -b "branch-name`. MAKE SURE you are ON the main branch when creating your feature branch.

Main will be protected, meaning no push will go through until a PR has been reviewed. Current industry best practice is to have two reviewers, for the sake and scope of this project, for most things we will only use one reviewer needed before a push.

### Commit Messages

Something that is not talked about enough are Commit Message conventions. There is a widely accepted standard that can found [here](https://www.conventionalcommits.org/en/v1.0.0/) thats gives a basic overview. It might seem small or pointless but it REALLY helps when quickly glancing over commit history or when a rollback is needed.

Examples:

- `git commit -m "fix: fixed this bug"`
- `git commit -m "chore: updated the design.md for doc site `
- `git commit -m "feat: adding this fully built feature"`

### MORE COMING SOON
