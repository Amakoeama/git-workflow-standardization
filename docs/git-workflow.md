# Git Workflow and Contribution Guidelines

**Repository:** https://github.com/Amakoeama/git-workflow-standardization

## 1. Workflow Model

This repository uses the Feature Branch Workflow to support reliable integration and Continuous Integration (CI).
The main branch represents the stable version of the project. All development work must be completed on separate branches created from main. Changes are integrated into main through pull requests after required checks, review, and approval are completed.

## 2. Branch Naming Conventions

All branches must be created from main and use a descriptive prefix followed by a short lowercase name.

* `feature/` for new features or project enhancements
* `bugfix/` for correcting defects
* `docs/` for documentation changes
* `chore/` for maintenance, configuration, or dependency updates

## 3. Commit Message Standards

This repository follows the Conventional Commits standard to keep commit history clear, consistent, and easy to understand.

Commit messages must use the following format: `<type>(<scope>): <short summary>`

* `feat` for a new feature


* `fix` for a bug fix


* `docs` for documentation changes


* `chore` for maintenance, configuration, or dependency updates


### Examples

* `feat(auth): add user login`

* `docs(workflow): add branch naming conventions`

* `fix(validation): correct input validation error`


## 4. Code Review and Merge Approval Process

Changes must not be merged directly into the main branch. All changes must go through a pull request and review process before merging.


1. **Create a Pull Request:** Open a pull request from the working branch into `main` after the changes are complete.

2. **Pass Automated Checks:** Any configured CI checks, tests, or validation processes must complete successfully before the pull request can be merged.

3. **Complete Code Review:** At least one reviewer must review the changes and provide approval before the pull request is merged.

4. **Receive Approval:** The reviewer must explicitly approve the pull request before merging is allowed.

5. **Merge the Pull Request:** After all required checks and approvals are complete, the pull request may be merged into `main`.

6. **Delete the Branch:** After the pull request is successfully merged, delete the remote working branch to keep the repository organized.


## 5. Branch Protection Rules

The main branch must be protected to prevent direct changes and ensure that all contributions follow the required pull request and review process.

The following protection rules are required: 

* Require a pull request before merging into `main`.

* Require at least one approving review before merging.

* Restrict direct changes to `main` so updates are integrated through pull requests.

* Require configured CI status checks to pass before merging when automated checks are available.


