# Lesson 149 --- Commit

# Part 10 --- Version Control Systems

> **Objective**
>
> Understand Git commits, how commits work internally, commit lifecycle,
> creating commits, commit history, commit messages, atomic commits,
> amending commits, reset vs revert, and professional commit practices.

------------------------------------------------------------------------

# Introduction

A commit is one of the most important concepts in Git.

Every meaningful change in a project should be recorded as a commit.

``` text
Code Changes

      ↓

Commit

      ↓

Version History
```

A commit acts like a checkpoint that saves the state of a project at a
specific point in time.

------------------------------------------------------------------------

# What is a Git Commit?

A **Git Commit** is a snapshot of staged changes stored permanently in
the Git repository.

A commit contains:

-   Changed files
-   Author information
-   Timestamp
-   Commit message
-   Parent commit reference

------------------------------------------------------------------------

# Why Do We Need Commits?

Without commits:

``` text
Code Changes

      ↓

No History

      ↓

Cannot Track Changes

      ↓

Difficult Recovery
```

Commits provide:

-   Version history
-   Change tracking
-   Collaboration support
-   Recovery points

------------------------------------------------------------------------

# Commit Lifecycle

The commit process:

``` text
Working Directory

        ↓

git add

        ↓

Staging Area

        ↓

git commit

        ↓

Repository History
```

------------------------------------------------------------------------

# Creating a Commit

## Step 1: Modify Files

Example:

    Login.java

Developer adds a login feature.

------------------------------------------------------------------------

## Step 2: Check Changes

Command:

``` bash
git status
```

Shows modified files.

------------------------------------------------------------------------

## Step 3: Stage Changes

Command:

``` bash
git add Login.java
```

Moves changes to staging area.

------------------------------------------------------------------------

## Step 4: Create Commit

Command:

``` bash
git commit -m "Added login functionality"
```

Git creates a new snapshot.

------------------------------------------------------------------------

# Commit Structure

Internally, a commit contains:

``` text
Commit Object

 |

 |-- Commit ID

 |-- Author

 |-- Date

 |-- Message

 |-- Parent Commit

 |-- Tree Reference
```

------------------------------------------------------------------------

# Commit ID

Every commit has a unique identifier.

Example:

    a83f9d7e2c91...

It is generated using hashing.

Used for:

-   Finding commits
-   Comparing versions
-   Reverting changes

------------------------------------------------------------------------

# Commit History

Git stores commits as a chain.

Example:

``` text
Commit C3

   ↓

Commit C2

   ↓

Commit C1

   ↓

Initial Commit
```

Each commit points to its parent.

------------------------------------------------------------------------

# Viewing Commit History

Command:

``` bash
git log
```

Example output:

    commit a83f9d

    Author: Developer

    Message:
    Added payment module

------------------------------------------------------------------------

# Commit Message

A commit message explains what changed.

Good commit message:

    Fix payment validation error

Bad commit messages:

    update

    changes

    final

Humans have somehow managed to turn "final_final_v2" into a cultural
artifact. Commit messages deserve slightly more dignity.

------------------------------------------------------------------------

# Characteristics of Good Commits

A good commit should be:

## Small

Contains related changes only.

------------------------------------------------------------------------

## Clear

Explains the purpose.

------------------------------------------------------------------------

## Atomic

Represents one logical change.

------------------------------------------------------------------------

# Atomic Commit

An **Atomic Commit** contains one complete logical change.

Example:

Good:

    Add user authentication

Bad:

    Add authentication

    Fix UI

    Update database

    Change documentation

------------------------------------------------------------------------

# Commit Best Practices

## 1. Commit Frequently

Small commits are easier to understand.

------------------------------------------------------------------------

## 2. Write Meaningful Messages

Example:

    Add password reset API

------------------------------------------------------------------------

## 3. Avoid Huge Commits

Large commits are difficult to review.

------------------------------------------------------------------------

## 4. Review Before Commit

Command:

``` bash
git diff
```

------------------------------------------------------------------------

# Viewing Commit Details

Command:

``` bash
git show commit_id
```

Shows:

-   Changed files
-   Author
-   Message
-   Difference

------------------------------------------------------------------------

# Amending a Commit

Sometimes a developer wants to modify the latest commit.

Command:

``` bash
git commit --amend
```

Used for:

-   Fixing message
-   Adding missed changes

Example:

    Old message:

    Add user

    New message:

    Add user authentication

------------------------------------------------------------------------

# Reset vs Revert

Both affect commits but work differently.

------------------------------------------------------------------------

# Git Reset

Moves branch pointer backward.

Example:

    C3

    ↓

    C2

    ↓

    C1

Reset removes commits from current history.

Command:

``` bash
git reset
```

Use carefully.

------------------------------------------------------------------------

# Git Revert

Creates a new commit that reverses previous changes.

Example:

    C3

    ↓

    Revert Commit

    ↓

    C2

    ↓

    C1

Safer for shared repositories.

Command:

``` bash
git revert commit_id
```

------------------------------------------------------------------------

# Reset vs Revert

  Reset                    Revert
  ------------------------ -------------------------
  Removes commit history   Creates new undo commit
  Changes branch pointer   Preserves history
  Riskier                  Safer
  Mostly local use         Shared repository use

------------------------------------------------------------------------

# Commit in Team Development

Typical workflow:

``` text
Developer

 ↓

Create Commit

 ↓

Push

 ↓

Code Review

 ↓

Merge
```

------------------------------------------------------------------------

# Commit Example

## E-Commerce Project

Developer adds cart feature.

Changes:

    CartController.java

    CartService.java

Commands:

``` bash
git add .

git commit -m "Add shopping cart functionality"
```

Result:

    New Commit Created

------------------------------------------------------------------------

# Common Commit Mistakes

## Mistake 1

Committing unfinished code.

Solution:

Commit stable changes.

------------------------------------------------------------------------

## Mistake 2

Poor commit messages.

Solution:

Describe actual changes.

------------------------------------------------------------------------

## Mistake 3

Mixing unrelated changes.

Solution:

Create separate commits.

------------------------------------------------------------------------

# Interview Questions

1.  What is a Git commit?
2.  Why are commits important?
3.  Explain commit lifecycle.
4.  What information does a commit contain?
5.  What is an atomic commit?
6.  Difference between reset and revert?
7.  What is git commit --amend?
8.  What makes a good commit message?

------------------------------------------------------------------------

# Cheat Sheet

``` text
Git Commit

Modify Files

      ↓

git add

      ↓

Staging Area

      ↓

git commit

      ↓

Snapshot Saved

      ↓

History Updated
```

------------------------------------------------------------------------

# Summary

Git commits are snapshots of project changes that create a complete
version history. Understanding commits helps developers track changes,
collaborate safely, recover previous versions, and maintain clean
professional repositories.
