# Lesson 192 --- Versioning

# Part 12 --- Software Maintenance

> **Objective**
>
> Understand software versioning, why versioning is required, version
> numbering schemes, Semantic Versioning (SemVer), major/minor/patch
> releases, release versions, relationship with version control, best
> practices, and interview concepts.

------------------------------------------------------------------------

# Introduction

Software changes continuously.

Developers release:

-   New features
-   Bug fixes
-   Security updates
-   Performance improvements

To identify and manage different software states, we use **Versioning**.

``` text
Software Update

      ↓

New Version Number

      ↓

Track Changes
```

------------------------------------------------------------------------

# What is Software Versioning?

**Software Versioning** is the process of assigning unique identifiers
to different releases or states of software.

Simple definition:

    Versioning = Tracking Software Changes Through Versions

------------------------------------------------------------------------

# Why is Versioning Needed?

Versioning helps with:

-   Identifying releases
-   Tracking changes
-   Managing updates
-   Supporting rollback
-   Maintaining compatibility

Without versioning:

    Multiple Changes

          ↓

    Confusion

          ↓

    Difficult Maintenance

------------------------------------------------------------------------

# Real-World Example

Consider a mobile application:

    Version 1.0

          ↓

    Version 1.1

          ↓

    Version 2.0

Each version represents a different software state.

------------------------------------------------------------------------

# Version Number Structure

Common format:

    MAJOR.MINOR.PATCH

Example:

    3.5.2

Meaning:

    3 = Major Version

    5 = Minor Version

    2 = Patch Version

------------------------------------------------------------------------

# Semantic Versioning (SemVer)

**Semantic Versioning** is a standard approach for version numbering.

Format:

    MAJOR.MINOR.PATCH

Example:

    2.4.1

------------------------------------------------------------------------

# 1. Major Version

Major version changes indicate breaking changes.

Example:

    1.0.0

          ↓

    2.0.0

Meaning:

-   Major functionality changes
-   Existing users may need modifications

Example:

API changes:

Before:

    /user

After:

    /customers

------------------------------------------------------------------------

# 2. Minor Version

Minor version adds new features without breaking existing functionality.

Example:

    2.1.0

Changes:

-   New features
-   Improvements
-   Additional capabilities

------------------------------------------------------------------------

# 3. Patch Version

Patch versions fix bugs.

Example:

    2.1.3

Changes:

-   Bug fixes
-   Security fixes
-   Small improvements

------------------------------------------------------------------------

# Major vs Minor vs Patch

  Version Type   Purpose            Example
  -------------- ------------------ ---------
  Major          Breaking changes   3.0.0
  Minor          New features       3.1.0
  Patch          Bug fixes          3.1.1

------------------------------------------------------------------------

# Types of Software Versions

## 1. Development Version

Used during development.

Example:

    0.x.x

------------------------------------------------------------------------

## 2. Alpha Version

Early testing version.

Characteristics:

-   Incomplete features
-   Internal testing

------------------------------------------------------------------------

## 3. Beta Version

Released for wider testing.

Characteristics:

-   More stable
-   User feedback collected

------------------------------------------------------------------------

## 4. Release Candidate (RC)

Almost final version.

Example:

    2.0.0-RC1

------------------------------------------------------------------------

## 5. Stable Release

Official production version.

Example:

    2.0.0

------------------------------------------------------------------------

# Versioning and Software Maintenance

Versioning supports maintenance activities.

## Corrective Maintenance

Example:

    1.0.1

    Bug Fix Release

------------------------------------------------------------------------

## Adaptive Maintenance

Example:

    2.0.0

    Platform Update

------------------------------------------------------------------------

## Perfective Maintenance

Example:

    1.5.0

    New Feature Added

------------------------------------------------------------------------

## Preventive Maintenance

Example:

    1.5.1

    Security Improvement

------------------------------------------------------------------------

# Version Control vs Versioning

  Version Control       Versioning
  --------------------- ------------------------------
  Tracks code changes   Identifies software releases
  Uses Git commits      Uses release numbers
  Developer focused     User/release focused

Example:

Git:

    commit abc123

Software:

    Version 2.0.1

------------------------------------------------------------------------

# Versioning in Git

Git supports version management through:

-   Tags
-   Branches
-   Commits

Example:

Create tag:

``` bash
git tag v1.0.0
```

View tags:

``` bash
git tag
```

------------------------------------------------------------------------

# Release Versioning

A release version represents a published software update.

Example:

    Application v5.2.0

Release notes include:

-   New features
-   Bug fixes
-   Breaking changes

------------------------------------------------------------------------

# Best Practices

## 1. Follow Semantic Versioning

Use clear version rules.

------------------------------------------------------------------------

## 2. Maintain Release Notes

Document changes.

------------------------------------------------------------------------

## 3. Avoid Random Version Numbers

Keep versions meaningful.

------------------------------------------------------------------------

## 4. Tag Releases

Use version tags in repositories.

------------------------------------------------------------------------

## 5. Communicate Breaking Changes

Inform users before major updates.

------------------------------------------------------------------------

# Common Versioning Problems

## Problem 1

Unclear version numbers.

Solution:

Use standard conventions.

------------------------------------------------------------------------

## Problem 2

Breaking changes without warning.

Solution:

Use major version updates.

------------------------------------------------------------------------

## Problem 3

Missing release documentation.

Solution:

Maintain release notes.

------------------------------------------------------------------------

# Real-World Example

## API Development

Version 1:

    /api/v1/users

New design:

    /api/v2/users

Benefits:

-   Existing applications continue working
-   New clients use updated API

------------------------------------------------------------------------

# Interview Questions

## 1. What is software versioning?

Software versioning is assigning identifiers to different software
releases.

------------------------------------------------------------------------

## 2. What is Semantic Versioning?

A versioning system using:

    MAJOR.MINOR.PATCH

------------------------------------------------------------------------

## 3. What does a major version indicate?

Major versions indicate breaking changes.

------------------------------------------------------------------------

## 4. Difference between minor and patch versions?

Minor versions add features.

Patch versions fix bugs.

------------------------------------------------------------------------

## 5. Difference between version control and versioning?

Version control manages code changes.

Versioning identifies software releases.

------------------------------------------------------------------------

# Cheat Sheet

``` text
Software Versioning

Change

 ↓

Version Number

 ↓

Release

 ↓

Track Software Evolution
```

------------------------------------------------------------------------

# Summary

Software versioning provides a structured way to identify and manage
software releases. Semantic Versioning helps teams communicate the
impact of changes through major, minor, and patch numbers.

Proper versioning improves maintenance, release management,
compatibility, and software reliability.
