# Lesson 164 --- Git & Version Control Revision Notes

# Part 10 --- Version Control Systems

> **Objective**
>
> Revise complete Git and Version Control concepts including Git
> fundamentals, architecture, repositories, commits, branches, merging,
> rebase, cherry-pick, stash, tags, GitHub workflow, best practices,
> important commands, and interview-focused points.

------------------------------------------------------------------------

# 1. Version Control System Overview

A Version Control System (VCS) manages changes in software projects.

It helps developers:

-   Track modifications
-   Maintain history
-   Collaborate
-   Restore previous versions

Types:

    Centralized VCS

            ↓

    Distributed VCS

            ↓

    Git

------------------------------------------------------------------------

# 2. Git Fundamentals

## What is Git?

Git is a distributed version control system used to track source code
changes.

Created by:

    Linus Torvalds

in 2005.

------------------------------------------------------------------------

# Why Git?

Git provides:

-   Distributed architecture
-   Fast operations
-   Offline support
-   Powerful branching
-   Reliable history tracking

------------------------------------------------------------------------

# Git vs GitHub

  Git                    GitHub
  ---------------------- ---------------------
  Version control tool   Hosting platform
  Works locally          Cloud collaboration
  Tracks changes         Stores repositories

------------------------------------------------------------------------

# 3. Git Architecture

Git follows:

    Working Directory

            ↓

    Staging Area

            ↓

    Local Repository

            ↓

    Remote Repository

------------------------------------------------------------------------

# Git Internal Objects

Git stores data as objects:

## Blob

Stores file content.

## Tree

Stores folder structure.

## Commit

Stores snapshots.

## Tag

Marks important commits.

------------------------------------------------------------------------

# .git Directory

Contains:

    .git

    ├── objects

    ├── refs

    ├── HEAD

    ├── index

    └── config

------------------------------------------------------------------------

# 4. Git Repository

A repository stores:

-   Source code
-   Commits
-   Branches
-   History
-   Metadata

Types:

    Local Repository

    Remote Repository

------------------------------------------------------------------------

# Important Repository Commands

Create:

``` bash
git init
```

Clone:

``` bash
git clone URL
```

Status:

``` bash
git status
```

------------------------------------------------------------------------

# 5. Git Commit

A commit is a snapshot of staged changes.

Workflow:

    Modify Files

          ↓

    git add

          ↓

    git commit

          ↓

    History Updated

------------------------------------------------------------------------

# Good Commit Practices

-   Small commits
-   Meaningful messages
-   One logical change per commit

Example:

Good:

    Fix payment validation issue

Bad:

    update

------------------------------------------------------------------------

# 6. Git Branch

A branch is an independent development path.

Used for:

-   Features
-   Bug fixes
-   Experiments

Example:

    main

     |

    feature-login

------------------------------------------------------------------------

# Branch Commands

Create:

``` bash
git branch feature-name
```

Create and switch:

``` bash
git checkout -b feature-name
```

View:

``` bash
git branch
```

------------------------------------------------------------------------

# 7. Git Merge

Merge combines branches.

Command:

``` bash
git merge branch-name
```

Types:

## Fast Forward Merge

Moves branch pointer.

## Three Way Merge

Creates merge commit.

------------------------------------------------------------------------

# 8. Merge Conflicts

Occurs when Git cannot automatically combine changes.

Reasons:

-   Same lines modified
-   File deleted in another branch
-   Different changes overlap

Resolution:

    Find Conflict

    ↓

    Edit File

    ↓

    Remove Markers

    ↓

    git add

    ↓

    git commit

------------------------------------------------------------------------

# 9. Git Rebase

Rebase moves commits onto another branch.

Command:

``` bash
git rebase main
```

Benefits:

-   Cleaner history
-   Linear commits

Avoid on:

-   Shared branches
-   Production history

------------------------------------------------------------------------

# Merge vs Rebase

  Merge                  Rebase
  ---------------------- ------------------
  Preserves history      Rewrites history
  Creates merge commit   Linear history
  Safer                  Cleaner

------------------------------------------------------------------------

