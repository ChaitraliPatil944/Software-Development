# Lesson 169 --- Continuous Delivery and Continuous Deployment (CD)

# Part 11 --- DevOps

> **Objective**
>
> Understand Continuous Delivery and Continuous Deployment, why they
> exist, their relationship with Continuous Integration, CD pipelines,
> deployment automation, release processes, deployment tools,
> strategies, benefits, challenges, and real-world usage.

------------------------------------------------------------------------

# Introduction

Continuous Integration ensures that code changes are automatically built
and tested.

But after testing, organizations need to deliver software to users.

This is where Continuous Delivery and Continuous Deployment come into
play.

``` text
Continuous Integration

        ↓

Continuous Delivery

        ↓

Continuous Deployment

        ↓

Users
```

------------------------------------------------------------------------

# What is Continuous Delivery?

**Continuous Delivery (CD)** is a DevOps practice where software changes
are automatically prepared and kept ready for release.

The application is always in a deployable state.

Simple definition:

    Continuous Delivery = Build + Test + Release Preparation

------------------------------------------------------------------------

# What is Continuous Deployment?

**Continuous Deployment** is the practice of automatically deploying
every validated change directly into production.

Simple definition:

    Continuous Deployment = Automatic Production Release

------------------------------------------------------------------------

# Continuous Delivery vs Continuous Deployment

  Continuous Delivery             Continuous Deployment
  ------------------------------- ------------------------------------
  Software is ready for release   Software is automatically released
  Manual approval may exist       No manual approval
  Safer release control           Faster releases

------------------------------------------------------------------------

# Why Do We Need CD?

Without CD:

    Code Ready

          ↓

    Manual Release Process

          ↓

    Delay

          ↓

    Slow Delivery

Problems:

-   Manual deployment errors
-   Slow releases
-   Difficult rollback
-   Inconsistent environments

------------------------------------------------------------------------

# Goals of CD

Continuous Delivery aims to:

-   Release software faster
-   Reduce deployment risk
-   Automate delivery steps
-   Improve reliability
-   Provide faster customer feedback

------------------------------------------------------------------------

# CI/CD Relationship

CI and CD work together.

    Developer

       ↓

    Git Repository

       ↓

    CI

    (Build + Test)

       ↓

    CD

    (Release + Deploy)

       ↓

    Production

------------------------------------------------------------------------

# CD Pipeline

A CD pipeline automates software delivery.

Example:

    Code Approved

          ↓

    Build Artifact

          ↓

    Release Preparation

          ↓

    Deployment

          ↓

    Monitoring

------------------------------------------------------------------------

# CD Pipeline Stages

## 1. Source Stage

Code is obtained from repository.

Examples:

-   GitHub
-   GitLab

------------------------------------------------------------------------

# 2. Build Stage

Application packages are created.

Examples:

Java:

    .jar file

Node.js:

    Build package

------------------------------------------------------------------------

# 3. Testing Stage

Automated tests validate the application.

Includes:

-   Unit tests
-   Integration tests
-   Security tests

------------------------------------------------------------------------

# 4. Artifact Storage

Generated packages are stored.

Examples:

-   Docker Registry
-   Artifact Repository

------------------------------------------------------------------------

# 5. Deployment Stage

Application is deployed to environments.

Example:

    Testing Environment

            ↓

    Production Environment

------------------------------------------------------------------------

# Continuous Delivery Workflow

    Developer

          ↓

    Commit Code

          ↓

    CI Pipeline

          ↓

    Tests Passed

          ↓

    Release Ready

          ↓

    Manual Approval

          ↓

    Production

------------------------------------------------------------------------

# Continuous Deployment Workflow

    Developer

          ↓

    Commit Code

          ↓

    CI Pipeline

          ↓

    Tests Passed

          ↓

    Automatic Deployment

          ↓

    Production

------------------------------------------------------------------------

# CD Tools Overview

## Jenkins

Used for:

-   Pipeline automation
-   Build and deployment

------------------------------------------------------------------------

## GitHub Actions

Provides:

-   Workflow automation
-   CI/CD pipelines

