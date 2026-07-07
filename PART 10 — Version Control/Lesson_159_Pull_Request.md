# Lesson 159 --- Pull Request

# Part 10 --- Version Control Systems

> **Objective**
>
> Understand Pull Requests, why they are used, PR lifecycle, creating
> pull requests, review process, approval workflow, merge strategies,
> best practices, and how professional teams use pull requests for
> collaboration.

------------------------------------------------------------------------

# Introduction

In professional software development, developers do not directly add
every change to the main codebase.

Changes are reviewed before becoming part of the final product.

Pull Requests provide this review mechanism.

``` text
Developer Branch

        ↓

Pull Request

        ↓

Code Review

        ↓

Approval

        ↓

Merge
```

------------------------------------------------------------------------

# What is a Pull Request?

A **Pull Request (PR)** is a request to merge changes from one branch
into another branch.

It allows team members to:

-   Review code
-   Discuss changes
-   Run tests
-   Approve modifications
-   Merge safely

------------------------------------------------------------------------

# Why Do We Need Pull Requests?

Without pull requests:

``` text
Developer Code

      ↓

Direct Merge

      ↓

Possible Bugs
```

Pull Requests provide:

-   Code quality checks
-   Team collaboration
-   Discussion
-   Documentation of changes
-   Safer releases

------------------------------------------------------------------------

# Pull Request Components

A Pull Request contains:

## 1. Source Branch

The branch containing changes.

Example:

    feature-login

------------------------------------------------------------------------

## 2. Target Branch

The branch receiving changes.

Example:

    main

------------------------------------------------------------------------

## 3. Description

Explains:

-   What changed
-   Why it changed
-   How it was tested

------------------------------------------------------------------------

## 4. Review Comments

Team members provide feedback.

------------------------------------------------------------------------

## 5. Checks

Automated systems verify:

-   Tests
-   Build
-   Code quality

------------------------------------------------------------------------

# Pull Request Lifecycle

``` text
Create Branch

      ↓

Develop Feature

      ↓

Push Branch

      ↓

Create Pull Request

      ↓

Code Review

      ↓

Approval

      ↓

Merge

      ↓

Delete Branch
```

------------------------------------------------------------------------

# Creating a Pull Request

Steps:

## Step 1

Push branch:

``` bash
git push origin feature-login
```

------------------------------------------------------------------------

## Step 2

Open repository platform.

Example:

GitHub.

------------------------------------------------------------------------

## Step 3

Create Pull Request.

Select:

    Source:

    feature-login


    Target:

    main

------------------------------------------------------------------------

## Step 4

Add:

-   Title
-   Description
-   Reviewers

------------------------------------------------------------------------

# Pull Request Review Process

``` text
Developer Creates PR

        ↓

Reviewer Checks Code

        ↓

Comments Added

        ↓

Developer Updates Code

        ↓

Approval

        ↓

Merge
```

------------------------------------------------------------------------

# Types of Review Feedback

## Comment

Suggestion or question.

------------------------------------------------------------------------

## Change Request

Reviewer asks for modifications.

------------------------------------------------------------------------

## Approval

Reviewer accepts changes.

------------------------------------------------------------------------

# Code Review in Pull Requests

Reviewers check:

## Code Quality

-   Clean code
-   Readability
-   Maintainability

------------------------------------------------------------------------

## Functionality

-   Correct behavior
-   Requirement satisfaction

------------------------------------------------------------------------

## Security

-   Vulnerabilities
-   Sensitive information

------------------------------------------------------------------------

## Performance

-   Efficiency
-   Resource usage

------------------------------------------------------------------------

# Pull Request Checks

Automated checks may include:

-   Unit tests
-   Integration tests
-   Build verification
-   Code formatting
-   Security scans

Example:

``` text
Pull Request

        ↓

CI Pipeline

        ↓

Tests Pass

        ↓

Ready to Merge
```

------------------------------------------------------------------------

# Pull Request Merge Strategies

## 1. Merge Commit

Creates a merge commit.

History:

    A---B---C

         \

          D

           \

            Merge

------------------------------------------------------------------------

## 2. Squash Merge

Combines all commits into one.

Before:

    Commit 1

    Commit 2

    Commit 3

After:

    Single Commit

------------------------------------------------------------------------

## 3. Rebase Merge

Creates linear history.

Example:

    A---B---C---D

------------------------------------------------------------------------

# Pull Request vs Merge

  Pull Request          Merge
  --------------------- -------------------
  Review process        Git operation
  Platform feature      Command operation
  Includes discussion   Combines code

------------------------------------------------------------------------

# Pull Request Best Practices

## Write Clear Titles

Bad:

    Update code

Good:

    Add user authentication API

------------------------------------------------------------------------

## Explain Changes

Include:

-   Purpose
-   Implementation details
-   Testing information

------------------------------------------------------------------------

## Keep PRs Small

Small PRs:

-   Review faster
-   Reduce conflicts
-   Improve quality

------------------------------------------------------------------------

## Respond to Feedback

Address review comments professionally.

------------------------------------------------------------------------

# Pull Request Example

## E-Commerce Application

Developer creates:

    feature-payment

Changes:

-   Payment API
-   Validation logic

Workflow:

    Push Branch

          ↓

    Create PR

          ↓

    Review

          ↓

    Tests Pass

          ↓

    Merge to Main

------------------------------------------------------------------------

# Common Pull Request Mistakes

## Mistake 1

Huge pull requests.

Solution:

Create smaller focused PRs.

------------------------------------------------------------------------

## Mistake 2

No description.

Solution:

Explain purpose and testing.

------------------------------------------------------------------------

## Mistake 3

Ignoring review comments.

Solution:

Discuss and update changes.

------------------------------------------------------------------------

# Pull Request in Open Source

Open-source workflow:

``` text
Fork Repository

        ↓

Create Branch

        ↓

Make Changes

        ↓

Create Pull Request

        ↓

Maintainer Review

        ↓

Merge
```

------------------------------------------------------------------------

# Interview Questions

1.  What is a Pull Request?
2.  Why are pull requests used?
3.  Explain PR lifecycle.
4.  Difference between pull request and merge?
5.  What happens during code review?
6.  Explain PR merge strategies.
7.  Why should PRs be small?
8.  What checks run on a PR?

------------------------------------------------------------------------

# Cheat Sheet

``` text
Pull Request

Create Branch

      ↓

Code Changes

      ↓

Push Branch

      ↓

Create PR

      ↓

Review

      ↓

Approve

      ↓

Merge
```

------------------------------------------------------------------------

# Summary

Pull Requests are an essential collaboration mechanism in modern
software development. They allow teams to review code, discuss
improvements, run automated checks, and safely merge changes into the
main codebase while maintaining software quality.
