# Lesson 162 --- Git & Version Control Interview Questions

# Part 10 --- Version Control Systems

> **Objective**
>
> Prepare for Git and Version Control interviews by understanding
> frequently asked questions about Git basics, architecture,
> repositories, commits, branches, merging, conflicts, rebase,
> cherry-pick, stash, tags, GitHub workflow, pull requests, and
> professional Git practices.

------------------------------------------------------------------------

# Section 1 --- Git Fundamentals

## Q1. What is Git?

**Answer:**

Git is a distributed version control system used to track changes in
source code and manage software development.

It allows developers to:

-   Track changes
-   Create versions
-   Collaborate
-   Manage branches

------------------------------------------------------------------------

## Q2. Why was Git created?

Git was created by Linus Torvalds in 2005 for managing Linux kernel
development.

It was designed for:

-   Speed
-   Distributed development
-   Reliable version tracking

------------------------------------------------------------------------

## Q3. Difference between Git and GitHub?

  Git                      GitHub
  ------------------------ -----------------------
  Version control system   Hosting platform
  Runs locally             Cloud-based
  Tracks changes           Enables collaboration

------------------------------------------------------------------------

## Q4. What are the advantages of Git?

Advantages:

-   Distributed architecture
-   Fast operations
-   Branching support
-   Offline capability
-   Complete history

------------------------------------------------------------------------

# Section 2 --- Git Architecture Questions

## Q5. Explain Git architecture.

Git has:

    Working Directory

            ↓

    Staging Area

            ↓

    Local Repository

            ↓

    Remote Repository

------------------------------------------------------------------------

## Q6. What is the .git folder?

`.git` stores Git metadata.

Contains:

-   Objects
-   References
-   HEAD
-   Index
-   Configuration

------------------------------------------------------------------------

## Q7. Explain Git objects.

Git uses four main objects:

### Blob

Stores file content.

### Tree

Stores directory structure.

### Commit

Stores snapshots.

### Tag

Marks important commits.

------------------------------------------------------------------------

## Q8. Why does Git use hashing?

Hashing provides:

-   Data integrity
-   Unique identification
-   Fast lookup

------------------------------------------------------------------------

# Section 3 --- Repository Questions

## Q9. What is a Git repository?

A Git repository stores:

-   Source code
-   History
-   Commits
-   Branches

------------------------------------------------------------------------

## Q10. Difference between local and remote repository?

  Local               Remote
  ------------------- --------------------
  Developer machine   Server
  Personal work       Team collaboration
  Offline             Shared

------------------------------------------------------------------------

## Q11. What does git init do?

Creates a new Git repository.

Command:

``` bash
git init
```

------------------------------------------------------------------------

## Q12. What does git clone do?

Creates a local copy of an existing repository.

Command:

``` bash
git clone URL
```

------------------------------------------------------------------------

# Section 4 --- Commit Questions

## Q13. What is a Git commit?

A commit is a snapshot of staged changes stored in Git history.

------------------------------------------------------------------------

## Q14. Explain commit lifecycle.

    Modify

     ↓

    git add

     ↓

    Staging

     ↓

    git commit

     ↓

    Repository

------------------------------------------------------------------------

## Q15. What is an atomic commit?

A commit containing one logical change.

Example:

    Add login API

------------------------------------------------------------------------

## Q16. What makes a good commit message?

A good message:

-   Is clear
-   Explains change
-   Uses action words

Example:

    Fix payment validation issue

------------------------------------------------------------------------

# Section 5 --- Branch Questions

## Q17. What is a Git branch?

A branch is a separate development path.

It allows independent work.

------------------------------------------------------------------------

## Q18. Why are branches used?

Branches help:

-   Develop features
-   Fix bugs
-   Experiment safely

------------------------------------------------------------------------

## Q19. How do you create a branch?

Command:

``` bash
git branch branch_name
```

or:

``` bash
git checkout -b branch_name
```

------------------------------------------------------------------------

## Q20. Difference between main and feature branch?

  Main          Feature
  ------------- -----------------
  Stable code   New development
  Production    Temporary work

------------------------------------------------------------------------

# Section 6 --- Merge Questions

## Q21. What is Git Merge?

Merge combines changes from one branch into another.

Command:

``` bash
git merge branch_name
```

------------------------------------------------------------------------

## Q22. Explain fast-forward merge.

Occurs when target branch has no new commits.

Git simply moves the branch pointer.

------------------------------------------------------------------------

## Q23. What is three-way merge?

A merge where both branches have new commits.

Git creates a merge commit.

------------------------------------------------------------------------

# Section 7 --- Merge Conflict Questions

