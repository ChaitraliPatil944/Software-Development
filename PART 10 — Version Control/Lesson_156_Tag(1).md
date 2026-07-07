# Lesson 156 --- Tag

# Part 10 --- Version Control Systems

> **Objective**
>
> Understand Git Tags, why tags are used, types of tags, creating and
> managing tags, tagging software releases, sharing tags with remote
> repositories, and best practices for version management.

------------------------------------------------------------------------

# Introduction

Software projects often have important milestones:

-   Version releases
-   Stable builds
-   Production deployments

Git Tags help mark these important points in project history.

``` text
Commit History

C1 ---- C2 ---- C3 ---- C4

                 ↑

              Version 1.0
```

------------------------------------------------------------------------

# What is a Git Tag?

A **Git Tag** is a reference that points to a specific commit in Git
history.

Tags are commonly used to mark:

-   Software releases
-   Stable versions
-   Important milestones

Example:

    v1.0

     ↓

    Release Commit

------------------------------------------------------------------------

# Why Do We Need Git Tags?

Without tags:

``` text
Many Commits

      ↓

Difficult to Find Release Version
```

Tags help:

-   Identify releases
-   Track versions
-   Simplify deployment
-   Reference important commits

------------------------------------------------------------------------

# Git Tag Architecture

A tag points to a commit.

Example:

    Tag

     ↓

    Commit

     ↓

    Tree

     ↓

    Files

------------------------------------------------------------------------

# Types of Git Tags

Git provides two main types:

``` text
Lightweight Tag

Annotated Tag
```

------------------------------------------------------------------------

# 1. Lightweight Tag

A lightweight tag is a simple pointer to a commit.

It contains:

-   Commit reference

Example:

    v1.0

     ↓

    Commit

------------------------------------------------------------------------

# Creating Lightweight Tag

Command:

``` bash
git tag tag_name
```

Example:

``` bash
git tag v1.0
```

------------------------------------------------------------------------

# 2. Annotated Tag

Annotated tags contain additional information.

They store:

-   Tag author
-   Date
-   Message
-   Signature

Example:

``` bash
git tag -a v1.0 -m "Release version 1.0"
```

------------------------------------------------------------------------

# Lightweight vs Annotated Tag

  Lightweight Tag    Annotated Tag
  ------------------ --------------------------
  Simple reference   Full Git object
  No metadata        Contains metadata
  Quick tagging      Recommended for releases

------------------------------------------------------------------------

# Viewing Tags

Command:

``` bash
git tag
```

Example:

    v1.0

    v1.1

    v2.0

------------------------------------------------------------------------

# Viewing Tag Details

Command:

``` bash
git show tag_name
```

Example:

``` bash
git show v1.0
```

Shows:

-   Commit information
-   Tag message
-   Changes

------------------------------------------------------------------------

# Creating Tags on Specific Commit

Command:

``` bash
git tag tag_name commit_id
```

Example:

``` bash
git tag v1.0 a83f9d7
```

Creates tag on a previous commit.

------------------------------------------------------------------------

# Deleting Tags

## Delete Local Tag

Command:

``` bash
git tag -d tag_name
```

Example:

``` bash
git tag -d v1.0
```

------------------------------------------------------------------------

# Remote Tags

Tags are not automatically pushed.

To push a tag:

``` bash
git push origin tag_name
```

Example:

``` bash
git push origin v1.0
```

------------------------------------------------------------------------

# Push All Tags

Command:

``` bash
git push origin --tags
```

Uploads all tags.

------------------------------------------------------------------------

# Deleting Remote Tags

Command:

``` bash
git push origin --delete tag_name
```

Example:

``` bash
git push origin --delete v1.0
```

------------------------------------------------------------------------

# Checking Out Tags

A tag can be checked out.

Command:

``` bash
git checkout tag_name
```

Example:

``` bash
git checkout v1.0
```

This creates a detached HEAD state.

------------------------------------------------------------------------

# Tag Workflow

Typical release process:

``` text
Complete Development

        ↓

Create Release Commit

        ↓

Create Tag

        ↓

Push Tag

        ↓

Deploy Version
```

------------------------------------------------------------------------

# Industry Example

## Software Release

Project history:

    Commit 1

    Commit 2

    Commit 3

    Commit 4

Production release:

    Commit 4

    ↓

    Tag:

    v2.0

Now teams can easily identify the production version.

------------------------------------------------------------------------

# Semantic Versioning

Many projects follow:

    MAJOR.MINOR.PATCH

Example:

    2.5.1

Meaning:

## Major

Breaking changes.

Example:

    3.0.0

------------------------------------------------------------------------

## Minor

New features.

Example:

    2.6.0

------------------------------------------------------------------------

## Patch

Bug fixes.

Example:

    2.5.2

------------------------------------------------------------------------

# Git Tag Best Practices

-   Use meaningful version names
-   Prefer annotated tags for releases
-   Follow semantic versioning
-   Tag stable versions only
-   Document release changes

------------------------------------------------------------------------

# Common Mistakes

## Mistake 1

Tagging unfinished code.

Solution:

Tag only stable releases.

------------------------------------------------------------------------

## Mistake 2

Forgetting to push tags.

Solution:

Use:

``` bash
git push --tags
```

------------------------------------------------------------------------

## Mistake 3

Using unclear tag names.

Bad:

    release1

Good:

    v1.0.0

------------------------------------------------------------------------

# Tag vs Branch

  Tag                      Branch
  ------------------------ ------------------------
  Points to fixed commit   Moves with new commits
  Used for releases        Used for development
  Usually permanent        Frequently changed

------------------------------------------------------------------------

# Tag vs Commit

  Tag                   Commit
  --------------------- ---------------------
  Reference to commit   Snapshot of changes
  Marks importance      Stores changes

------------------------------------------------------------------------

# Interview Questions

1.  What is a Git Tag?
2.  Why are tags used?
3.  Difference between lightweight and annotated tags?
4.  How do you create a tag?
5.  How do you push tags to remote?
6.  Difference between tag and branch?
7.  Explain semantic versioning.
8.  How do you delete a tag?

------------------------------------------------------------------------

# Cheat Sheet

``` text
Git Tag

Stable Commit

      ↓

Create Tag

      ↓

Version Name

      ↓

Push Tag

      ↓

Release Software
```

------------------------------------------------------------------------

# Summary

Git Tags are used to mark important commits such as software releases
and stable versions. They provide a simple way to identify and manage
different versions of software throughout the development lifecycle.
