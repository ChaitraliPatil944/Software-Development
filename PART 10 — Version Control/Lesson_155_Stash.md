# Lesson 155 --- Stash

# Part 10 --- Version Control Systems

> **Objective**
>
> Understand Git Stash, why temporary storage of changes is needed, how
> stash works, stash commands, applying and managing stashes, stash
> conflicts, and best practices for handling unfinished work.

------------------------------------------------------------------------

# Introduction

Developers often work on a feature but need to switch tasks suddenly.

Examples:

-   Urgent bug fix arrives
-   Need to change branches
-   Need to pull latest code

Committing incomplete work is usually not a good idea.

Git Stash provides a temporary storage area for unfinished changes.

``` text
Unfinished Changes

        ↓

Git Stash

        ↓

Clean Working Directory

        ↓

Continue Later
```

------------------------------------------------------------------------

# What is Git Stash?

**Git Stash** is a Git feature that temporarily saves modified and
staged changes without creating a commit.

It stores work that is not ready to be committed.

------------------------------------------------------------------------

# Why Do We Need Git Stash?

Without stash:

``` text
Unfinished Work

        ↓

Need Branch Switch

        ↓

Commit Incomplete Code

        ↓

Messy History
```

Stash helps:

-   Save unfinished work
-   Switch branches safely
-   Keep commit history clean
-   Resume work later

------------------------------------------------------------------------

# How Git Stash Works

Before stash:

    Working Directory

    Modified Files

Run:

``` bash
git stash
```

After stash:

    Working Directory

    Clean


    Stash Storage

    Saved Changes

------------------------------------------------------------------------

# Creating a Stash

Command:

``` bash
git stash
```

or:

``` bash
git stash save "message"
```

Example:

``` bash
git stash save "Login feature work"
```

------------------------------------------------------------------------

# Viewing Stashes

Command:

``` bash
git stash list
```

Example:

    stash@{0}: Login feature work

    stash@{1}: Payment changes

------------------------------------------------------------------------

# Applying a Stash

The apply command restores changes.

Command:

``` bash
git stash apply
```

Restores the latest stash.

------------------------------------------------------------------------

# Applying Specific Stash

Command:

``` bash
git stash apply stash@{1}
```

Restores a specific stash.

------------------------------------------------------------------------

# Stash Pop

Command:

``` bash
git stash pop
```

It:

1.  Applies stash changes
2.  Removes stash entry

Workflow:

    Stash

     ↓

    Pop

     ↓

    Changes Restored

     ↓

    Stash Removed

------------------------------------------------------------------------

# Stash Apply vs Stash Pop

  git stash apply   git stash pop
  ----------------- -------------------
  Applies changes   Applies changes
  Keeps stash       Removes stash
  Safer option      Cleans stash list

------------------------------------------------------------------------

# Listing Stashes

Command:

``` bash
git stash list
```

Shows all saved stashes.

Example:

    stash@{0}

    stash@{1}

    stash@{2}

------------------------------------------------------------------------

# Viewing Stash Details

Command:

``` bash
git stash show
```

Shows summary of changes.

For full details:

``` bash
git stash show -p
```

------------------------------------------------------------------------

# Removing Stashes

## Remove Specific Stash

Command:

``` bash
git stash drop stash@{0}
```

------------------------------------------------------------------------

## Remove All Stashes

Command:

``` bash
git stash clear
```

Deletes all stored stashes.

------------------------------------------------------------------------

# Stashing Specific Files

Command:

``` bash
git stash push filename
```

Example:

``` bash
git stash push app.java
```

Only that file is stored.

------------------------------------------------------------------------

# Including Untracked Files

By default, stash does not include untracked files.

Command:

``` bash
git stash -u
```

Stores:

-   Modified files
-   Untracked files

------------------------------------------------------------------------

# Stash Workflow Example

Scenario:

Developer working on login feature.

Suddenly:

    Critical Bug Fix Required

Current changes:

    Login Feature

Steps:

``` bash
git stash
```

Switch branch:

``` bash
git checkout bugfix
```

Fix issue.

Return:

``` bash
git checkout feature-login
```

Restore work:

``` bash
git stash pop
```

------------------------------------------------------------------------

# Stash Conflicts

Conflicts may occur when:

-   Current code changed
-   Stashed code modifies same area

Example:

    Current Branch

    +

    Stashed Changes

    ↓

    Conflict

------------------------------------------------------------------------

# Resolving Stash Conflicts

Steps:

``` text
Identify Conflict

        ↓

Edit Files

        ↓

Remove Conflict Markers

        ↓

git add

        ↓

Commit Changes
```

------------------------------------------------------------------------

# Stash vs Commit

  Stash                 Commit
  --------------------- --------------------
  Temporary storage     Permanent history
  Not shared            Shared with team
  For unfinished work   For completed work

------------------------------------------------------------------------

# Stash vs Branch

  Stash                Branch
  -------------------- -----------------------
  Short-term storage   Long-term development
  Local only           Can be shared
  Quick save           Feature isolation

------------------------------------------------------------------------

# Real-World Example

## Software Team

Developer is working on:

    Payment Feature

Manager requests urgent:

    Security Fix

Solution:

``` text
git stash

↓

Fix Security Issue

↓

Return to Payment Feature

↓

git stash pop
```

------------------------------------------------------------------------

# Best Practices

-   Use stash for temporary work
-   Add stash messages
-   Avoid keeping stashes for months
-   Review changes after applying
-   Commit completed work instead

------------------------------------------------------------------------

# Common Mistakes

## Mistake 1

Using stash instead of commits.

Solution:

Commit finished work.

------------------------------------------------------------------------

## Mistake 2

Forgetting stored changes.

Solution:

Regularly check:

``` bash
git stash list
```

------------------------------------------------------------------------

## Mistake 3

Applying wrong stash.

Solution:

Review stash details first.

------------------------------------------------------------------------

# Interview Questions

1.  What is Git Stash?
2.  Why is stash used?
3.  Difference between stash and commit?
4.  Difference between stash apply and stash pop?
5.  How do you view stashes?
6.  How do you delete a stash?
7.  Can stash include untracked files?
8.  How are stash conflicts resolved?

------------------------------------------------------------------------

# Cheat Sheet

``` text
Git Stash

Modify Code

      ↓

git stash

      ↓

Clean Workspace

      ↓

Switch Task

      ↓

git stash pop

      ↓

Continue Work
```

------------------------------------------------------------------------

# Summary

Git Stash is a temporary storage mechanism that allows developers to
save unfinished changes without committing them. It helps maintain clean
commit history, switch tasks safely, and restore work when needed.
