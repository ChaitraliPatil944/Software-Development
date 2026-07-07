# Lesson 191 --- Change Management

# Part 12 --- Software Maintenance

> **Objective**
>
> Understand Change Management, why it is required, software change
> processes, change requests, impact analysis, approval processes,
> Change Control Board (CCB), change management in Agile and DevOps,
> challenges, best practices, and real-world applications.

------------------------------------------------------------------------

# Introduction

Software systems continuously change after deployment.

Changes may be required because of:

-   New business requirements
-   Bug fixes
-   Security updates
-   Technology upgrades
-   User feedback

Managing these changes properly is called **Change Management**.

``` text
Change Request

      ↓

Analysis

      ↓

Approval

      ↓

Implementation

      ↓

Verification
```

------------------------------------------------------------------------

# What is Change Management?

**Change Management** is the process of controlling, analyzing,
approving, implementing, and tracking changes made to software systems.

Simple definition:

    Change Management = Controlled Software Changes

------------------------------------------------------------------------

# Why is Change Management Needed?

Without proper management:

    Random Changes

          ↓

    System Instability

          ↓

    Failures

Problems:

-   Unexpected bugs
-   Service disruption
-   Poor tracking
-   Security risks

------------------------------------------------------------------------

# Goals of Change Management

Change management aims to:

-   Reduce risks
-   Maintain software stability
-   Ensure proper approval
-   Track modifications
-   Improve communication

------------------------------------------------------------------------

# Types of Software Changes

## 1. Corrective Changes

Fix existing problems.

Example:

    Bug Fix

------------------------------------------------------------------------

## 2. Adaptive Changes

Adjust software to environmental changes.

Example:

    Database Migration

------------------------------------------------------------------------

## 3. Perfective Changes

Improve features and performance.

Example:

    New Feature

------------------------------------------------------------------------

## 4. Preventive Changes

Avoid future problems.

Example:

    Security Improvement

------------------------------------------------------------------------

# Change Management Process

``` text
Identify Change

      ↓

Create Change Request

      ↓

Impact Analysis

      ↓

Approval

      ↓

Implementation

      ↓

Testing

      ↓

Deployment

      ↓

Review
```

------------------------------------------------------------------------

# Step 1 --- Identify Change

Changes come from:

-   Users
-   Developers
-   Business teams
-   Security teams
-   Monitoring systems

Example:

    Customer Requests New Payment Option

------------------------------------------------------------------------

# Step 2 --- Change Request

A formal request is created.

It contains:

-   Change description
-   Reason
-   Expected impact
-   Priority
-   Required resources

------------------------------------------------------------------------

# Step 3 --- Impact Analysis

Before implementation, teams analyze:

-   Technical impact
-   Cost
-   Time
-   Risks
-   Dependencies

Example:

    Database Change

          ↓

    Affects API Layer

          ↓

    Requires Testing

------------------------------------------------------------------------

# Step 4 --- Change Approval

Changes are reviewed before implementation.

Approval may involve:

-   Project managers
-   Technical leads
-   Change Control Board

------------------------------------------------------------------------

# Change Control Board (CCB)

A **Change Control Board** is a group responsible for reviewing and
approving significant changes.

Members may include:

-   Project managers
-   Developers
-   Operations teams
-   Business representatives

------------------------------------------------------------------------

# CCB Responsibilities

The CCB:

-   Reviews change requests
-   Evaluates risks
-   Approves or rejects changes
-   Maintains change records

------------------------------------------------------------------------

# Step 5 --- Implementation

Approved changes are developed.

Activities:

-   Code modification
-   Configuration updates
-   Infrastructure changes

------------------------------------------------------------------------

# Step 6 --- Testing

Changes are tested using:

-   Unit testing
-   Integration testing
-   Regression testing

------------------------------------------------------------------------

# Step 7 --- Deployment

The change is released.

Process:

    Deploy

     ↓

    Monitor

     ↓

    Verify

------------------------------------------------------------------------

# Step 8 --- Review

After implementation:

-   Check results
-   Update documentation
-   Record lessons learned

------------------------------------------------------------------------

# Change Management in Agile

Agile handles changes differently.

Characteristics:

-   Frequent changes
-   Short iterations
-   Continuous feedback

Process:

    Backlog

     ↓

    Sprint Planning

     ↓

    Development

     ↓

    Review

------------------------------------------------------------------------

# Change Management in DevOps

DevOps uses automation to manage changes.

Includes:

-   CI/CD pipelines
-   Automated testing
-   Infrastructure as Code
-   Monitoring

Workflow:

    Code Change

     ↓

    CI Pipeline

     ↓

    Testing

     ↓

    Deployment

     ↓

    Monitoring

------------------------------------------------------------------------

# Change Management Tools

Common tools:

-   Jira
-   ServiceNow
-   Git
-   Jenkins
-   GitHub Actions

------------------------------------------------------------------------

# Change Management Challenges

## 1. Resistance to Change

People may hesitate to adopt new systems.

------------------------------------------------------------------------

## 2. Poor Planning

Unplanned changes create risks.

------------------------------------------------------------------------

## 3. Communication Problems

Teams may not know about changes.

------------------------------------------------------------------------

## 4. Change Overload

Too many changes can affect stability.

------------------------------------------------------------------------

# Best Practices

## 1. Document Every Change

Maintain change history.

------------------------------------------------------------------------

## 2. Perform Impact Analysis

Understand consequences before changing.

------------------------------------------------------------------------

## 3. Automate Testing

Reduce change-related risks.

------------------------------------------------------------------------

## 4. Use Version Control

Track all modifications.

------------------------------------------------------------------------

## 5. Have Rollback Plans

Restore previous versions if needed.

------------------------------------------------------------------------

# Real-World Example

## Banking Application

Change:

    Add New Payment Gateway

Process:

    Change Request

          ↓

    Security Review

          ↓

    Impact Analysis

          ↓

    Approval

          ↓

    Development

          ↓

    Testing

          ↓

    Production Release

------------------------------------------------------------------------

# Change Management vs Configuration Management

  Change Management           Configuration Management
  --------------------------- --------------------------
  Controls modifications      Manages system settings
  Focuses on change process   Focuses on system state

------------------------------------------------------------------------

# Interview Questions

## 1. What is Change Management?

Change Management controls and manages software changes to reduce risks.

------------------------------------------------------------------------

## 2. Why is change management important?

It ensures changes are planned, tested, approved, and safely
implemented.

------------------------------------------------------------------------

## 3. What is a Change Request?

A formal document describing a requested modification.

------------------------------------------------------------------------

## 4. What is CCB?

Change Control Board reviews and approves important changes.

------------------------------------------------------------------------

## 5. How does DevOps handle changes?

Through automation, CI/CD pipelines, testing, and monitoring.

------------------------------------------------------------------------

# Cheat Sheet

``` text
Change Management

Request

 ↓

Analyze

 ↓

Approve

 ↓

Implement

 ↓

Test

 ↓

Deploy

 ↓

Review
```

------------------------------------------------------------------------

# Summary

Change Management ensures software modifications are performed safely
and systematically. By analyzing impact, obtaining approval, testing
changes, and maintaining records, organizations reduce risks and
maintain stable software systems.

Effective change management is essential for reliable software
maintenance and continuous improvement.
