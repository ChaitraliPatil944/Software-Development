# Lesson 153 --- Rebase

# Part 10 --- Version Control Systems

> **Objective**
>
> Understand Git Rebase, why rebase is used, how rebase works
> internally, differences between merge and rebase, interactive rebase,
> rewriting history, squashing commits, workflow, and best practices.

------------------------------------------------------------------------

# Introduction

In Git, developers often need to combine changes from different
branches.

There are two common approaches:

1.  Merge
2.  Rebase

Both integrate changes, but they work differently.

``` text
Merge

Combines Histories


Rebase

Moves History
```

------------------------------------------------------------------------

# What is Git Rebase?

**Git Rebase** is a Git operation that moves or reapplies commits from
one branch onto another branch.

It creates a cleaner and linear project history.

Example:

Before:

            C
           /
    A --- B
           \
            D

After rebase:

    A --- B --- D --- C

------------------------------------------------------------------------

# Why Do We Need Rebase?

Rebase helps:

-   Maintain clean history
-   Avoid unnecessary merge commits
-   Make commit history easier to understand
-   Prepare branches before merging

------------------------------------------------------------------------

# Merge vs Rebase

  Merge                       Rebase
  --------------------------- ---------------------------
  Combines branches           Moves commits
  Creates merge commit        Rewrites history
  Preserves history           Creates linear history
  Safer for shared branches   Better for local branches

------------------------------------------------------------------------

# How Rebase Works?

Suppose:

    main

    A --- B --- C


    feature

    A --- B --- D --- E

Main receives new commits:

    main

    A --- B --- C --- F

Feature is rebased:

``` bash
git rebase main
```

Git:

1.  Temporarily removes feature commits
2.  Moves feature branch to latest main
3.  Reapplies feature commits

Result:

    A --- B --- C --- F --- D' --- E'

New commits are created because history changes.

------------------------------------------------------------------------

# Rebase Workflow

Typical workflow:

``` text
Update Main Branch

        ↓

Switch Feature Branch

        ↓

Run Rebase

        ↓

Resolve Conflicts

        ↓

Continue Rebase

        ↓

Push Changes
```

------------------------------------------------------------------------

# Basic Rebase Command

Command:

``` bash
git rebase branch_name
```

Example:

``` bash
git checkout feature-login

git rebase main
```

------------------------------------------------------------------------

# Rebase Conflict Handling

Conflicts may occur during rebase.

Process:

``` text
Conflict Detected

        ↓

Fix Files

        ↓

git add

        ↓

git rebase --continue
```

------------------------------------------------------------------------

# Aborting Rebase

If rebase becomes complicated:

Command:

``` bash
git rebase --abort
```

Returns repository to previous state.

------------------------------------------------------------------------

# Interactive Rebase

Interactive rebase allows modifying commits.

Command:

``` bash
git rebase -i HEAD~n
```

Example:

``` bash
git rebase -i HEAD~3
```

Allows editing last 3 commits.

------------------------------------------------------------------------

# Interactive Rebase Operations

Options:

## Pick

Keep commit.

Example:

    pick abc123 Add login

------------------------------------------------------------------------

## Reword

Change commit message.

Example:

    reword abc123 Update message

------------------------------------------------------------------------

## Squash

Combine commits.

Example:

    pick Add feature

    squash Fix bug

Result:

    One clean commit

------------------------------------------------------------------------

## Drop

Remove commit.

------------------------------------------------------------------------

# Squashing Commits

Squashing combines multiple commits into one.

Before:

    Commit A

    Commit B

    Commit C

After:

    Single Commit

Benefits:

-   Cleaner history
-   Easier review

------------------------------------------------------------------------

# Rebase Example

Developer creates:

    Commit 1

    Commit 2

    Commit 3

Before submitting pull request:

``` bash
git rebase -i HEAD~3
```

Squash:

    Feature Implementation

Now reviewers see a cleaner history.

------------------------------------------------------------------------

# When Should We Use Rebase?

Good use cases:

-   Cleaning local commits
-   Updating feature branches
-   Preparing pull requests
-   Maintaining linear history

------------------------------------------------------------------------

# When Should We Avoid Rebase?

Avoid rebasing:

-   Public shared branches
-   Production history
-   Commits already used by others

Reason:

Rebase changes commit history.

------------------------------------------------------------------------

# Rebase in Industry

Typical workflow:

    Developer

     ↓

    Feature Branch

     ↓

    Rebase with Main

     ↓

    Code Review

     ↓

    Merge

------------------------------------------------------------------------

# Rebase vs Merge Example

## Merge

History:

    A---B---C
         \

          D---E

               \

                Merge Commit

------------------------------------------------------------------------

## Rebase

History:

    A---B---C---D'---E'

------------------------------------------------------------------------

# Advantages of Rebase

-   Cleaner history
-   Easier debugging
-   Better commit organization
-   Avoids unnecessary merge commits

------------------------------------------------------------------------

# Disadvantages of Rebase

-   Rewrites history
-   Can create conflicts
-   Dangerous on shared branches

------------------------------------------------------------------------

# Best Practices

-   Rebase before creating pull requests
-   Do not rebase public branches
-   Create backups before complex rebases
-   Understand history changes
-   Test after rebasing

------------------------------------------------------------------------

# Common Mistakes

## Mistake 1

Rebasing shared branches.

Solution:

Only rebase personal branches.

------------------------------------------------------------------------

## Mistake 2

Using rebase without understanding.

Solution:

Practice on test repositories.

------------------------------------------------------------------------

## Mistake 3

Ignoring conflicts.

Solution:

Resolve carefully and test.

------------------------------------------------------------------------

# Interview Questions

1.  What is Git Rebase?
2.  Difference between merge and rebase?
3.  How does rebase work internally?
4.  What is interactive rebase?
5.  Explain squash in Git.
6.  What happens during rebase conflict?
7.  When should you avoid rebase?
8.  Why does rebase rewrite history?

------------------------------------------------------------------------

# Cheat Sheet

``` text
Git Rebase

Update Main

      ↓

Switch Branch

      ↓

git rebase main

      ↓

Resolve Conflicts

      ↓

Continue

      ↓

Clean History
```

------------------------------------------------------------------------

# Summary

Git Rebase is a powerful tool for reorganizing commit history and
creating a clean linear development timeline. It is useful for local
feature branches and code preparation, but it must be used carefully
because it rewrites commit history.
