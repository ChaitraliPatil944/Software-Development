# Lesson 150 --- Branch

# Part 10 --- Version Control Systems

> **Objective**
>
> Understand Git branches, why branching is required, branch
> architecture, creating and managing branches, branch strategies,
> naming conventions, and how software teams use branches in
> professional development.

------------------------------------------------------------------------

# Introduction

Software development often requires multiple features and fixes to be
developed at the same time.

Developers need a way to work independently without affecting the stable
application.

Git Branches solve this problem.

``` text
Main Code

    |

    +---- Feature A

    |

    +---- Feature B

    |

    +---- Bug Fix
```

------------------------------------------------------------------------

# What is a Git Branch?

A **Git Branch** is a separate line of development that allows
developers to work on changes independently.

A branch is simply a pointer to a commit.

Example:

    main

     ↓

    Commit C3

Create branch:

    feature-login

     ↓

    Commit C3

------------------------------------------------------------------------

# Why Do We Need Branches?

Without branches:

``` text
Multiple Developers

        ↓

Same Codebase

        ↓

Conflicts

        ↓

Unstable Application
```

Branches help:

-   Develop features separately
-   Fix bugs safely
-   Experiment without affecting main code
-   Support parallel development

------------------------------------------------------------------------

# Branch Architecture

Git branches are lightweight references.

Example:

                  Feature Branch

                        |

                        ↓

    C1 ---- C2 ---- C3 ---- C4

                        ↑

                      main

Both branches can share the same history.

------------------------------------------------------------------------

# Main Branch

The main branch contains stable production-ready code.

Common names:

-   main
-   master

Example:

    main

     ↓

    Production Code

------------------------------------------------------------------------

# Feature Branch

Used for developing new features.

Example:

    main

     |

    feature-payment

After completion, it is merged into main.

------------------------------------------------------------------------

# Bug Fix Branch

Used for fixing problems.

Example:

    main

     |

    bugfix-login-error

------------------------------------------------------------------------

# Creating a Branch

Command:

``` bash
git branch branch_name
```

Example:

``` bash
git branch feature-login
```

Creates a new branch.

------------------------------------------------------------------------

# Viewing Branches

Command:

``` bash
git branch
```

Example output:

    * main

      feature-login

      bugfix-payment

The `*` indicates the current branch.

------------------------------------------------------------------------

# Switching Branches

Command:

``` bash
git checkout branch_name
```

Example:

``` bash
git checkout feature-login
```

Modern command:

``` bash
git switch feature-login
```

------------------------------------------------------------------------

# Creating and Switching Together

Command:

``` bash
git checkout -b branch_name
```

Example:

``` bash
git checkout -b feature-dashboard
```

Creates and switches to the new branch.

------------------------------------------------------------------------

# Branch Workflow

Typical workflow:

``` text
Create Branch

      ↓

Develop Feature

      ↓

Commit Changes

      ↓

Push Branch

      ↓

Code Review

      ↓

Merge
```

------------------------------------------------------------------------

# Branch Naming Convention

Good branch names are descriptive.

Examples:

    feature-user-login

    feature-payment-api

    bugfix-cart-error

    hotfix-security-issue

Avoid:

    test

    new

    branch1

------------------------------------------------------------------------

# Feature Branch Workflow

Example:

Task:

    Add User Authentication

Steps:

``` text
Create Branch

feature-auth

        ↓

Write Code

        ↓

Commit Changes

        ↓

Review

        ↓

Merge to main
```

------------------------------------------------------------------------

# Branch Strategies

Organizations use different branching models.

------------------------------------------------------------------------

# 1. Feature Branching

Each feature gets its own branch.

Example:

    main

     |

    feature-login

     |

    feature-payment

Advantages:

-   Safe development
-   Easy review

------------------------------------------------------------------------

# 2. Git Flow

A structured branching model.

Branches:

    main

    develop

    feature

    release

    hotfix

Used in larger projects.

------------------------------------------------------------------------

# 3. Trunk-Based Development

Developers frequently merge into main.

Advantages:

-   Faster delivery
-   Supports CI/CD

------------------------------------------------------------------------

# Branch Merging

After completing work, branches are combined.

Example:

    feature-login

          ↓

    Merge

          ↓

    main

Command:

``` bash
git merge branch_name
```

------------------------------------------------------------------------

# Branch Deletion

After merging, unnecessary branches can be removed.

Command:

``` bash
git branch -d branch_name
```

Example:

``` bash
git branch -d feature-login
```

------------------------------------------------------------------------

# Remote Branches

Branches can exist on remote repositories.

Example:

    Local Branch

            ↓

    Remote Branch

Commands:

Push branch:

``` bash
git push origin branch_name
```

Fetch branches:

``` bash
git fetch
```

------------------------------------------------------------------------

# Branch in Industry

Example:

Software Team:

    main

     |

    develop

     |

    feature-payment

     |

    feature-login

Developers work independently and merge completed features after review.

------------------------------------------------------------------------

# Branch Best Practices

-   Create branches for features
-   Keep branches small
-   Use meaningful names
-   Merge frequently
-   Delete old branches
-   Avoid direct changes to main

------------------------------------------------------------------------

# Common Branch Problems

## Problem 1

Long-running branches.

Solution:

Merge frequently.

------------------------------------------------------------------------

## Problem 2

Too many branches.

Solution:

Remove unused branches.

------------------------------------------------------------------------

## Problem 3

Conflicts during merge.

Solution:

Sync branches regularly.

------------------------------------------------------------------------

# Interview Questions

1.  What is a Git branch?
2.  Why are branches used?
3.  How are branches stored internally?
4.  Difference between main branch and feature branch?
5.  How do you create a branch?
6.  How do you switch branches?
7.  Explain Git Flow.
8.  What is trunk-based development?
9.  How do you delete a branch?

------------------------------------------------------------------------

# Cheat Sheet

``` text
Git Branch

Create Branch

      ↓

Work Independently

      ↓

Commit Changes

      ↓

Review

      ↓

Merge

      ↓

Delete Branch
```

------------------------------------------------------------------------

# Summary

Git branches allow developers to work on multiple features, fixes, and
experiments independently without affecting stable code. Branching is a
fundamental Git concept used by professional software teams to support
collaboration, code review, and safe software delivery.
