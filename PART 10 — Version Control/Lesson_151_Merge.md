# Lesson 151 --- Merge

# Part 10 --- Version Control Systems

> **Objective**
>
> Understand Git Merge, why merging is required, merge workflow, types
> of merges, merge strategies, fast-forward merge, three-way merge, and
> best practices for combining changes in software projects.

------------------------------------------------------------------------

# Introduction

Developers often work on different branches.

After completing work, changes need to be combined into the main
codebase.

Git Merge performs this combination.

``` text
Feature Branch

      ↓

    Merge

      ↓

Main Branch
```

------------------------------------------------------------------------

# What is Git Merge?

**Git Merge** is the process of combining changes from one branch into
another branch.

Example:

    main

    A --- B --- C


    feature

    A --- B --- D --- E

After merge:

    A --- B --- C --- M

              \

               D --- E

------------------------------------------------------------------------

# Why Do We Need Merge?

Without merging:

``` text
Feature Work

      ↓

Separate Branch

      ↓

Never Added to Product
```

Merge helps:

-   Combine features
-   Integrate team work
-   Deliver completed changes
-   Maintain project history

------------------------------------------------------------------------

# Merge Workflow

Typical workflow:

``` text
Create Feature Branch

        ↓

Develop Feature

        ↓

Commit Changes

        ↓

Switch to Main

        ↓

Merge Branch

        ↓

Test Code
```

------------------------------------------------------------------------

# Basic Merge Command

Command:

``` bash
git merge branch_name
```

Example:

``` bash
git merge feature-login
```

This merges `feature-login` into the current branch.

------------------------------------------------------------------------

# Example Merge Process

Branches:

    main

    A --- B


    feature

    A --- B --- C --- D

Command:

``` bash
git checkout main

git merge feature
```

Result:

    A --- B --- C --- D

------------------------------------------------------------------------

# Types of Git Merge

Main types:

``` text
Fast-Forward Merge

Three-Way Merge
```

------------------------------------------------------------------------

# 1. Fast-Forward Merge

Occurs when the main branch has no new commits.

Example:

Before:

    main

    A --- B


    feature

    A --- B --- C

After:

    main

    A --- B --- C

Git simply moves the branch pointer forward.

------------------------------------------------------------------------

# Advantages of Fast-Forward Merge

-   Simple history
-   No extra merge commit
-   Easy to understand

------------------------------------------------------------------------

# 2. Three-Way Merge

Occurs when both branches have new commits.

Example:

Before:

            C

           /

    A --- B

           \

            D

After:

            C

           /

    A --- B --- M

           \

            D

Git creates a new merge commit.

------------------------------------------------------------------------

# Merge Commit

A merge commit combines two histories.

Contains:

-   Two parent commits
-   Merge information
-   Final combined state

Example:

    Merge Commit

     |

     |-- Parent 1

     |-- Parent 2

------------------------------------------------------------------------

# Merge Strategies

Git provides different strategies.

------------------------------------------------------------------------

# 1. Recursive Merge

Default strategy for many situations.

Used when:

-   Two branches diverged
-   History needs comparison

------------------------------------------------------------------------

# 2. Resolve Strategy

Simple merge strategy.

Used for:

-   Smaller merges

------------------------------------------------------------------------

# 3. Octopus Merge

Used for merging multiple branches.

Example:

    Branch A

    Branch B

    Branch C

          ↓

    Merge

------------------------------------------------------------------------

# Checking Merge Status

Command:

``` bash
git status
```

Shows:

-   Merge progress
-   Conflicts
-   Remaining actions

------------------------------------------------------------------------

# Aborting a Merge

If merge causes problems:

Command:

``` bash
git merge --abort
```

Returns repository to previous state.

------------------------------------------------------------------------

# Merge vs Rebase

  Merge                  Rebase
  ---------------------- ------------------------
  Creates merge commit   Rewrites history
  Preserves history      Creates linear history
  Safer                  Requires caution

------------------------------------------------------------------------

# Merge Example in Industry

## E-Commerce Application

Developer A:

    Feature Cart

Developer B:

    Feature Payment

Branches:

    feature-cart

    feature-payment

After review:

    Merge

    ↓

    Main Branch

    ↓

    Release

------------------------------------------------------------------------

# Merge Best Practices

-   Pull latest changes before merging
-   Merge small changes frequently
-   Test after merging
-   Resolve conflicts carefully
-   Review merge results

------------------------------------------------------------------------

# Common Merge Problems

## Problem 1

Merge conflicts.

Cause:

Same file modified by multiple developers.

Solution:

Resolve conflicts manually.

------------------------------------------------------------------------

## Problem 2

Large complicated merges.

Solution:

Merge regularly.

------------------------------------------------------------------------

## Problem 3

Merging unfinished code.

Solution:

Merge only tested changes.

------------------------------------------------------------------------

# Interview Questions

1.  What is Git Merge?
2.  Why is merging required?
3.  Explain merge workflow.
4.  What is fast-forward merge?
5.  What is three-way merge?
6.  What is a merge commit?
7.  Difference between merge and rebase?
8.  How do you abort a merge?
9.  What causes merge conflicts?

------------------------------------------------------------------------

# Cheat Sheet

``` text
Git Merge

Feature Branch

      ↓

git merge

      ↓

Combine Changes

      ↓

Test

      ↓

Final Code
```

------------------------------------------------------------------------

# Summary

Git Merge combines changes from different branches into a single
codebase. Understanding fast-forward merges, three-way merges, merge
commits, and merge strategies helps developers collaborate effectively
and maintain clean software development workflows.
