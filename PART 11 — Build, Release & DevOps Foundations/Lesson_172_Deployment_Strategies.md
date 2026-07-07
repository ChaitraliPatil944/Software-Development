# Lesson 172 --- Deployment Strategies

# Part 11 --- DevOps

> **Objective**
>
> Understand deployment strategies, why they are required, different
> deployment approaches, zero-downtime deployment, rollback handling,
> strategy comparison, and real-world usage in production systems.

------------------------------------------------------------------------

# Introduction

After software is tested and ready, it must be deployed to users.

The way software is released can affect:

-   Availability
-   User experience
-   Risk
-   Recovery time

Deployment strategies define how new versions are introduced into
production.

``` text
New Version

      ↓

Deployment Strategy

      ↓

Production Users
```

------------------------------------------------------------------------

# What are Deployment Strategies?

A **Deployment Strategy** is a method used to release a new version of
an application into a production environment.

It defines:

-   How updates are delivered
-   How traffic is managed
-   How failures are handled
-   How rollback is performed

------------------------------------------------------------------------

# Why Do We Need Deployment Strategies?

Without proper strategy:

    New Release

          ↓

    Direct Deployment

          ↓

    Failure

          ↓

    System Downtime

Problems:

-   Service interruption
-   User impact
-   Difficult rollback
-   High deployment risk

------------------------------------------------------------------------

# Goals of Deployment Strategies

A good deployment strategy provides:

-   Minimum downtime
-   Reduced risk
-   Faster recovery
-   Better user experience
-   Controlled releases

------------------------------------------------------------------------

# 1. Recreate Deployment

## Concept

The old version is stopped before the new version starts.

Flow:

    Old Version

          ↓

    Stop Application

          ↓

    Deploy New Version

          ↓

    Start Application

------------------------------------------------------------------------

## Advantages

-   Simple approach
-   Easy to understand
-   Low infrastructure requirement

------------------------------------------------------------------------

## Disadvantages

-   Downtime occurs
-   Not suitable for critical systems

------------------------------------------------------------------------

## Example

Small internal application update.

------------------------------------------------------------------------

# 2. Rolling Deployment

## Concept

The new version replaces the old version gradually.

Example:

    Servers:

    A  Old

    B  Old

    C  Old


    Update:


    A  New

    B  Old

    C  Old


    A  New

    B  New

    C  Old


    All New

------------------------------------------------------------------------

## Advantages

-   Minimal downtime
-   Controlled release
-   Lower resource usage

------------------------------------------------------------------------

## Disadvantages

-   Multiple versions run together
-   Rollback can be complex

------------------------------------------------------------------------

## Example

Web applications with multiple servers.

------------------------------------------------------------------------

# 3. Blue-Green Deployment

## Concept

Two identical environments are maintained.

    Blue Environment

    (Current Version)


    Green Environment

    (New Version)

Traffic switches after validation.

------------------------------------------------------------------------

## Workflow

    Deploy New Version

            ↓

    Test Green Environment

            ↓

    Switch Traffic

            ↓

    Green Becomes Production

------------------------------------------------------------------------

## Advantages

-   Almost zero downtime
-   Easy rollback
-   Safer releases

------------------------------------------------------------------------

## Disadvantages

-   Requires duplicate infrastructure
-   Higher cost

------------------------------------------------------------------------

# 4. Canary Deployment

## Concept

A new version is released to a small percentage of users first.

Example:

    5% Users

          ↓

    Monitor

          ↓

    50% Users

          ↓

    100% Users

------------------------------------------------------------------------

## Advantages

-   Reduces risk
-   Real user feedback
-   Early issue detection

------------------------------------------------------------------------

## Disadvantages

-   Complex traffic management
-   Requires monitoring

------------------------------------------------------------------------

## Example

Large platforms releasing features gradually.

------------------------------------------------------------------------

# 5. A/B Testing Deployment

## Concept

Two versions are shown to different user groups.

Example:

    Group A

    Version 1


    Group B

    Version 2

Performance and user behavior are compared.

------------------------------------------------------------------------

## Uses

-   UI experiments
-   Feature testing
-   User experience improvement

