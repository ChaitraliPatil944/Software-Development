# Lesson 148 --- Git Repository

# Part 10 --- Version Control Systems

> **Objective**
>
> Understand Git repositories, types of repositories, repository
> structure, creating repositories, cloning repositories, managing
> repositories, and how repositories are used in professional software
> development.

------------------------------------------------------------------------

# Introduction

A Git repository is the foundation of Git-based development.

It stores:

-   Source code
-   Project history
-   Commits
-   Branches
-   Tags
-   Configuration

``` text
Project Files

      ↓

Git Repository

      ↓

Version History
```

------------------------------------------------------------------------

# What is a Git Repository?

A **Git Repository** is a storage location where Git tracks files,
changes, and project history.

A repository contains:

-   Working files
-   Git metadata
-   Commit history
-   Branch information

------------------------------------------------------------------------

# Types of Git Repositories

Git repositories are mainly:

``` text
Local Repository

        +

Remote Repository
```

------------------------------------------------------------------------

# 1. Local Repository

A repository stored on a developer's computer.

Example:

    Developer Laptop

            ↓

    Local Git Repository

Used for:

-   Creating commits
-   Managing branches
-   Viewing history

------------------------------------------------------------------------

# 2. Remote Repository

A repository hosted on a server.

Examples:

-   GitHub
-   GitLab
-   Bitbucket

Used for:

-   Team collaboration
-   Code sharing
-   Backup

------------------------------------------------------------------------

# Local vs Remote Repository

  Local Repository              Remote Repository
  ----------------------------- ------------------------------
  Stored on developer machine   Stored on server
  Used for personal changes     Used for collaboration
  Works offline                 Requires network for syncing

------------------------------------------------------------------------

# Repository Structure

A Git repository contains:

``` text
Project

 |

 ├── Source Files

 ├── .git/

 ├── Branches

 ├── Commits

 └── Tags
```

------------------------------------------------------------------------

# The .git Directory

When Git initializes a repository:

``` bash
git init
```

Git creates:

    .git/

This folder contains Git information.

Structure:

    .git

    ├── objects

    ├── refs

    ├── HEAD

    ├── index

    └── config

------------------------------------------------------------------------

# Creating a Git Repository

## Method 1: Initialize New Repository

Command:

``` bash
git init
```

Example:

    New Project Folder

            ↓

    git init

            ↓

    Git Repository Created

------------------------------------------------------------------------

# Method 2: Clone Existing Repository

Command:

``` bash
git clone URL
```

Example:

``` bash
git clone https://github.com/user/project.git
```

Creates a local copy of an existing repository.

------------------------------------------------------------------------

# Repository Initialization Workflow

``` text
Create Folder

      ↓

git init

      ↓

Add Files

      ↓

git add

      ↓

git commit
```

------------------------------------------------------------------------

# Checking Repository Information

## Check Status

Command:

``` bash
git status
```

Shows:

-   Modified files
-   Staged files
-   Untracked files

------------------------------------------------------------------------

## View Repository History

Command:

``` bash
git log
```

Displays:

-   Commit history
-   Authors
-   Messages

------------------------------------------------------------------------

# Adding Files to Repository

New files are initially:

    Untracked

Command:

``` bash
git add filename
```

Moves files to:

    Staging Area

------------------------------------------------------------------------

# Committing Changes

Command:

``` bash
git commit -m "message"
```

Creates a permanent snapshot.

Example:

``` bash
git commit -m "Added user authentication"
```

------------------------------------------------------------------------

# Connecting Local Repository to Remote

Command:

``` bash
git remote add origin URL
```

Example:

``` bash
git remote add origin https://github.com/user/project.git
```

------------------------------------------------------------------------

# Uploading Changes

Command:

``` bash
git push
```

Uploads local commits to remote repository.

Workflow:

``` text
Local Repository

        ↓

git push

        ↓

Remote Repository
```

------------------------------------------------------------------------

# Downloading Changes

Command:

``` bash
git pull
```

Downloads and integrates changes from remote repository.

------------------------------------------------------------------------

# Repository Branches

Repositories support multiple development paths.

Example:

    main

     |

    feature-login

     |

    feature-payment

Branches allow:

-   Parallel development
-   Feature isolation
-   Safer changes

------------------------------------------------------------------------

# Repository Tags

Tags mark important versions.

Example:

    v1.0

    v2.0

    release-2026

Used for:

-   Software releases
-   Version tracking

------------------------------------------------------------------------

# Repository Workflow in Industry

Example:

    Developer

     ↓

    Local Repository

     ↓

    Commit Changes

     ↓

    Push

     ↓

    Remote Repository

     ↓

    Code Review

     ↓

    Production Release

------------------------------------------------------------------------

# Repository Management Best Practices

-   Keep repository organized
-   Use meaningful commit messages
-   Maintain clean branches
-   Avoid storing sensitive information
-   Use `.gitignore`
-   Regularly synchronize with remote repository

------------------------------------------------------------------------

# .gitignore

`.gitignore` specifies files Git should ignore.

Examples:

    node_modules/

    .env

    build/

Used to avoid committing:

-   Temporary files
-   Secrets
-   Generated files

------------------------------------------------------------------------

# Common Repository Problems

## Problem 1

Accidentally committing unnecessary files.

Solution:

Use `.gitignore`.

------------------------------------------------------------------------

## Problem 2

Large repository size.

Solution:

Remove unnecessary files and use proper storage practices.

------------------------------------------------------------------------

## Problem 3

Merge conflicts.

Solution:

Pull latest changes and coordinate with team.

------------------------------------------------------------------------

# Interview Questions

1.  What is a Git repository?
2.  Difference between local and remote repository?
3.  What happens after git init?
4.  Explain the .git folder.
5.  Difference between git clone and git init?
6.  What is .gitignore?
7.  How do you connect local repository to remote?
8.  Explain repository workflow.

------------------------------------------------------------------------

# Cheat Sheet

``` text
Git Repository

Create

 ↓

Initialize

 ↓

Add Files

 ↓

Commit

 ↓

Branch

 ↓

Push

 ↓

Collaborate
```

------------------------------------------------------------------------

# Summary

A Git repository stores source code, history, commits, branches, and
metadata required for version control. Understanding repositories is
essential for using Git effectively because every Git operation happens
within the context of a repository.
