# Lesson 183 --- Corrective Maintenance

# Part 12 --- Software Maintenance

> **Objective**
>
> Understand Corrective Maintenance, why it is required, defect fixing
> process, bug lifecycle, examples, challenges, best practices, and its
> role in software maintenance.

------------------------------------------------------------------------

# Introduction

After software is released, users may discover defects or unexpected
behavior.

Examples:

-   Application crashes
-   Incorrect output
-   Failed transactions
-   Security vulnerabilities

Fixing these problems is called **Corrective Maintenance**.

``` text
Software Released

        ↓

Defect Found

        ↓

Analyze Problem

        ↓

Fix Defect

        ↓

Deploy Update
```

------------------------------------------------------------------------

# What is Corrective Maintenance?

**Corrective Maintenance** is the process of modifying software to fix
errors, defects, or failures discovered after deployment.

Simple definition:

    Corrective Maintenance = Finding + Fixing Software Problems

------------------------------------------------------------------------

# Why is Corrective Maintenance Needed?

Software may contain defects due to:

-   Coding mistakes
-   Incorrect requirements
-   Testing limitations
-   Environment changes
-   Unexpected user behavior

Corrective maintenance restores correct system behavior.

------------------------------------------------------------------------

# Types of Defects

## 1. Functional Defects

Software does not perform expected functionality.

Example:

    Login button does not work

------------------------------------------------------------------------

## 2. Performance Defects

System performs slowly.

Example:

    API response takes too long

------------------------------------------------------------------------

## 3. Security Defects

Security weaknesses are discovered.

Example:

    Unauthorized access vulnerability

------------------------------------------------------------------------

## 4. Compatibility Defects

Software fails in different environments.

Example:

    Application fails on new browser version

------------------------------------------------------------------------

# Corrective Maintenance Process

``` text
Defect Detection

        ↓

Issue Reporting

        ↓

Problem Analysis

        ↓

Bug Fixing

        ↓

Testing

        ↓

Deployment

        ↓

Verification
```

------------------------------------------------------------------------

# Step 1 --- Defect Detection

Problems are identified through:

-   User reports
-   Monitoring alerts
-   Testing
-   Support tickets

Example:

    Customer reports payment failure

------------------------------------------------------------------------

# Step 2 --- Issue Analysis

Teams analyze:

-   Error logs
-   Source code
-   Recent changes
-   System behavior

Goal:

Find the cause of the defect.

------------------------------------------------------------------------

# Step 3 --- Bug Fixing

Developers modify code to remove the defect.

Example:

Before:

    Wrong calculation logic

After:

    Correct calculation implemented

------------------------------------------------------------------------

# Step 4 --- Testing

The fix is tested.

Testing includes:

-   Unit testing
-   Integration testing
-   Regression testing

------------------------------------------------------------------------

# Step 5 --- Deployment

The corrected version is released.

Flow:

    Fix

     ↓

    Test

     ↓

    Release

     ↓

    Monitor

------------------------------------------------------------------------

# Defect Lifecycle

A typical bug lifecycle:

``` text
New

 ↓

Assigned

 ↓

In Progress

 ↓

Fixed

 ↓

Testing

 ↓

Closed
```

------------------------------------------------------------------------

# Corrective Maintenance Example

## Banking Application

Problem:

    Users cannot complete transactions

Process:

    Incident Report

          ↓

    Analyze Logs

          ↓

    Find Code Error

          ↓

    Apply Fix

          ↓

    Test Transaction

          ↓

    Release Patch

------------------------------------------------------------------------

# Corrective Maintenance vs Preventive Maintenance

  Corrective                Preventive
  ------------------------- --------------------------------
  Fixes existing problems   Prevents future problems
  Reactive approach         Proactive approach
  Triggered by defects      Triggered by improvement needs

------------------------------------------------------------------------

# Challenges in Corrective Maintenance

## 1. Finding Root Cause

Large systems make debugging difficult.

------------------------------------------------------------------------

## 2. Risk of New Bugs

A fix may affect existing features.

------------------------------------------------------------------------

## 3. Limited Documentation

Missing information increases analysis time.

------------------------------------------------------------------------

## 4. Urgent Fix Requirements

Critical defects require quick response.

------------------------------------------------------------------------

# Best Practices

## 1. Maintain Bug Tracking

Use tools to track issues.

Examples:

-   Jira
-   GitHub Issues

------------------------------------------------------------------------

## 2. Perform Root Cause Analysis

Understand why the defect happened.

------------------------------------------------------------------------

## 3. Add Regression Tests

Ensure the problem does not return.

------------------------------------------------------------------------

## 4. Maintain Code Quality

Clean code reduces future defects.

------------------------------------------------------------------------

# Corrective Maintenance Tools

Common tools:

-   Jira
-   Bugzilla
-   GitHub Issues
-   Jenkins
-   Testing frameworks

------------------------------------------------------------------------

# Corrective Maintenance in SDLC

``` text
Development

      ↓

Testing

      ↓

Deployment

      ↓

Defect Found

      ↓

Corrective Maintenance

      ↓

Updated Software
```

------------------------------------------------------------------------

# Interview Questions

## 1. What is Corrective Maintenance?

Corrective Maintenance is the process of fixing defects discovered after
software deployment.

------------------------------------------------------------------------

## 2. Why is corrective maintenance required?

It restores software functionality and resolves failures.

------------------------------------------------------------------------

## 3. Give examples of corrective maintenance.

Examples:

-   Fixing application crashes
-   Fixing calculation errors
-   Fixing security bugs

------------------------------------------------------------------------

## 4. Difference between corrective and preventive maintenance?

Corrective fixes existing issues, while preventive avoids future
problems.

------------------------------------------------------------------------

## 5. What is regression testing?

Regression testing ensures that a bug fix has not broken existing
functionality.

------------------------------------------------------------------------

# Cheat Sheet

``` text
Corrective Maintenance

Bug Found

    ↓

Analyze

    ↓

Fix

    ↓

Test

    ↓

Deploy

    ↓

Verify
```

------------------------------------------------------------------------

# Summary

Corrective Maintenance focuses on identifying and fixing software
defects after deployment. It is an essential maintenance activity that
restores system reliability, improves user experience, and ensures
software continues to function correctly.
