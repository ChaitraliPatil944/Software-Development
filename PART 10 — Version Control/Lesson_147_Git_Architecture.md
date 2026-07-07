# Lesson 147 --- Git Architecture

# Part 10 --- Version Control Systems

> **Objective**
>
> Understand the internal architecture of Git, how Git stores data, the
> `.git` directory structure, Git objects, SHA-1 hashing, commits, and
> how Git maintains complete version history efficiently.

------------------------------------------------------------------------

# Introduction

Most developers use Git commands daily:

``` bash
git add

git commit

git push
```

But internally Git performs many operations to store and manage
versions.

Understanding Git architecture helps developers:

-   Debug Git problems
-   Understand commits
-   Work efficiently with branches
-   Use advanced Git features

``` text
Git Command

      ↓

Git Internal System

      ↓

Objects + References

      ↓

Version History
```

------------------------------------------------------------------------

# What is Git Architecture?

**Git Architecture** describes how Git internally stores, manages, and
tracks changes in a repository.

Git follows a:

    Distributed + Object Based Architecture

------------------------------------------------------------------------

# Git Architecture Overview

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

# Git Internal Components

Git mainly contains:

``` text
Repository

 |

--------------------

Objects

References

Index

Configuration
```

------------------------------------------------------------------------

# 1. Git Repository

A Git repository stores:

-   Project files
-   Change history
-   Metadata
-   Git objects

The repository is stored inside:

    .git

directory.

------------------------------------------------------------------------

# .git Directory

When running:

``` bash
git init
```

Git creates:

    .git/

    ├── objects/

    ├── refs/

    ├── HEAD

    ├── index

    ├── config

------------------------------------------------------------------------

# Important .git Files

## objects/

Stores Git objects.

Contains:

-   Commits
-   Trees
-   Blobs

------------------------------------------------------------------------

## refs/

Stores references to commits.

Examples:

-   Branch references
-   Tags

------------------------------------------------------------------------

## HEAD

Points to the current branch.

Example:

    HEAD

     ↓

    main branch

     ↓

    Latest commit

------------------------------------------------------------------------

## index

Represents the staging area.

It stores information about changes prepared for commit.

------------------------------------------------------------------------

## config

Stores repository configuration.

Example:

-   User settings
-   Repository options

------------------------------------------------------------------------

# Git Object Model

Git stores everything as objects.

Main objects:

``` text
Blob

Tree

Commit

Tag
```

------------------------------------------------------------------------

# 1. Blob Object

A blob stores file content.

Example:

    login.java

           ↓

    Blob Object

Important:

Blob stores content, not filename.

------------------------------------------------------------------------

# 2. Tree Object

A tree stores directory structure.

It connects:

-   Files
-   Folders
-   Blob objects

Example:

    Project Tree

     |

     |-- login.java

     |-- user.java

------------------------------------------------------------------------

# 3. Commit Object

A commit stores information about a snapshot.

Contains:

-   Author
-   Date
-   Message
-   Parent commit
-   Tree reference

Example:

    Commit

     |

     |-- Author

     |-- Message

     |-- Tree

     |-- Parent

------------------------------------------------------------------------

# 4. Tag Object

A tag points to a specific commit.

Used for:

-   Releases
-   Versions

Example:

    v1.0

     ↓

    Commit

------------------------------------------------------------------------

# Git Object Relationship

``` text
Commit

   ↓

Tree

   ↓

Blob

   ↓

File Content
```

------------------------------------------------------------------------

# SHA-1 Hashing

Git identifies objects using SHA-1 hashes.

Example:

    a84b9f2c8d7e...

Each object gets a unique identifier.

------------------------------------------------------------------------

# Why Does Git Use Hashing?

Hashing provides:

## Data Integrity

Changes create different hashes.

## Fast Lookup

Objects can be found quickly.

## Duplicate Detection

Same content creates same hash.

------------------------------------------------------------------------

# Git Commit Internally

When a developer runs:

``` bash
git commit -m "Added login"
```

Git performs:

``` text
Files

 ↓

Create Blob Objects

 ↓

Create Tree Object

 ↓

Create Commit Object

 ↓

Update Branch Reference
```

------------------------------------------------------------------------

# Example Commit History

    Commit C3

     |

    Commit C2

     |

    Commit C1

     |

    Initial Commit

Each commit points to the previous commit.

------------------------------------------------------------------------

# Branch Internals

A branch is simply a reference to a commit.

Example:

    main

     ↓

    Commit C3

Creating a branch:

    feature

     ↓

    Commit C3

Both point to the same history initially.

------------------------------------------------------------------------

# Git Index (Staging Area)

The index stores changes ready for commit.

Workflow:

``` text
Working Directory

        ↓

git add

        ↓

Index

        ↓

git commit

        ↓

Repository
```

------------------------------------------------------------------------

# Git Data Storage

Git uses:

## Content Addressable Storage

Data is stored based on its hash.

Example:

    File Content

          ↓

    SHA Hash

          ↓

    Object Storage

------------------------------------------------------------------------

# Snapshot Model

Git stores snapshots, not differences.

Example:

Version 1:

    File A

    File B

Version 2:

    File A Changed

    File B

Git stores references efficiently.

------------------------------------------------------------------------

# Git vs Traditional Version Control Storage

  Traditional VCS           Git
  ------------------------- ------------------
  Stores file differences   Stores snapshots
  Centralized               Distributed
  Slower branching          Fast branching

------------------------------------------------------------------------

# Remote Repository Architecture

Example:

    Local Repository

            |

            |

    Remote Repository

    (GitHub)

Commands:

Upload:

``` bash
git push
```

Download:

``` bash
git pull
```

------------------------------------------------------------------------

# Industry Example

## Software Development Team

Developer creates commit:

    Code Changes

          ↓

    Blob Objects

          ↓

    Tree

          ↓

    Commit

          ↓

    Branch

          ↓

    Remote Repository

------------------------------------------------------------------------

# Advantages of Git Architecture

-   Fast operations
-   Complete history
-   Data integrity
-   Offline development
-   Efficient branching
-   Easy collaboration

------------------------------------------------------------------------

# Common Mistakes

## Mistake 1

Editing `.git` manually.

Solution:

Use Git commands.

------------------------------------------------------------------------

## Mistake 2

Deleting `.git` folder accidentally.

Solution:

Maintain backups.

------------------------------------------------------------------------

## Mistake 3

Not understanding staged changes.

Solution:

Use:

``` bash
git status
```

regularly.

------------------------------------------------------------------------

# Interview Questions

1.  Explain Git architecture.
2.  What is stored inside `.git`?
3.  Explain Git objects.
4.  What is a blob?
5.  What is a tree object?
6.  Explain commit objects.
7.  Why does Git use SHA-1?
8.  Difference between snapshot and delta storage?
9.  What is HEAD in Git?

------------------------------------------------------------------------

# Cheat Sheet

``` text
Git Architecture

Files

 ↓

Blob

 ↓

Tree

 ↓

Commit

 ↓

Branch Reference

 ↓

Repository
```

------------------------------------------------------------------------

# Summary

Git architecture is based on an object storage model where files are
stored as blobs, directories as trees, and changes as commits. Through
hashing, references, and snapshots, Git provides fast, reliable, and
distributed version control for modern software development.
