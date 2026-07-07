# Lesson 171 --- Release Pipeline

# Part 11 --- DevOps

> **Objective**
>
> Understand Release Pipelines, their purpose, relationship with Build
> Pipelines, release automation, artifact promotion, approval stages,
> deployment flow, environments, rollback strategies, and real-world
> release management practices.

------------------------------------------------------------------------

# Introduction

A build pipeline creates a validated software artifact.

But an artifact still needs to be delivered to users.

The process of moving software from build output to production is
handled by a **Release Pipeline**.

``` text
Source Code

      ↓

Build Pipeline

      ↓

Artifact

      ↓

Release Pipeline

      ↓

Production
```

------------------------------------------------------------------------

# What is a Release Pipeline?

A **Release Pipeline** is an automated workflow that manages the process
of delivering a software artifact to different environments and
eventually releasing it to users.

It handles:

-   Deployment
-   Approval
-   Environment promotion
-   Release management
-   Rollback

------------------------------------------------------------------------

# Why Do We Need Release Pipelines?

Without automation:

``` text
Build Complete

      ↓

Manual Deployment

      ↓

Configuration Errors

      ↓

Release Problems
```

Problems:

-   Slow releases
-   Human errors
-   Inconsistent deployments
-   Difficult rollback

------------------------------------------------------------------------

# Goals of Release Pipeline

A release pipeline provides:

-   Faster software delivery
-   Reliable deployments
-   Consistent environments
-   Controlled releases
-   Easy recovery

------------------------------------------------------------------------

# Build Pipeline vs Release Pipeline

  Build Pipeline            Release Pipeline
  ------------------------- ----------------------
  Creates artifact          Deploys artifact
  Compiles and tests code   Delivers software
  Validates application     Manages environments
  Developer focused         Operations focused

------------------------------------------------------------------------

# Release Pipeline Architecture

Typical flow:

``` text
Artifact

   ↓

Development Environment

   ↓

Testing Environment

   ↓

Staging Environment

   ↓

Production Environment
```

------------------------------------------------------------------------

# Release Pipeline Stages

## Stage 1 --- Artifact Selection

The pipeline selects the approved artifact.

Example:

    Application v2.0

------------------------------------------------------------------------

# Stage 2 --- Environment Deployment

The artifact is deployed into an environment.

Examples:

-   Development
-   Testing
-   Staging
-   Production

------------------------------------------------------------------------

# Stage 3 --- Validation

The deployment is verified.

Checks:

-   Application availability
-   Automated tests
-   Health checks

------------------------------------------------------------------------

# Stage 4 --- Approval

Some organizations require approval before production deployment.

Example:

    Testing

     ↓

    Manager Approval

     ↓

    Production

------------------------------------------------------------------------

# Stage 5 --- Production Release

The application becomes available to users.

------------------------------------------------------------------------

# Release Pipeline Workflow

``` text
Build Completed

      ↓

Artifact Created

      ↓

Deploy to Dev

      ↓

Run Tests

      ↓

Deploy to Staging

      ↓

Approval

      ↓

Deploy to Production
```

------------------------------------------------------------------------

# Release Environments

Software moves through multiple environments.

## Development Environment

Used by developers.

Purpose:

-   Feature testing
-   Early validation

------------------------------------------------------------------------

## Testing Environment

Used for:

-   QA testing
-   Integration testing

------------------------------------------------------------------------

## Staging Environment

A production-like environment.

Purpose:

-   Final verification
-   Performance testing

------------------------------------------------------------------------

## Production Environment

The live environment used by customers.

------------------------------------------------------------------------

# Artifact Promotion

Artifact promotion means moving the same tested artifact through
environments.

Example:

``` text
Artifact v1.5

      ↓

Development

      ↓

Testing

      ↓

Production
```

Benefits:

-   Consistency
-   Less risk
-   Better traceability

------------------------------------------------------------------------

# Deployment Strategies in Release Pipelines

## 1. Rolling Deployment

Updates servers gradually.

Example:

    Server 1

    Server 2

    Server 3

------------------------------------------------------------------------

## 2. Blue-Green Deployment

Two environments:

    Blue

    (Current Version)


    Green

    (New Version)

Traffic switches after validation.

------------------------------------------------------------------------

## 3. Canary Deployment

Release to a small group first.

Example:

    5% Users

          ↓

    Monitor

          ↓

    100% Users

------------------------------------------------------------------------

# Rollback Strategy

A rollback returns the system to a previous stable version.

Example:

    New Release

          ↓

    Failure

          ↓

    Previous Version Restored

------------------------------------------------------------------------

# Release Automation Tools

Common tools:

## Jenkins

Used for:

-   Pipeline automation
-   Deployment workflows

------------------------------------------------------------------------

## GitHub Actions

Used for:

-   Automated releases
-   Deployment workflows

------------------------------------------------------------------------

## GitLab CI/CD

Provides:

-   Build pipelines
-   Release automation

------------------------------------------------------------------------

## Argo CD

Used for:

-   Kubernetes deployments
-   GitOps workflows

------------------------------------------------------------------------

# Release Pipeline Example

## Banking Application

Flow:

``` text
Code Change

      ↓

Build Pipeline

      ↓

Artifact Created

      ↓

Testing Environment

      ↓

Security Validation

      ↓

Approval

      ↓

Production Release
```

------------------------------------------------------------------------

# Release Pipeline Best Practices

-   Automate deployments
-   Maintain environment consistency
-   Use versioned artifacts
-   Monitor releases
-   Have rollback plans
-   Require approvals for critical systems

------------------------------------------------------------------------

# Common Release Problems

## Problem 1 --- Deployment Failure

Solution:

Use rollback mechanisms.

------------------------------------------------------------------------

## Problem 2 --- Environment Differences

Solution:

Use configuration management.

------------------------------------------------------------------------

## Problem 3 --- Manual Errors

Solution:

Automate release steps.

------------------------------------------------------------------------

# Interview Questions

## 1. What is a Release Pipeline?

A Release Pipeline is an automated workflow that deploys software
artifacts across environments and manages software delivery.

------------------------------------------------------------------------

## 2. Difference between Build Pipeline and Release Pipeline?

Build Pipeline creates and validates artifacts.

Release Pipeline deploys and manages those artifacts.

------------------------------------------------------------------------

## 3. What are release environments?

Common environments:

-   Development
-   Testing
-   Staging
-   Production

------------------------------------------------------------------------

## 4. What is artifact promotion?

Artifact promotion is moving the same tested artifact through different
environments.

------------------------------------------------------------------------

## 5. Why are rollback strategies important?

They help restore stable software quickly after deployment failures.

------------------------------------------------------------------------

# Cheat Sheet

``` text
Release Pipeline

Artifact

   ↓

Development

   ↓

Testing

   ↓

Staging

   ↓

Approval

   ↓

Production

   ↓

Monitoring
```

------------------------------------------------------------------------

# Summary

A Release Pipeline automates the process of delivering software from a
validated artifact to production. It manages deployments, approvals,
environments, and rollback strategies. Together with Build Pipelines,
Release Pipelines create a reliable CI/CD workflow that enables faster
and safer software delivery.