# 10. Git Cherry Pick

Cherry pick applies a specific commit.

Command:

``` bash
git cherry-pick commit_id
```

Used for:

-   Hotfixes
-   Backporting
-   Selective changes

------------------------------------------------------------------------

# 11. Git Stash

Stash temporarily stores unfinished changes.

Command:

``` bash
git stash
```

Restore:

``` bash
git stash pop
```

Used when:

-   Switching branches
-   Saving incomplete work

------------------------------------------------------------------------

# 12. Git Tag

Tag marks important commits.

Example:

    v1.0.0

Types:

-   Lightweight Tag
-   Annotated Tag

Create:

``` bash
git tag v1.0
```

------------------------------------------------------------------------

# 13. Remote Repository

Remote repository enables team collaboration.

Examples:

-   GitHub
-   GitLab
-   Bitbucket

------------------------------------------------------------------------

# Remote Commands

Add remote:

``` bash
git remote add origin URL
```

Push:

``` bash
git push
```

Pull:

``` bash
git pull
```

Fetch:

``` bash
git fetch
```

------------------------------------------------------------------------

# 14. GitHub Workflow

Professional workflow:

    Clone Repository

            ↓

    Create Branch

            ↓

    Write Code

            ↓

    Commit

            ↓

    Push

            ↓

    Pull Request

            ↓

    Code Review

            ↓

    Merge

------------------------------------------------------------------------

# 15. Pull Request

A Pull Request requests merging changes into another branch.

Provides:

-   Code review
-   Discussion
-   Automated checks
-   Approval process

------------------------------------------------------------------------

# 16. Code Review

Code review checks:

-   Functionality
-   Readability
-   Security
-   Performance
-   Testing

Benefits:

-   Better quality
-   Knowledge sharing
-   Early bug detection

------------------------------------------------------------------------

# 17. Git Best Practices

## Commits

✓ Small commits

✓ Clear messages

✓ Avoid secrets

------------------------------------------------------------------------

## Branches

✓ Feature branches

✓ Protected main branch

✓ Meaningful names

------------------------------------------------------------------------

## Collaboration

✓ Pull before push

✓ Review code

✓ Resolve conflicts carefully

------------------------------------------------------------------------

# Important Git Commands Cheat Sheet

  Task          Command
  ------------- -----------------
  Initialize    git init
  Clone         git clone
  Status        git status
  Add           git add
  Commit        git commit
  Log           git log
  Branch        git branch
  Switch        git switch
  Merge         git merge
  Rebase        git rebase
  Cherry Pick   git cherry-pick
  Stash         git stash
  Tag           git tag
  Push          git push
  Pull          git pull
  Fetch         git fetch

------------------------------------------------------------------------

# Common Interview Topics

Frequently asked:

1.  Git vs GitHub
2.  Git architecture
3.  Commit lifecycle
4.  Branching strategy
5.  Merge vs Rebase
6.  Conflict resolution
7.  Cherry-pick usage
8.  Stash usage
9.  Pull Request workflow
10. Code review process

------------------------------------------------------------------------

# Real-World Developer Workflow

    Create Issue

          ↓

    Create Branch

          ↓

    Develop Feature

          ↓

    Commit Changes

          ↓

    Push Branch

          ↓

    Pull Request

          ↓

    Code Review

          ↓

    Merge

          ↓

    Release

------------------------------------------------------------------------

# Final Revision Checklist

✓ Understand Git architecture

✓ Know repository concepts

✓ Create commits properly

✓ Manage branches

✓ Perform merges

✓ Resolve conflicts

✓ Understand rebase

✓ Use cherry-pick

✓ Manage stashes

✓ Create tags

✓ Work with remotes

✓ Follow GitHub workflow

✓ Apply best practices

------------------------------------------------------------------------

# Summary

Git is an essential tool in modern software development. Strong Git
knowledge requires understanding not only commands but also workflows,
collaboration practices, branching strategies, and safe methods for
managing software changes.

A professional developer uses Git to maintain clean history, collaborate
effectively, and deliver reliable software.