## Q24. What is a merge conflict?

A conflict occurs when Git cannot automatically combine changes.

------------------------------------------------------------------------

## Q25. Why do conflicts occur?

Reasons:

-   Same lines modified
-   File deleted in one branch
-   Long-running branches

------------------------------------------------------------------------

## Q26. How do you resolve conflicts?

Steps:

    Identify Conflict

    ↓

    Edit Files

    ↓

    Remove Markers

    ↓

    git add

    ↓

    git commit

------------------------------------------------------------------------

# Section 8 --- Rebase Questions

## Q27. What is Git Rebase?

Rebase moves commits onto another branch to create cleaner history.

Command:

``` bash
git rebase main
```

------------------------------------------------------------------------

## Q28. Difference between merge and rebase?

  Merge                  Rebase
  ---------------------- ------------------
  Creates merge commit   Rewrites history
  Safer                  Cleaner history

------------------------------------------------------------------------

## Q29. What is interactive rebase?

Allows editing commits.

Command:

``` bash
git rebase -i
```

Operations:

-   Pick
-   Squash
-   Reword
-   Drop

------------------------------------------------------------------------

# Section 9 --- Cherry Pick Questions

## Q30. What is cherry-pick?

Applies a specific commit from one branch to another.

Command:

``` bash
git cherry-pick commit_id
```

------------------------------------------------------------------------

## Q31. When is cherry-pick used?

Used for:

-   Hotfixes
-   Backporting
-   Selective changes

------------------------------------------------------------------------

# Section 10 --- Stash Questions

## Q32. What is Git Stash?

Temporarily stores unfinished changes.

Command:

``` bash
git stash
```

------------------------------------------------------------------------

## Q33. Difference between stash apply and stash pop?

  Apply              Pop
  ------------------ ----------------------------
  Restores changes   Restores and removes stash

------------------------------------------------------------------------

# Section 11 --- Tag Questions

## Q34. What is Git Tag?

A tag marks an important commit.

Example:

    v1.0.0

------------------------------------------------------------------------

## Q35. Difference between tag and branch?

  Tag               Branch
  ----------------- ------------------
  Fixed reference   Moving reference
  Release marking   Development

------------------------------------------------------------------------

# Section 12 --- Remote Repository Questions

## Q36. What is a remote repository?

A repository hosted on a server for collaboration.

------------------------------------------------------------------------

## Q37. Explain git push and git pull.

Push:

    Local → Remote

Pull:

    Remote → Local

------------------------------------------------------------------------

## Q38. Difference between fetch and pull?

  Fetch            Pull
  ---------------- --------------------
  Downloads only   Downloads + merges

------------------------------------------------------------------------

# Section 13 --- GitHub Workflow Questions

## Q39. What is GitHub workflow?

A process:

    Clone

    ↓

    Branch

    ↓

    Commit

    ↓

    Push

    ↓

    Pull Request

    ↓

    Review

    ↓

    Merge

------------------------------------------------------------------------

## Q40. What is a Pull Request?

A request to merge changes into another branch.

------------------------------------------------------------------------

## Q41. Why is code review important?

It improves:

-   Quality
-   Security
-   Maintainability

------------------------------------------------------------------------

# Section 14 --- Scenario Based Questions

## Q42. You committed code accidentally. What will you do?

Answer:

Use:

    git revert

or:

    git reset

depending on situation.

------------------------------------------------------------------------

## Q43. Your push is rejected. What will you do?

Answer:

    git pull

    resolve conflicts

    push again

------------------------------------------------------------------------

## Q44. Production has a bug fix in another branch. How will you move it?

Answer:

Use:

    git cherry-pick

------------------------------------------------------------------------

## Q45. You need to switch branches but have unfinished work.

Answer:

Use:

    git stash

------------------------------------------------------------------------

# Quick Revision Table

  Concept       Command
  ------------- -----------------
  Initialize    git init
  Clone         git clone
  Status        git status
  Add           git add
  Commit        git commit
  Branch        git branch
  Merge         git merge
  Rebase        git rebase
  Cherry Pick   git cherry-pick
  Stash         git stash
  Push          git push
  Pull          git pull

------------------------------------------------------------------------

# Interview Tips

For Git questions:

1.  Explain concept
2.  Give command
3.  Provide real-world example

Example:

"Git branch creates an independent development path. Teams use feature
branches to develop features safely before merging into main."

------------------------------------------------------------------------

# Summary

Git and Version Control System interviews focus on understanding
concepts, commands, workflows, and real-world collaboration practices. A
strong developer should understand not only Git commands but also why
and when each operation is used.
