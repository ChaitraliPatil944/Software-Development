# Lesson 154 --- Cherry Pick

# Part 10 --- Version Control Systems

> **Objective**
>
> Understand Git Cherry Pick, why it is used, how to apply specific
> commits from one branch to another, cherry-pick workflow, conflict
> handling, comparison with merge and rebase, and real-world usage
> scenarios.

------------------------------------------------------------------------

# Introduction

Sometimes developers do not need an entire branch.

They only need one specific change from another branch.

Git Cherry Pick solves this problem.

``` text
Branch A

Commit 1

Commit 2

Commit 3


Need only Commit 2

        ↓

Cherry Pick

        ↓

Branch B
```

------------------------------------------------------------------------

# What is Git Cherry Pick?

**Git Cherry Pick** is a Git command that applies the changes introduced
by a specific commit from one branch onto another branch.

It copies the commit changes without merging the entire branch.

------------------------------------------------------------------------

# Why Do We Need Cherry Pick?

Without cherry pick:

``` text
Need One Fix

      ↓

Merge Entire Branch

      ↓

Unwanted Changes Included
```

Cherry pick helps:

-   Apply specific bug fixes
-   Move selected features
-   Recover important commits
-   Share individual changes

------------------------------------------------------------------------

# Cherry Pick vs Merge

## Merge

Combines entire branches.

Example:

    Feature Branch

    A---B---C

            ↓

    Merge

            ↓

    Main

------------------------------------------------------------------------

## Cherry Pick

Copies only selected commits.

Example:

    Feature Branch

    A---B---C

    Need B only

            ↓

    Cherry Pick

            ↓

    Main

------------------------------------------------------------------------

# Cherry Pick Command

Syntax:

``` bash
git cherry-pick commit_id
```

Example:

``` bash
git cherry-pick a83f9d7
```

Git creates a new commit containing the same changes.

------------------------------------------------------------------------

# How Cherry Pick Works?

Suppose:

    main

    A---B


    feature

    A---B---C---D

Need commit C.

Command:

``` bash
git cherry-pick C
```

Result:

    main

    A---B---C'

C' contains the same changes as C but has a different commit ID.

------------------------------------------------------------------------

# Cherry Pick Workflow

``` text
Identify Commit

        ↓

Copy Commit ID

        ↓

Switch Target Branch

        ↓

Run Cherry Pick

        ↓

Resolve Conflicts

        ↓

Commit Applied
```

------------------------------------------------------------------------

# Finding Commit ID

Command:

``` bash
git log
```

Example:

    commit a83f9d7

    Fix payment issue

Use:

``` bash
git cherry-pick a83f9d7
```

------------------------------------------------------------------------

# Cherry Pick Multiple Commits

## Multiple Individual Commits

Example:

``` bash
git cherry-pick abc123 def456
```

------------------------------------------------------------------------

## Range of Commits

Example:

``` bash
git cherry-pick A..D
```

Applies commits between A and D.

------------------------------------------------------------------------

# Cherry Pick Conflict

A conflict occurs when:

-   Target branch has different changes
-   Same code area is modified

Example:

    Commit Changes

            +

    Current Branch Changes

            ↓

    Conflict

------------------------------------------------------------------------

# Resolving Cherry Pick Conflicts

Steps:

``` text
Conflict Detected

        ↓

Edit Files

        ↓

Remove Conflict Markers

        ↓

git add

        ↓

git cherry-pick --continue
```

------------------------------------------------------------------------

# Aborting Cherry Pick

If you want to cancel:

Command:

``` bash
git cherry-pick --abort
```

Returns to previous state.

------------------------------------------------------------------------

# Cherry Pick Example

## Production Bug Fix

Scenario:

Production has a critical bug.

Fix exists in development branch.

Branches:

    development

    A---B---C(fix)


    production

    A---B

Need only C.

Command:

``` bash
git cherry-pick C
```

Result:

    production

    A---B---C'

Bug fix applied without bringing unfinished features.

------------------------------------------------------------------------

# Real-World Use Cases

## 1. Hotfix Deployment

Apply urgent fixes to production.

------------------------------------------------------------------------

## 2. Backport Changes

Move fixes to older release versions.

Example:

    Version 2.0

    ↓

    Version 1.5 Fix

------------------------------------------------------------------------

## 3. Selective Feature Migration

Move specific functionality.

------------------------------------------------------------------------

# Cherry Pick vs Rebase

  Cherry Pick                 Rebase
  --------------------------- -----------------------------
  Copies selected commits     Moves entire branch history
  Creates new commits         Rewrites history
  Used for specific changes   Used for branch cleanup

------------------------------------------------------------------------

# Cherry Pick vs Merge vs Rebase

  Feature             Merge   Rebase   Cherry Pick
  ------------------- ------- -------- -------------
  Combines branches   Yes     No       No
  Copies commits      No      Yes      Yes
  Rewrites history    No      Yes      No
  Selective changes   No      No       Yes

------------------------------------------------------------------------

# Advantages of Cherry Pick

-   Selective changes
-   Useful for emergency fixes
-   Easy backporting
-   Avoids unnecessary merges

------------------------------------------------------------------------

# Disadvantages of Cherry Pick

-   Creates duplicate commits
-   Can create confusion
-   Requires careful tracking

------------------------------------------------------------------------

# Best Practices

-   Use cherry pick for small targeted changes
-   Document why commit was cherry-picked
-   Avoid excessive cherry picking
-   Test after applying changes
-   Communicate with team

------------------------------------------------------------------------

# Common Mistakes

## Mistake 1

Cherry picking many commits.

Solution:

Consider merging instead.

------------------------------------------------------------------------

## Mistake 2

Cherry picking without understanding dependencies.

Solution:

Check related commits.

------------------------------------------------------------------------

## Mistake 3

Ignoring conflicts.

Solution:

Resolve and test carefully.

------------------------------------------------------------------------

# Interview Questions

1.  What is Git Cherry Pick?
2.  Why is cherry pick used?
3.  How does cherry pick work?
4.  Difference between cherry pick and merge?
5.  Difference between cherry pick and rebase?
6.  How do you resolve cherry-pick conflicts?
7.  Explain real-world use cases of cherry pick.

------------------------------------------------------------------------

# Cheat Sheet

``` text
Git Cherry Pick

Find Commit ID

      ↓

Switch Branch

      ↓

git cherry-pick commit_id

      ↓

Resolve Conflicts

      ↓

Commit Applied
```

------------------------------------------------------------------------

# Summary

Git Cherry Pick allows developers to apply specific commits from one
branch to another without merging the complete branch. It is especially
useful for hotfixes, backporting changes, and selective feature
migration when only a particular change is required.
