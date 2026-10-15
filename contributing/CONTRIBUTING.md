# Nexirift Contributing Guide

**THIS IS A DRAFT**

**Last Updated:** 15th of October 2026 at 12:00 PM (ACDT)

Please ensure that you have read and agree to the [Code of Conduct](CODE_OF_CONDUCT.md) in its entirety.

Have a look at the [Projects](PROJECTS.md) page to ensure that you are not committing to a legacy project!

Regularly read over this document as we may update information here.

## Artifical intelligence usage

Follow the [AI usage](AI_USAGE.md) document.

## Pull requests

- Never push straight to the `main` branch, or others without approval.
- Use the format `username/add-fix-etc` to create your branches.
- Do not merge unless you have at least 2+ reviews.
- Delete your branches after merging, this can be done in the PR UI.
- Do not make massive changes (e.g. 10,000 lines) in a single commit.
- Give the pull request an appropriate name and description.
  - It defaults to the first commit which might not be good enough.
- Do not interfere with other people's pull request commits.
- Squash when merging if there are a lot of commits for the same thing.
- Ensure that you are based on `main` and not another pull request.
- Action workflows are required to pass prior to merging.
- Do not mark your pull request as ready unless it is completed.

### How do I do start?

Firstly, if there is an existing issue, assign yourself and/or leave a comment to say that it is being actively worked on. Otherwise, you could create an issue to track your progress.

#### To create a new branch (VS Code):

- Click the `main` in the bottom left.
- Click `Create new branch`, follow above.
- Commit your changes in this branch.

#### To switch back to main (CLI):

- Switch back: `git checkout main`
- Pull changes: `git pull main`

## Issues

We utilise issues to track what needs to be done within the project.

- No assignees means it is free for you to work on.
- Assign yourself if you are actively working on it.
- Utilise the appropriate labels, e.g. `Kind/Feature`.
- When requested, review pull requests and leave comments.
- Mark your pull request as a draft if actively worked on.
- Feel free to edit and/or improve other people's issues.

## Before committing, please...

- Ensure compliance with all information above
- Run the proper check command, usually: `pnpm check`
- Run the proper format command, usually: `pnpm format`
