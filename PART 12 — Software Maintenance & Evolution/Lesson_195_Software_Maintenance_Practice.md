# Lesson 195 --- Software Maintenance Practice

# Part 12 --- Software Maintenance

> **Objective**
>
> Practice software maintenance concepts through real-world exercises
> involving maintenance types, legacy systems, technical debt,
> refactoring, documentation, change management, versioning, release
> management, and problem-solving scenarios.

------------------------------------------------------------------------

# Introduction

Software maintenance skills are developed through practical problem
solving.

A software engineer must understand:

-   How to fix existing systems
-   How to improve software quality
-   How to manage changes safely
-   How to maintain long-term reliability

``` text
Identify Problem

      ↓

Analyze

      ↓

Improve

      ↓

Test

      ↓

Release
```

------------------------------------------------------------------------

# Practice 1 --- Identify Maintenance Type

## Scenario 1

A payment application crashes when users complete transactions.

Question:

Which maintenance type is required?

Answer:

    Corrective Maintenance

Reason:

Existing defect needs to be fixed.

------------------------------------------------------------------------

## Scenario 2

A company moves its application from local servers to cloud
infrastructure.

Question:

Which maintenance type is required?

Answer:

    Adaptive Maintenance

Reason:

Software must adapt to a new environment.

------------------------------------------------------------------------

## Scenario 3

Users request a better search feature.

Question:

Which maintenance type is required?

Answer:

    Perfective Maintenance

Reason:

Existing functionality is being improved.

------------------------------------------------------------------------

## Scenario 4

Developers clean old code and update dependencies.

Question:

Which maintenance type is required?

Answer:

    Preventive Maintenance

Reason:

Future problems are being prevented.

------------------------------------------------------------------------

# Practice 2 --- Bug Fixing Workflow

## Scenario

Users report that login fails after deployment.

Task:

Design the corrective maintenance process.

Solution:

    User Report

          ↓

    Create Bug Ticket

          ↓

    Analyze Logs

          ↓

    Find Root Cause

          ↓

    Fix Code

          ↓

    Regression Testing

          ↓

    Deploy Patch

          ↓

    Monitor

------------------------------------------------------------------------

# Practice 3 --- Legacy System Modernization

## Scenario

A bank uses a 20-year-old application.

Problems:

-   Slow performance
-   Security issues
-   Difficult maintenance

Task:

Suggest modernization strategy.

Solution:

Steps:

    Analyze Existing System

          ↓

    Document Architecture

          ↓

    Choose Migration Strategy

          ↓

    Modernize Components

          ↓

    Test

          ↓

    Deploy

Possible approaches:

-   Rehosting
-   Replatforming
-   Refactoring
-   Reengineering

------------------------------------------------------------------------

# Practice 4 --- Technical Debt Identification

## Scenario

A project has:

-   Duplicate code
-   Missing tests
-   Poor documentation
-   Outdated libraries

Identify technical debt.

Answer:

    Code Debt

    Testing Debt

    Documentation Debt

    Dependency Debt

------------------------------------------------------------------------

# Practice 5 --- Refactoring Exercise

## Problem

A function contains:

    500 Lines

    Multiple Responsibilities

    Duplicate Logic

Task:

Suggest improvements.

Solution:

Apply:

-   Extract methods
-   Split classes
-   Remove duplicate code
-   Add tests

------------------------------------------------------------------------

# Practice 6 --- Documentation Exercise

## Scenario

A new developer joins a project.

Problem:

No documentation exists.

Task:

Create documentation plan.

Solution:

Create:

    Architecture Document

    API Documentation

    Database Documentation

    Deployment Guide

    User Guide

------------------------------------------------------------------------

# Practice 7 --- Change Request Handling

## Scenario

Business requests a new payment feature.

Process:

    Change Request

          ↓

    Impact Analysis

          ↓

    Approval

          ↓

    Development

          ↓

    Testing

          ↓

    Deployment

------------------------------------------------------------------------

# Practice 8 --- Change Impact Analysis

## Scenario

Database schema needs modification.

Analyze:

-   Affected modules
-   API impact
-   Migration requirements
-   Testing needs

------------------------------------------------------------------------

# Practice 9 --- Versioning Practice

## Task

Assign versions.

------------------------------------------------------------------------

## Bug Fix Release

Answer:

    1.0.1

Reason:

Patch update.

------------------------------------------------------------------------

## New Feature Addition

Answer:

    1.1.0

Reason:

Minor feature update.

------------------------------------------------------------------------

## Breaking API Change

Answer:

    2.0.0

Reason:

Major version change.

------------------------------------------------------------------------

# Practice 10 --- Release Planning

## Scenario

An e-commerce application releases a new checkout system.

Create release plan.

Solution:

    Feature Development

          ↓

    Testing

          ↓

    Security Review

          ↓

    Approval

          ↓

    Canary Release

          ↓

    Monitoring

          ↓

    Full Deployment

------------------------------------------------------------------------

# Practice 11 --- Rollback Scenario

## Problem

New release causes production failures.

Solution:

    Detect Failure

          ↓

    Stop Deployment

          ↓

    Rollback Previous Version

          ↓

    Investigate Issue

          ↓

    Release Fix

------------------------------------------------------------------------

# Practice 12 --- Maintenance Workflow Design

Design complete maintenance workflow.

Solution:

    Issue Detection

          ↓

    Classification

          ↓

    Analysis

          ↓

    Change Planning

          ↓

    Implementation

          ↓

    Testing

          ↓

    Release

          ↓

    Monitoring

------------------------------------------------------------------------

# Practice 13 --- Real-World Project Exercise

## Project

Maintain an online banking application.

Requirements:

-   Fix transaction bugs
-   Add mobile payment support
-   Improve performance
-   Update security
-   Maintain documentation

------------------------------------------------------------------------

# Solution Approach

## Corrective

Fix transaction failures.

------------------------------------------------------------------------

## Adaptive

Support new banking infrastructure.

------------------------------------------------------------------------

## Perfective

Improve payment experience.

------------------------------------------------------------------------

## Preventive

Refactor old modules and improve security.

------------------------------------------------------------------------

# Practice Questions

## Q1. A software has slow response time. What maintenance can improve it?

Answer:

Perfective Maintenance.

------------------------------------------------------------------------

## Q2. A vulnerability is found in an old library. What action is needed?

Answer:

Preventive Maintenance.

------------------------------------------------------------------------

## Q3. A company upgrades its database system. Which maintenance type?

Answer:

Adaptive Maintenance.

------------------------------------------------------------------------

## Q4. A production bug affects users. What should happen first?

Answer:

Create issue, analyze root cause, and perform corrective maintenance.

------------------------------------------------------------------------

## Q5. Why is refactoring important?

Answer:

It improves code quality and reduces technical debt.

------------------------------------------------------------------------

# Maintenance Checklist

✓ Identify maintenance type

✓ Analyze impact

✓ Document changes

✓ Test modifications

✓ Review code

✓ Deploy safely

✓ Monitor results

✓ Update documentation

------------------------------------------------------------------------

# Final Workflow

    Problem

     ↓

    Analyze

     ↓

    Choose Maintenance Type

     ↓

    Implement Change

     ↓

    Test

     ↓

    Release

     ↓

    Improve

------------------------------------------------------------------------

# Summary

Software maintenance practice develops the ability to manage real-world
software changes. Engineers must identify problems correctly, choose
suitable maintenance strategies, improve code quality, handle changes
safely, and maintain reliable software systems.

Strong maintenance skills help software survive long-term business and
technology evolution.
