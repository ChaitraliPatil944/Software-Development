# Lesson 182 --- Software Maintenance

# Part 12 --- Software Maintenance

> **Objective**
>
> Understand software maintenance, why maintenance is required after
> deployment, software maintenance lifecycle, maintenance activities,
> types of maintenance, challenges, cost factors, and its importance in
> real-world software engineering.

------------------------------------------------------------------------

# Introduction

Software development does not end after deployment.

Once users start using an application, new requirements, bugs, security
issues, and technology changes appear.

Software needs continuous improvement and support.

This process is called **Software Maintenance**.

``` text
Development

      ↓

Deployment

      ↓

Software Maintenance

      ↓

Continuous Improvement
```

------------------------------------------------------------------------

# What is Software Maintenance?

**Software Maintenance** is the process of modifying, updating,
improving, and managing software after it has been delivered to users.

It includes:

-   Fixing defects
-   Adding new features
-   Improving performance
-   Adapting to new environments
-   Preventing future problems

------------------------------------------------------------------------

# Why is Software Maintenance Needed?

Software operates in changing environments.

Changes happen because of:

-   User requirements
-   Business needs
-   Technology updates
-   Security threats
-   Hardware changes

Without maintenance:

    Old Software

          ↓

    Performance Issues

          ↓

    System Failure

------------------------------------------------------------------------

# Software Maintenance Lifecycle

A typical maintenance process:

``` text
Issue Identification

        ↓

Analysis

        ↓

Change Planning

        ↓

Implementation

        ↓

Testing

        ↓

Deployment

        ↓

Monitoring
```

------------------------------------------------------------------------

# Software Maintenance Activities

## 1. Bug Fixing

Correct errors found after release.

Examples:

-   Application crashes
-   Incorrect calculations
-   Failed transactions

------------------------------------------------------------------------

## 2. Feature Enhancement

Adding new capabilities.

Examples:

-   New payment option
-   Better user interface
-   Additional reports

------------------------------------------------------------------------

## 3. Performance Improvement

Improving:

-   Speed
-   Memory usage
-   Response time

------------------------------------------------------------------------

## 4. Security Updates

Protecting software from threats.

Examples:

-   Security patches
-   Vulnerability fixes

------------------------------------------------------------------------

## 5. Platform Updates

Adapting software to:

-   New operating systems
-   New browsers
-   New hardware

------------------------------------------------------------------------

# Types of Software Maintenance

Software maintenance is classified into four major types:

    Corrective

    Adaptive

    Perfective

    Preventive

------------------------------------------------------------------------

# 1. Corrective Maintenance

Purpose:

Fix defects and errors after deployment.

Example:

    Payment module fails

            ↓

    Bug Fix

------------------------------------------------------------------------

# 2. Adaptive Maintenance

Purpose:

Modify software for environmental changes.

Examples:

-   New operating system
-   New database version
-   Cloud migration

------------------------------------------------------------------------

# 3. Perfective Maintenance

Purpose:

Improve software performance and features.

Examples:

-   Better user experience
-   Faster response time
-   New functionality

------------------------------------------------------------------------

# 4. Preventive Maintenance

Purpose:

Prevent future problems.

Examples:

-   Code cleanup
-   Refactoring
-   Updating dependencies

------------------------------------------------------------------------

# Software Maintenance Cost

Maintenance often consumes a large portion of software lifecycle cost.

Reasons:

-   Existing code complexity
-   Lack of documentation
-   Changing requirements
-   Technical debt

------------------------------------------------------------------------

# Factors Affecting Maintenance Cost

## 1. Software Complexity

Complex systems require more effort.

------------------------------------------------------------------------

## 2. Code Quality

Poor-quality code increases maintenance difficulty.

------------------------------------------------------------------------

## 3. Documentation Quality

Good documentation reduces understanding time.

------------------------------------------------------------------------

## 4. Developer Knowledge

Understanding existing systems affects maintenance speed.

------------------------------------------------------------------------

## 5. Technology Changes

Older technologies require adaptation.

------------------------------------------------------------------------

# Maintenance Challenges

## 1. Understanding Existing Code

Large systems may have years of modifications.

------------------------------------------------------------------------

## 2. Changing Requirements

Business needs continuously evolve.

------------------------------------------------------------------------

## 3. Legacy Technology

Old systems may use outdated platforms.

------------------------------------------------------------------------

## 4. Risk of Introducing Bugs

Changes can affect existing functionality.

------------------------------------------------------------------------

## 5. Lack of Documentation

Missing information makes maintenance difficult.

------------------------------------------------------------------------

# Software Maintenance and SDLC

Maintenance is the final phase of the Software Development Life Cycle.

``` text
Requirement

 ↓

Design

 ↓

Development

 ↓

Testing

 ↓

Deployment

 ↓

Maintenance
```

------------------------------------------------------------------------

# Maintenance vs Development

  Development                Maintenance
  -------------------------- -----------------------------
  Creates new software       Improves existing software
  Starts from requirements   Starts from existing system
  More design work           More analysis work

------------------------------------------------------------------------

# Real-World Example

## Banking Application

After deployment:

Issue:

    Transaction failure detected

Maintenance process:

    Analyze Issue

          ↓

    Fix Defect

          ↓

    Test

          ↓

    Deploy Update

Later:

    Add New Payment Method

          ↓

    Perfective Maintenance

------------------------------------------------------------------------

# Software Maintenance Best Practices

## 1. Maintain Documentation

Keep system knowledge updated.

------------------------------------------------------------------------

## 2. Write Clean Code

Readable code reduces maintenance effort.

------------------------------------------------------------------------

## 3. Use Version Control

Track every change.

------------------------------------------------------------------------

## 4. Automate Testing

Prevent new defects.

------------------------------------------------------------------------

## 5. Monitor Software

Detect issues early.

------------------------------------------------------------------------

# Interview Questions

## 1. What is software maintenance?

Software maintenance is the process of modifying and improving software
after deployment.

------------------------------------------------------------------------

## 2. Why is software maintenance important?

It helps fix defects, adapt to changes, improve performance, and
maintain software reliability.

------------------------------------------------------------------------

## 3. What are the four types of software maintenance?

-   Corrective
-   Adaptive
-   Perfective
-   Preventive

------------------------------------------------------------------------

## 4. Why is software maintenance expensive?

Because of system complexity, changing requirements, technical debt, and
lack of documentation.

------------------------------------------------------------------------

## 5. Is maintenance part of SDLC?

Yes. Maintenance is the final and longest phase of the software
lifecycle.

------------------------------------------------------------------------

# Cheat Sheet

``` text
Software Maintenance

Fix Bugs

+

Adapt Changes

+

Improve Features

+

Prevent Problems

        ↓

Reliable Software
```

------------------------------------------------------------------------

# Summary

Software Maintenance ensures that software remains useful, secure, and
reliable after deployment. It includes correcting errors, adapting to
changes, improving functionality, and preventing future problems.

A well-maintained software system survives changing business
requirements and technology evolution.