------------------------------------------------------------------------

## GitLab CI/CD

Integrated DevOps platform.

------------------------------------------------------------------------

## Argo CD

Used for:

-   Kubernetes deployments
-   GitOps workflows

------------------------------------------------------------------------

# Deployment Automation

CD automates:

-   Server configuration
-   Application deployment
-   Environment setup
-   Rollbacks

Benefits:

-   Faster releases
-   Fewer mistakes
-   Repeatable deployments

------------------------------------------------------------------------

# Deployment Pipeline Example

Application:

    E-Commerce System

Flow:

    Developer Push

          ↓

    CI Build

          ↓

    Automated Tests

          ↓

    Create Docker Image

          ↓

    Deploy to Cloud

          ↓

    Monitor Application

------------------------------------------------------------------------

# Continuous Delivery Benefits

## Faster Releases

Teams release features quickly.

------------------------------------------------------------------------

## Improved Quality

Automated testing reduces defects.

------------------------------------------------------------------------

## Reduced Risk

Small changes are easier to manage.

------------------------------------------------------------------------

## Better Customer Experience

Users receive improvements faster.

------------------------------------------------------------------------

# Continuous Deployment Benefits

-   Fully automated delivery
-   Extremely fast releases
-   Immediate feedback
-   Reduced manual work

------------------------------------------------------------------------

# Challenges of CD

## 1. Requires Strong Testing

Automation needs reliable tests.

------------------------------------------------------------------------

## 2. Monitoring is Essential

Production issues must be detected quickly.

------------------------------------------------------------------------

## 3. Cultural Change

Teams must trust automation.

------------------------------------------------------------------------

## 4. Security Requirements

Deployment pipelines must protect sensitive systems.

------------------------------------------------------------------------

# CD Best Practices

## Automate Everything Possible

Automate:

-   Build
-   Testing
-   Deployment

------------------------------------------------------------------------

## Maintain Deployment Environments

Keep environments consistent.

------------------------------------------------------------------------

## Use Version Control

Store:

-   Code
-   Configuration
-   Pipeline definitions

------------------------------------------------------------------------

## Monitor After Deployment

Track:

-   Errors
-   Performance
-   Availability

------------------------------------------------------------------------

# CI/CD Pipeline Example

    Developer

     ↓

    Git Commit

     ↓

    CI Build

     ↓

    Automated Tests

     ↓

    Artifact Creation

     ↓

    CD Deployment

     ↓

    Production Monitoring

------------------------------------------------------------------------

# Industry Example

## Banking Application

Developer updates transaction feature.

Process:

    Code Commit

          ↓

    Automated Security Tests

          ↓

    Build Package

          ↓

    Approval

          ↓

    Production Deployment

          ↓

    Monitoring

------------------------------------------------------------------------

# Interview Questions

## 1. What is Continuous Delivery?

Continuous Delivery is a practice where software is automatically
prepared and kept ready for release.

------------------------------------------------------------------------

## 2. What is Continuous Deployment?

Continuous Deployment automatically releases every validated change into
production.

------------------------------------------------------------------------

## 3. Difference between Continuous Delivery and Continuous Deployment?

Continuous Delivery requires possible manual approval.

Continuous Deployment automatically deploys changes.

------------------------------------------------------------------------

## 4. Explain CI/CD pipeline.

CI validates code changes.

CD automates software delivery and deployment.

------------------------------------------------------------------------

## 5. Name CD tools.

Examples:

-   Jenkins
-   GitHub Actions
-   GitLab CI/CD
-   Argo CD

------------------------------------------------------------------------

# Cheat Sheet

    CI/CD

    Code

     ↓

    Build

     ↓

    Test

     ↓

    Release

     ↓

    Deploy

     ↓

    Monitor

------------------------------------------------------------------------

# Summary

Continuous Delivery and Continuous Deployment extend Continuous
Integration by automating software release and deployment processes.
Continuous Delivery keeps software ready for release, while Continuous
Deployment automatically delivers validated changes to production.

Together, CI/CD creates a fast, reliable, and automated software
delivery pipeline that is a foundation of modern DevOps practices.
