# Lesson 146 --- Git Basics

# Part 10 --- Version Control Systems

> **Objective**
>
> Understand Git fundamentals, why Git was created, how Git works, basic
> Git terminology, essential commands, workflow, and how developers use
> Git in real-world software development.

------------------------------------------------------------------------

# Introduction

Modern software development involves many developers changing the same
codebase.

Git helps developers:

-   Track changes
-   Collaborate
-   Manage versions
-   Recover previous code
-   Work on features independently

``` text
Developer

      ↓

Git

      ↓

Version History

      ↓

Collaboration
```

------------------------------------------------------------------------

# What is Git?

**Git** is a distributed version control system used to track changes in
source code and manage software development.

Git allows developers to:

-   Save versions of code
-   Create branches
-   Merge changes
-   Collaborate with teams

------------------------------------------------------------------------

# History of Git

Git was created by:

**Linus Torvalds**

in 2005.

Reason:

The Linux kernel project needed a fast and reliable version control
system.

Git was designed to provide:

-   Speed
-   Distributed architecture
-   Strong branching
-   Data integrity

------------------------------------------------------------------------

# Why Was Git Created?

Before Git, many teams used centralized systems.

Problems:

-   Slow operations
-   Dependency on central server
-   Limited offline work

Git solved these problems using a distributed approach.

------------------------------------------------------------------------

# Git vs Version Control System

Git is a type of Version Control System.

    Version Control System

            |

    ------------------

    Git

    SVN

    Mercurial

------------------------------------------------------------------------

# Why is Git Popular?

Git provides:

## 1. Distributed Architecture

Every developer has a complete repository.

    Developer A

    Repository Copy


    Developer B

    Repository Copy

------------------------------------------------------------------------

## 2. Fast Performance

Most operations happen locally.

------------------------------------------------------------------------

## 3. Powerful Branching

Creating branches is quick and easy.

Example:

    Main Branch

          |

    Feature Branch

------------------------------------------------------------------------

## 4. Offline Capability

Developers can commit changes without internet access.

------------------------------------------------------------------------

# Git Architecture

Git has three main areas:

``` text
Working Directory

        ↓

Staging Area

        ↓

Local Repository

        ↓

Remote Repository
```

------------------------------------------------------------------------

# 1. Working Directory

The folder where developers edit files.

Example:

    project/

     ├── app.java

     ├── index.html

     └── database.sql

------------------------------------------------------------------------

# 2. Staging Area

A temporary area where changes are prepared before committing.

Command:

``` bash
git add
```

------------------------------------------------------------------------

# 3. Local Repository

Stores committed changes on the developer's machine.

Command:

``` bash
git commit
```

------------------------------------------------------------------------

# 4. Remote Repository

A repository hosted online.

Examples:

-   GitHub
-   GitLab
-   Bitbucket

Command:

``` bash
git push
```

------------------------------------------------------------------------

# Git Workflow

Basic Git workflow:

``` text
Create/Edit Files

        ↓

Add Changes

        ↓

Commit Changes

        ↓

Push Changes

        ↓

Share With Team
```

------------------------------------------------------------------------

# Installing Git

After installation, verify Git:

``` bash
git --version
```

Example output:

    git version 2.x.x

------------------------------------------------------------------------

# Creating a Git Repository

## Initialize Repository

Command:

``` bash
git init
```

Creates a new Git repository.

Example:

    Project Folder

            ↓

    git init

            ↓

    .git folder created

------------------------------------------------------------------------

# Cloning a Repository

Command:

``` bash
git clone repository_url
```

Creates a local copy of an existing repository.

Example:

``` bash
git clone https://example.com/project.git
```

------------------------------------------------------------------------

# Checking Repository Status

Command:

``` bash
git status
```

Shows:

-   Modified files
-   Staged files
-   Untracked files

------------------------------------------------------------------------

# Adding Changes

Command:

``` bash
git add filename
```

or:

``` bash
git add .
```

Adds changes to staging area.

------------------------------------------------------------------------

# Creating a Commit

Command:

``` bash
git commit -m "message"
```

Creates a snapshot of changes.

Example:

``` bash
git commit -m "Added login feature"
```

------------------------------------------------------------------------

# Viewing History

Command:

``` bash
git log
```

Shows:

-   Commit ID
-   Author
-   Date
-   Commit message

------------------------------------------------------------------------

# Comparing Changes

Command:

``` bash
git diff
```

Shows differences between versions.

------------------------------------------------------------------------

# Git File States

A file can have different states:

``` text
Untracked

      ↓

Modified

      ↓

Staged

      ↓

Committed
```

------------------------------------------------------------------------

# Git Example Workflow

Scenario:

Adding login functionality.

Step 1:

Modify code.

    login.java

Step 2:

Check status.

``` bash
git status
```

Step 3:

Stage changes.

``` bash
git add login.java
```

Step 4:

Commit.

``` bash
git commit -m "Added login feature"
```

------------------------------------------------------------------------

# Common Git Commands

  Command      Purpose
  ------------ -------------------
  git init     Create repository
  git clone    Copy repository
  git status   Check changes
  git add      Stage changes
  git commit   Save changes
  git log      View history
  git diff     Compare changes
  git push     Upload changes
  git pull     Download updates

------------------------------------------------------------------------

# Git in Industry

Software teams use Git for:

-   Application development
-   Open-source projects
-   Team collaboration
-   CI/CD pipelines
-   Release management

Example:

    Developer

    ↓

    Git Repository

    ↓

    Code Review

    ↓

    Production Release

------------------------------------------------------------------------

# Common Git Mistakes

## Mistake 1

Large commits.

Solution:

Make small meaningful commits.

------------------------------------------------------------------------

## Mistake 2

Poor commit messages.

Bad:

    update

Good:

    Fix payment validation issue

------------------------------------------------------------------------

## Mistake 3

Committing unnecessary files.

Solution:

Use `.gitignore`.

------------------------------------------------------------------------

# Git Best Practices

-   Commit frequently
-   Write meaningful messages
-   Pull before pushing
-   Use branches for features
-   Review changes before commit
-   Keep commits focused

------------------------------------------------------------------------

# Interview Questions

1.  What is Git?
2.  Why was Git created?
3.  Difference between Git and VCS?
4.  Explain Git architecture.
5.  What is staging area?
6.  Difference between git add and git commit?
7.  What does git clone do?
8.  Explain Git workflow.

------------------------------------------------------------------------

# Cheat Sheet

``` text
Git Workflow

Working Directory

        ↓

git add

        ↓

Staging Area

        ↓

git commit

        ↓

Local Repository

        ↓

git push

        ↓

Remote Repository
```

------------------------------------------------------------------------

# Summary

Git is a distributed version control system that enables developers to
manage code changes, collaborate efficiently, and maintain software
history. Understanding Git basics is essential for every modern software
developer because almost every professional development environment
depends on version control.
