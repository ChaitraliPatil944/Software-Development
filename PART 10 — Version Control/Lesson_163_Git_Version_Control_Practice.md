# Lesson 163 --- Git & Version Control Practice

# Part 10 --- Version Control Systems

> **Objective**
>
> Practice Git concepts through hands-on exercises including repository
> creation, commits, branches, merging, conflict resolution, rebase,
> stash, tags, remote repositories, GitHub workflow, and real-world
> development scenarios.

------------------------------------------------------------------------

# Introduction

Git skills improve through practice.

Knowing commands is not enough. Developers must understand when and why
to use each operation.

``` text
Learn Concept

      ↓

Practice Command

      ↓

Solve Scenario

      ↓

Build Skill
```

------------------------------------------------------------------------

# Practice 1 --- Create Git Repository

## Task

Create a new project repository.

Project:

    Student Management System

------------------------------------------------------------------------

## Steps

Create folder:

``` bash
mkdir student-system
```

Enter folder:

``` bash
cd student-system
```

Initialize Git:

``` bash
git init
```

Check status:

``` bash
git status
```

------------------------------------------------------------------------

# Practice 2 --- Add and Commit Files

Create files:

    app.py

    README.md

Check status:

``` bash
git status
```

Add files:

``` bash
git add .
```

Create commit:

``` bash
git commit -m "Initial project setup"
```

------------------------------------------------------------------------

# Practice 3 --- View Commit History

Command:

``` bash
git log
```

Tasks:

-   Find commit ID
-   Check author
-   Check message

------------------------------------------------------------------------

# Practice 4 --- Create Branch

Scenario:

Add login functionality.

Create branch:

``` bash
git checkout -b feature-login
```

Verify:

``` bash
git branch
```

------------------------------------------------------------------------

# Practice 5 --- Feature Development Workflow

Task:

Implement login feature.

Workflow:

``` text
Create Branch

      ↓

Modify Code

      ↓

git add

      ↓

git commit

      ↓

Push Branch
```

------------------------------------------------------------------------

# Practice 6 --- Merge Branch

Scenario:

Feature completed.

Switch main:

``` bash
git checkout main
```

Merge:

``` bash
git merge feature-login
```

Verify:

``` bash
git log
```

------------------------------------------------------------------------

# Practice 7 --- Merge Conflict Practice

## Scenario

Two developers modify the same file.

Developer A:

    Update login message

Developer B:

    Update login validation

------------------------------------------------------------------------

## Steps

Create two branches:

``` bash
git checkout -b developer-a

git checkout -b developer-b
```

Modify same file.

Merge:

``` bash
git merge developer-a
```

Resolve conflict manually.

Complete:

``` bash
git add .

git commit
```

------------------------------------------------------------------------

# Practice 8 --- Rebase Practice

Scenario:

Update feature branch with latest main.

Commands:

``` bash
git checkout feature-login

git rebase main
```

Practice:

-   Resolve conflicts
-   Continue rebase

Command:

``` bash
git rebase --continue
```

------------------------------------------------------------------------

# Practice 9 --- Interactive Rebase

Create multiple commits:

    Commit A

    Commit B

    Commit C

Run:

``` bash
git rebase -i HEAD~3
```

Practice:

-   Squash commits
-   Change messages
-   Remove commits

------------------------------------------------------------------------

# Practice 10 --- Cherry Pick Practice

Scenario:

Bug fix exists in another branch.

Find commit:

``` bash
git log
```

Apply:

``` bash
git cherry-pick commit_id
```

Verify:

``` bash
git log
```

------------------------------------------------------------------------

# Practice 11 --- Stash Practice

Scenario:

Working on feature.

Urgent bug arrives.

Save changes:

``` bash
git stash
```

Check stash:

``` bash
git stash list
```

Restore:

``` bash
git stash pop
```

------------------------------------------------------------------------

# Practice 12 --- Tag Practice

Scenario:

Release version 1.0.

Create tag:

``` bash
git tag -a v1.0 -m "Release version 1.0"
```

View tags:

``` bash
git tag
```

View details:

``` bash
git show v1.0
```

------------------------------------------------------------------------

# Practice 13 --- Remote Repository Practice

Connect remote:

``` bash
git remote add origin URL
```

Check:

``` bash
git remote -v
```

Push:

``` bash
git push origin main
```

------------------------------------------------------------------------

# Practice 14 --- GitHub Workflow Practice

Complete workflow:

``` text
Clone Repository

      ↓

Create Branch

      ↓

Develop Feature

      ↓

Commit

      ↓

Push Branch

      ↓

Create Pull Request

      ↓

Code Review

      ↓

Merge
```

------------------------------------------------------------------------

# Practice 15 --- .gitignore Practice

Create:

    .gitignore

Add:

    node_modules/

    .env

    build/

Commit:

``` bash
git add .

git commit -m "Add gitignore"
```

------------------------------------------------------------------------

# Practice 16 --- Scenario Questions

## Scenario 1

You accidentally committed wrong code.

Solution:

``` bash
git revert commit_id
```

------------------------------------------------------------------------

## Scenario 2

Your push is rejected.

Reason:

Remote has newer changes.

Solution:

``` bash
git pull

resolve conflicts

git push
```

------------------------------------------------------------------------

## Scenario 3

You need one commit from another branch.

Solution:

``` bash
git cherry-pick commit_id
```

------------------------------------------------------------------------

## Scenario 4

You need to switch branches with unfinished work.

Solution:

``` bash
git stash
```

------------------------------------------------------------------------

# Practice Project

## Build Workflow for E-Commerce Application

Branches:

    main

     |

    develop

     |

    feature-cart

     |

    feature-payment

Tasks:

1.  Create repository
2.  Create branches
3.  Add features
4.  Commit changes
5.  Merge branches
6.  Resolve conflicts
7.  Create release tag

------------------------------------------------------------------------

# Git Command Practice Sheet

  Task                Command
  ------------------- -----------------
  Create repository   git init
  Clone repository    git clone
  Check status        git status
  Add files           git add
  Commit              git commit
  View history        git log
  Create branch       git branch
  Switch branch       git switch
  Merge               git merge
  Rebase              git rebase
  Cherry pick         git cherry-pick
  Stash               git stash
  Create tag          git tag
  Push                git push
  Pull                git pull

------------------------------------------------------------------------

# Mini Interview Practice

## Question 1

Explain Git workflow.

Answer:

    Clone

    ↓

    Branch

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

------------------------------------------------------------------------

## Question 2

Difference between merge and rebase?

Answer:

Merge combines history.

Rebase creates a cleaner linear history.

------------------------------------------------------------------------

## Question 3

When do you use stash?

Answer:

When temporary unfinished changes need to be saved before switching
tasks.

------------------------------------------------------------------------

# Practice Checklist

✓ Repository created

✓ Commits created

✓ Branches created

✓ Merge performed

✓ Conflict resolved

✓ Rebase practiced

✓ Cherry-pick performed

✓ Stash used

✓ Tags created

✓ Remote connected

✓ Pull Request workflow understood

------------------------------------------------------------------------

# Summary

Practical Git knowledge comes from repeated usage. By practicing
repositories, commits, branches, merges, rebases, stash, tags, and
GitHub workflows, developers build confidence in real-world version
control operations.
