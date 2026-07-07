# Lesson 152 --- Merge Conflicts

# Part 10 --- Version Control Systems

> **Objective**
>
> Understand Git merge conflicts, why conflicts occur, how Git detects
> conflicts, conflict markers, conflict resolution methods, tools used
> for resolving conflicts, and best practices for avoiding conflicts in
> team development.

------------------------------------------------------------------------

# Introduction

Multiple developers often modify the same code at the same time.

When Git cannot automatically combine changes, a **merge conflict**
occurs.

``` text
Developer A Changes

        +

Developer B Changes

        ↓

Git Cannot Decide

        ↓

Merge Conflict
```

------------------------------------------------------------------------

# What is a Merge Conflict?

A **Merge Conflict** occurs when Git cannot automatically merge changes
from different branches because the same part of a file has been
modified differently.

Git requires a developer to manually decide which changes should remain.

------------------------------------------------------------------------

# Why Do Merge Conflicts Occur?

Common causes:

-   Two developers edit the same lines
-   One developer deletes a file modified by another
-   Different changes are made to the same code section
-   Long-running branches

------------------------------------------------------------------------

# Example of Conflict

Initial code:

``` java
System.out.println("Hello");
```

Developer A changes:

``` java
System.out.println("Hello User");
```

Developer B changes:

``` java
System.out.println("Hello Developer");
```

Git sees:

    Same line

    Different changes

    ↓

    Conflict

------------------------------------------------------------------------

# How Git Detects Conflicts

During merge:

``` bash
git merge branch_name
```

Git compares:

-   Common ancestor
-   Current branch changes
-   Incoming branch changes

If changes overlap:

    Merge Conflict Detected

------------------------------------------------------------------------

# Conflict Markers

Git adds markers inside the file:

``` text
<<<<<<< HEAD

Current Branch Code

=======

Incoming Branch Code

>>>>>>> feature-branch
```

Meaning:

    <<<<<<<

    Your changes


    =======

    Other branch changes


    >>>>>>>

------------------------------------------------------------------------

# Merge Conflict Resolution Process

Steps:

``` text
1. Detect Conflict

        ↓

2. Open Conflicted File

        ↓

3. Understand Changes

        ↓

4. Choose Correct Code

        ↓

5. Remove Markers

        ↓

6. Commit Resolution
```

------------------------------------------------------------------------

# Step 1: Identify Conflicts

Command:

``` bash
git status
```

Example:

    both modified:
    app.java

------------------------------------------------------------------------

# Step 2: Open File

Example:

Before resolution:

``` java
<<<<<<< HEAD

login();

=======

authenticate();

>>>>>>> feature
```

------------------------------------------------------------------------

# Step 3: Decide Final Code

Developer chooses:

``` java
login();
authenticate();
```

------------------------------------------------------------------------

# Step 4: Remove Conflict Markers

Remove:

    <<<<<<<

    =======

    >>>>>>>

Save file.

------------------------------------------------------------------------

# Step 5: Stage Resolved File

Command:

``` bash
git add filename
```

------------------------------------------------------------------------

# Step 6: Complete Merge

Command:

``` bash
git commit
```

Merge is completed.

------------------------------------------------------------------------

# Aborting Conflict Resolution

If you do not want to continue:

Command:

``` bash
git merge --abort
```

Restores previous state.

------------------------------------------------------------------------

# Types of Merge Conflicts

## 1. Content Conflict

Same lines changed differently.

Example:

    Same function modified

------------------------------------------------------------------------

## 2. File Deletion Conflict

One branch deletes a file while another modifies it.

------------------------------------------------------------------------

## 3. Rename Conflict

Different branches rename the same file.

------------------------------------------------------------------------

# Merge Conflict Example

## Team Development

Developer A:

    Updates payment calculation

Developer B:

    Updates payment calculation

Both merge:

    Conflict occurs

Resolution:

    Review both changes

    ↓

    Combine correct logic

    ↓

    Commit

------------------------------------------------------------------------

# Tools for Conflict Resolution

Developers use:

-   VS Code Merge Editor
-   IntelliJ Git Tools
-   GitKraken
-   Command line tools

------------------------------------------------------------------------

# Useful Git Commands

## Check Conflict Status

``` bash
git status
```

------------------------------------------------------------------------

## See Differences

``` bash
git diff
```

------------------------------------------------------------------------

## Abort Merge

``` bash
git merge --abort
```

------------------------------------------------------------------------

## Continue Merge

``` bash
git commit
```

------------------------------------------------------------------------

# Preventing Merge Conflicts

## 1. Pull Frequently

Keep branch updated.

``` bash
git pull
```

------------------------------------------------------------------------

## 2. Make Small Commits

Small changes are easier to merge.

------------------------------------------------------------------------

## 3. Communicate Changes

Inform teammates about major modifications.

------------------------------------------------------------------------

## 4. Avoid Long-Running Branches

Merge regularly.

------------------------------------------------------------------------

## 5. Follow Coding Standards

Consistent code reduces conflicts.

------------------------------------------------------------------------

# Merge Conflict Best Practices

-   Understand both changes
-   Do not blindly accept code
-   Test after resolution
-   Review merged code
-   Communicate with developers

------------------------------------------------------------------------

# Merge Conflict vs Merge Error

  Merge Conflict            Merge Error
  ------------------------- -----------------------------------
  Code changes overlap      Technical problem
  Requires human decision   Usually command/environment issue
  Common in teams           Less frequent

------------------------------------------------------------------------

# Interview Questions

1.  What is a merge conflict?
2.  Why do merge conflicts occur?
3.  How does Git detect conflicts?
4.  Explain conflict markers.
5.  How do you resolve conflicts?
6.  What command shows conflicts?
7.  How do you abort a merge?
8.  How can conflicts be prevented?

------------------------------------------------------------------------

# Cheat Sheet

``` text
Merge Conflict

Merge

 ↓

Conflict Detected

 ↓

Review Changes

 ↓

Resolve

 ↓

git add

 ↓

git commit

 ↓

Merge Complete
```

------------------------------------------------------------------------

# Summary

Merge conflicts occur when Git cannot automatically combine changes from
different branches. Developers must manually review, select, and
integrate the correct changes. Understanding conflict resolution is
essential for effective teamwork and maintaining stable software
projects.
