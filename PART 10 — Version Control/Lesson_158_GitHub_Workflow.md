# Lesson 158 --- GitHub Workflow

# Part 10 --- Version Control Systems

> **Objective**
>
> Understand the GitHub development workflow, repository setup,
> collaboration process, fork and clone workflow, branch-based
> development, pull requests, code reviews, issue tracking, CI/CD
> integration, and professional GitHub practices.

------------------------------------------------------------------------

# Introduction

GitHub is a platform built around Git that enables developers to
collaborate, manage projects, review code, and automate software
delivery.

A typical professional workflow:

``` text
Developer

      ↓

GitHub Repository

      ↓

Branch Development

      ↓

Pull Request

      ↓

Code Review

      ↓

Merge

      ↓

Release
```

------------------------------------------------------------------------

# What is GitHub?

GitHub is a cloud-based platform for hosting Git repositories and
collaborating on software projects.

It provides:

-   Repository hosting
-   Collaboration tools
-   Code review
-   Issue tracking
-   Automation
-   CI/CD integration

------------------------------------------------------------------------

# GitHub vs Git

  Git                      GitHub
  ------------------------ -------------------------------------
  Version control system   Hosting platform
  Works locally            Cloud-based service
  Tracks code changes      Enables collaboration
  Command-line tool        Web interface + collaboration tools

------------------------------------------------------------------------

# GitHub Workflow Overview

A common workflow:

``` text
Create Repository

        ↓

Clone Repository

        ↓

Create Branch

        ↓

Write Code

        ↓

Commit Changes

        ↓

Push Branch

        ↓

Create Pull Request

        ↓

Review

        ↓

Merge
```

------------------------------------------------------------------------

# Step 1 --- Create Repository

A repository stores:

-   Source code
-   History
-   Documentation
-   Issues
-   Configuration files

Example:

    Project Repository

    ├── src/

    ├── README.md

    ├── .gitignore

    └── package.json

------------------------------------------------------------------------

# Step 2 --- Clone Repository

Clone creates a local copy.

Command:

``` bash
git clone repository_url
```

Example:

``` bash
git clone https://github.com/user/project.git
```

After cloning:

    GitHub Repository

            ↓

    Local Repository

------------------------------------------------------------------------

# Step 3 --- Create Branch

Developers avoid directly modifying the main branch.

Create feature branch:

``` bash
git checkout -b feature-login
```

Example:

    main

     |

    feature-login

------------------------------------------------------------------------

# Step 4 --- Develop Feature

Developer:

-   Writes code
-   Tests changes
-   Reviews modifications

Check status:

``` bash
git status
```

------------------------------------------------------------------------

# Step 5 --- Commit Changes

Stage files:

``` bash
git add .
```

Create commit:

``` bash
git commit -m "Add login functionality"
```

------------------------------------------------------------------------

# Step 6 --- Push Branch

Upload branch to GitHub:

``` bash
git push origin feature-login
```

Now team members can access the changes.

------------------------------------------------------------------------

# Step 7 --- Pull Request

A Pull Request (PR) requests merging changes into another branch.

Example:

    feature-login

            ↓

    Pull Request

            ↓

    main

A PR includes:

-   Code changes
-   Description
-   Review discussion
-   Tests

------------------------------------------------------------------------

# Pull Request Workflow

``` text
Developer Creates PR

        ↓

Automated Checks Run

        ↓

Code Review

        ↓

Changes Requested

        ↓

Approval

        ↓

Merge
```

------------------------------------------------------------------------

# Fork Workflow

Forking creates a personal copy of another repository.

Common in open-source projects.

Workflow:

``` text
Original Repository

        ↓

Fork

        ↓

Personal Repository

        ↓

Clone

        ↓

Modify

        ↓

Pull Request
```

------------------------------------------------------------------------

# Clone vs Fork

  Clone                      Fork
  -------------------------- -------------------------------
  Local copy                 Remote copy
  Used by team members       Used by external contributors
  Creates local repository   Creates GitHub repository

------------------------------------------------------------------------

# GitHub Issues

Issues are used to track:

-   Bugs
-   Feature requests
-   Tasks
-   Improvements

Example:

    Issue #25

    Fix login validation error

------------------------------------------------------------------------

# Labels and Milestones

## Labels

Categorize issues.

Examples:

    bug

    enhancement

    documentation

------------------------------------------------------------------------

## Milestones

Group issues for releases.

Example:

    Version 2.0 Release

     ├── Issue 1

     ├── Issue 2

     └── Issue 3

------------------------------------------------------------------------

# GitHub Actions and CI/CD

GitHub supports automation using GitHub Actions.

Used for:

-   Testing
-   Building
-   Deployment

Workflow:

``` text
Push Code

      ↓

Run Tests

      ↓

Build Application

      ↓

Deploy
```

------------------------------------------------------------------------

# Branch Protection

Important branches should be protected.

Protection rules:

-   Require pull requests
-   Require reviews
-   Run automated checks
-   Prevent direct pushes

------------------------------------------------------------------------

# Professional GitHub Workflow

Example:

    main

     |

    develop

     |

    feature-payment

     |

    Pull Request

     |

    Code Review

     |

    Merge

     |

    Release

------------------------------------------------------------------------

# GitHub Best Practices

## Repository Management

-   Maintain clear README
-   Use meaningful names
-   Keep repository organized

## Commit Practices

-   Write clear messages
-   Make small commits
-   Avoid unnecessary files

## Collaboration

-   Use pull requests
-   Review code carefully
-   Communicate changes

------------------------------------------------------------------------

# Common GitHub Mistakes

## Mistake 1

Directly pushing to main.

Solution:

Use branches and pull requests.

------------------------------------------------------------------------

## Mistake 2

Committing secrets.

Solution:

Use environment variables.

------------------------------------------------------------------------

## Mistake 3

Poor repository documentation.

Solution:

Maintain README and documentation.

------------------------------------------------------------------------

# Industry Example

Software team building an e-commerce application:

    Developer

     ↓

    feature-cart branch

     ↓

    Commit

     ↓

    Push to GitHub

     ↓

    Pull Request

     ↓

    Code Review

     ↓

    Merge to main

     ↓

    Deployment

------------------------------------------------------------------------

# Interview Questions

1.  What is GitHub?
2.  Difference between Git and GitHub?
3.  Explain GitHub workflow.
4.  What is a pull request?
5.  Difference between clone and fork?
6.  What are GitHub issues?
7.  What is GitHub Actions?
8.  Why are branch protections used?

------------------------------------------------------------------------

# Cheat Sheet

``` text
GitHub Workflow

Clone

 ↓

Branch

 ↓

Code

 ↓

Commit

 ↓

Push

 ↓

Pull Request

 ↓

Review

 ↓

Merge
```

------------------------------------------------------------------------

# Summary

GitHub workflow provides a structured approach for collaborative
software development. Through repositories, branches, commits, pull
requests, reviews, and automation, teams can build reliable software
while maintaining code quality and development history.
