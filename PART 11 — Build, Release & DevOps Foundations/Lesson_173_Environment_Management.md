# Lesson 173 --- Environment Management

# Part 11 --- DevOps

> **Objective**
>
> Understand software environments, environment management, differences
> between development, testing, staging, and production environments,
> environment consistency, configuration handling, promotion flow, and
> DevOps best practices.

------------------------------------------------------------------------

# Introduction

Software applications are not built and released in a single
environment.

Different stages are required to:

-   Develop features
-   Test functionality
-   Validate releases
-   Serve real users

These stages are called **software environments**.

``` text
Development

      ↓

Testing

      ↓

Staging

      ↓

Production
```

------------------------------------------------------------------------

# What is an Environment?

A **software environment** is a collection of resources required to run
an application.

It includes:

-   Application code
-   Operating system
-   Runtime
-   Libraries
-   Database
-   Configuration
-   Infrastructure

Example:

    Application

    +

    Database

    +

    Server

    +

    Configuration

    =

    Environment

------------------------------------------------------------------------

# Why Do We Need Multiple Environments?

Without separate environments:

    Developer Changes

          ↓

    Direct Production Update

          ↓

    System Failure

Multiple environments provide:

-   Safe testing
-   Reduced production risk
-   Better quality
-   Controlled releases

------------------------------------------------------------------------

# Types of Software Environments

Common environments:

1.  Development
2.  Testing
3.  Staging
4.  Production

------------------------------------------------------------------------

# 1. Development Environment

## Purpose

Used by developers to build and modify applications.

Activities:

-   Writing code
-   Debugging
-   Local testing

------------------------------------------------------------------------

## Characteristics

-   Frequent changes
-   Developer-controlled
-   Not customer-facing

Example:

    Developer Laptop

    +

    Local Database

------------------------------------------------------------------------

# 2. Testing Environment

## Purpose

Used by QA teams to verify application behavior.

Activities:

-   Functional testing
-   Integration testing
-   Bug detection

------------------------------------------------------------------------

## Characteristics

-   Stable compared to development
-   Contains test data
-   Used for quality validation

------------------------------------------------------------------------

# 3. Staging Environment

## Purpose

A production-like environment used for final validation.

It should closely match production.

------------------------------------------------------------------------

## Activities

-   Final testing
-   Performance testing
-   Release verification

------------------------------------------------------------------------

## Characteristics

Similar to production:

    Same:

    OS

    Database

    Configuration

    Infrastructure

------------------------------------------------------------------------

# 4. Production Environment

## Purpose

The live environment used by real users.

------------------------------------------------------------------------

## Characteristics

-   High availability
-   Strong security
-   Real customer data
-   Continuous monitoring

------------------------------------------------------------------------

# Environment Comparison

  Environment   Purpose                Users
  ------------- ---------------------- -------------------
  Development   Build features         Developers
  Testing       Verify functionality   QA Team
  Staging       Final validation       QA + Release Team
  Production    Real usage             Customers

------------------------------------------------------------------------

# Environment Promotion Flow

Software moves through environments.

Example:

    Developer Code

          ↓

    Development

          ↓

    Testing

          ↓

    Staging

          ↓

    Production

Each stage validates quality before moving forward.

------------------------------------------------------------------------

# Environment Differences Problem

A common problem:

    Works in Development

            ↓

    Fails in Production

Causes:

-   Different configurations
-   Different libraries
-   Different database versions
-   Different operating systems

------------------------------------------------------------------------

# Environment Consistency

DevOps aims to make environments similar.

Methods:

-   Containerization
-   Infrastructure as Code
-   Configuration management
-   Automated setup

Example:

    Development

    =

    Testing

    =

    Production

------------------------------------------------------------------------

# Configuration Management

Applications require different configurations.

Examples:

Development:

    Database = localhost

Production:

    Database = Cloud Server

Configuration should be managed separately from code.

------------------------------------------------------------------------

# Environment Variables

Sensitive values should not be hardcoded.

Bad:

    database_password = "12345"

Good:

    DATABASE_PASSWORD

            ↓

    Environment Variable

------------------------------------------------------------------------

# Environment Management Tools

## Docker

Provides consistent application environments.

Example:

    Application

    +

    Dependencies

    +

    Runtime

    =

    Container

------------------------------------------------------------------------

## Kubernetes

Manages containerized environments.

Provides:

-   Deployment
-   Scaling
-   Management

------------------------------------------------------------------------

## Terraform

Creates infrastructure automatically.

------------------------------------------------------------------------

## Ansible

Automates configuration management.

------------------------------------------------------------------------

# Environment Management in CI/CD

Typical workflow:

    Code Commit

          ↓

    Build

          ↓

    Deploy to Development

          ↓

    Test

          ↓

    Deploy to Staging

          ↓

    Approval

          ↓

    Production

------------------------------------------------------------------------

# Environment Management Best Practices

## 1. Keep Environments Similar

Avoid configuration differences.

------------------------------------------------------------------------

## 2. Automate Environment Setup

Use:

-   Containers
-   Infrastructure as Code

------------------------------------------------------------------------

## 3. Separate Configuration from Code

Use:

-   Environment variables
-   Configuration files

------------------------------------------------------------------------

## 4. Control Access

Example:

    Developer

    QA

    Production Admin

------------------------------------------------------------------------

## 5. Monitor Each Environment

Track:

-   Performance
-   Errors
-   Availability

------------------------------------------------------------------------

# Real-World Example

## Banking Application

Environments:

    Development

    Developer tests transaction feature


    Testing

    QA validates functionality


    Staging

    Security testing


    Production

    Customers use application

------------------------------------------------------------------------

# Common Environment Problems

## Problem 1

Different environments behave differently.

Solution:

Use containerization.

------------------------------------------------------------------------

## Problem 2

Configuration mistakes.

Solution:

Use configuration management tools.

------------------------------------------------------------------------

## Problem 3

Manual environment setup.

Solution:

Automate infrastructure creation.

------------------------------------------------------------------------

# Interview Questions

## 1. What is a software environment?

A software environment is the combination of resources required to run
an application.

------------------------------------------------------------------------

## 2. Why do we need multiple environments?

To safely develop, test, validate, and release applications.

------------------------------------------------------------------------

## 3. Difference between staging and production?

Staging is a production-like testing environment, while production
serves real users.

------------------------------------------------------------------------

## 4. Why should environments be consistent?

To avoid application failures caused by environment differences.

------------------------------------------------------------------------

## 5. How do DevOps teams manage environments?

Using:

-   Containers
-   Infrastructure as Code
-   Configuration management
-   Automation

------------------------------------------------------------------------

# Cheat Sheet

    Environment Management

    Development

          ↓

    Testing

          ↓

    Staging

          ↓

    Production

          ↓

    Users

------------------------------------------------------------------------

# Summary

Environment management ensures that software moves safely from
development to production. By maintaining consistent environments,
separating configurations, and automating setup, DevOps teams reduce
deployment failures and improve software reliability.

Proper environment management is essential for successful CI/CD
workflows.