------------------------------------------------------------------------

# 6. Feature Flag Deployment

## Concept

Code is deployed but features are controlled using configuration
switches.

Example:

    Application Code

          +

    Feature Flag

          ↓

    Feature Enabled/Disabled

------------------------------------------------------------------------

## Advantages

-   Safe feature release
-   Quick disabling
-   Experiment support

------------------------------------------------------------------------

# Zero-Downtime Deployment

Zero-downtime deployment means users can continue using the application
while updates are released.

Achieved using:

-   Rolling deployment
-   Blue-green deployment
-   Load balancing
-   Health checks

------------------------------------------------------------------------

# Deployment Strategy Comparison

  Strategy     Downtime   Risk       Infrastructure
  ------------ ---------- ---------- ----------------
  Recreate     High       High       Low
  Rolling      Low        Medium     Medium
  Blue-Green   Very Low   Low        High
  Canary       Very Low   Very Low   Medium/High

------------------------------------------------------------------------

# Deployment Strategy Selection

Choose based on:

## Application Type

Example:

Banking systems require safer strategies.

------------------------------------------------------------------------

## User Impact

Customer-facing systems need minimal downtime.

------------------------------------------------------------------------

## Infrastructure Budget

Blue-green requires more resources.

------------------------------------------------------------------------

## Release Frequency

Frequent releases benefit from automation.

------------------------------------------------------------------------

# Deployment in CI/CD Pipeline

Typical flow:

    Code Commit

          ↓

    Build

          ↓

    Test

          ↓

    Artifact

          ↓

    Deployment Strategy

          ↓

    Production

          ↓

    Monitoring

------------------------------------------------------------------------

# Rollback Strategy

Rollback restores the previous stable version.

Example:

    Version 2.0

          ↓

    Failure

          ↓

    Rollback

          ↓

    Version 1.9

------------------------------------------------------------------------

# Deployment Tools

Common tools:

-   Kubernetes
-   Docker
-   Jenkins
-   GitHub Actions
-   Argo CD
-   AWS CodeDeploy

------------------------------------------------------------------------

# Real-World Example

## E-Commerce Platform

New payment service release:

Option:

Canary Deployment

    Deploy to 5% users

          ↓

    Monitor Errors

          ↓

    Increase Traffic

          ↓

    Full Release

------------------------------------------------------------------------

# Best Practices

-   Automate deployments
-   Monitor applications
-   Maintain rollback plans
-   Test before production
-   Use versioned releases
-   Track deployment metrics

------------------------------------------------------------------------

# Common Mistakes

## Mistake 1

Deploying directly without testing.

Solution:

Use staged environments.

------------------------------------------------------------------------

## Mistake 2

No rollback plan.

Solution:

Always maintain previous stable versions.

------------------------------------------------------------------------

## Mistake 3

Ignoring monitoring.

Solution:

Track application health after deployment.

------------------------------------------------------------------------

# Interview Questions

## 1. What is a deployment strategy?

A deployment strategy defines how a new software version is released
into production.

------------------------------------------------------------------------

## 2. Explain rolling deployment.

Rolling deployment gradually replaces old instances with new ones.

------------------------------------------------------------------------

## 3. Difference between blue-green and canary deployment?

Blue-green switches between two environments.

Canary releases to a small user group first.

------------------------------------------------------------------------

## 4. What is zero-downtime deployment?

A deployment approach where users experience no service interruption
during updates.

------------------------------------------------------------------------

## 5. Which deployment strategy is safest?

Canary deployment is often safest because changes are gradually
introduced and monitored.

------------------------------------------------------------------------

# Cheat Sheet

    Deployment Strategies

    Recreate
        ↓
    Rolling
        ↓
    Blue-Green
        ↓
    Canary
        ↓
    Feature Flags

------------------------------------------------------------------------

# Summary

Deployment strategies help organizations release software safely and
efficiently. Different strategies such as rolling, blue-green, and
canary deployment provide different levels of risk control, downtime
reduction, and infrastructure requirements.

Choosing the right deployment strategy is essential for reliable
production software delivery.
