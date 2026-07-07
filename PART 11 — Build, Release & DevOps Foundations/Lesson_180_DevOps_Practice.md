# Lesson 180 --- DevOps Practice

# Part 11 --- DevOps

> **Objective**
>
> Practice DevOps concepts through hands-on exercises involving CI/CD
> pipelines, build and release workflows, deployment strategies,
> environment management, configuration management, Infrastructure as
> Code, monitoring, logging, and incident response scenarios.

------------------------------------------------------------------------

# Introduction

DevOps skills are developed through practical implementation.

Understanding concepts is important, but real DevOps requires working
with:

-   Code
-   Pipelines
-   Infrastructure
-   Monitoring
-   Production scenarios

``` text
Learn Concept

      ↓

Practice

      ↓

Automate

      ↓

Improve
```

------------------------------------------------------------------------

# Practice 1 --- Create DevOps Project Structure

## Task

Create a simple web application project.

Structure:

    devops-project

    ├── application

    ├── tests

    ├── docker

    ├── pipeline

    └── monitoring

------------------------------------------------------------------------

# Practice 2 --- Version Control Setup

## Task

Initialize Git repository.

Commands:

``` bash
git init
```

Add files:

``` bash
git add .
```

Create commit:

``` bash
git commit -m "Initial project setup"
```

------------------------------------------------------------------------

# Practice 3 --- Branching Workflow

Create branches:

    main

    develop

    feature-login

Commands:

``` bash
git checkout -b develop
```

Workflow:

    Feature Branch

          ↓

    Develop Branch

          ↓

    Main Branch

------------------------------------------------------------------------

# Practice 4 --- Create CI Pipeline

## Task

Create a pipeline that performs:

1.  Code checkout
2.  Build
3.  Testing
4.  Report generation

Pipeline:

    Code Push

          ↓

    CI Trigger

          ↓

    Build

          ↓

    Test

          ↓

    Result

------------------------------------------------------------------------

# Practice 5 --- Build Automation

## Task

Create automated build process.

Example:

Java:

``` bash
mvn clean package
```

Node.js:

``` bash
npm install

npm run build
```

------------------------------------------------------------------------

# Practice 6 --- Automated Testing

Create tests:

    Unit Tests

    Integration Tests

    Regression Tests

Expected workflow:

    Build

     ↓

    Tests

     ↓

    Success / Failure

------------------------------------------------------------------------

# Practice 7 --- Create Docker Container

## Task

Containerize application.

Docker workflow:

    Application

          ↓

    Dockerfile

          ↓

    Docker Image

          ↓

    Container

Example commands:

Build:

``` bash
docker build .
```

Run:

``` bash
docker run image_name
```

------------------------------------------------------------------------

# Practice 8 --- Environment Management

Create environments:

    Development

    Testing

    Staging

    Production

Task:

Maintain separate configurations.

Example:

Development:

    DATABASE=local

Production:

    DATABASE=cloud

------------------------------------------------------------------------

# Practice 9 --- Configuration Management

Create configuration file.

Example:

    application.yml

Store:

-   Database settings
-   Application settings
-   Environment values

------------------------------------------------------------------------

# Practice 10 --- Environment Variables

Create variables:

Example:

    DATABASE_URL

    API_KEY

    PORT

Access them from application.

------------------------------------------------------------------------

# Practice 11 --- Infrastructure as Code Practice

## Task

Create infrastructure definition.

Example:

Terraform workflow:

    Write Configuration

          ↓

    terraform init

          ↓

    terraform plan

          ↓

    terraform apply

------------------------------------------------------------------------

# Practice 12 --- Deployment Strategy Exercise

## Scenario

Release a new application version.

Choose deployment strategy.

Options:

-   Recreate
-   Rolling
-   Blue-Green
-   Canary

------------------------------------------------------------------------

## Example Solution

Large e-commerce application:

Use:

    Canary Deployment

Reason:

-   Low risk
-   Gradual rollout
-   Real user feedback

------------------------------------------------------------------------

# Practice 13 --- Monitoring Setup

## Task

Monitor application:

Track:

-   CPU
-   Memory
-   Response time
-   Errors

Workflow:

    Application

          ↓

    Metrics

          ↓

    Dashboard

          ↓

    Alerts

------------------------------------------------------------------------

# Practice 14 --- Logging Practice

Create logs:

Example:

    INFO User login successful

    ERROR Database connection failed

Analyze:

-   Errors
-   Patterns
-   Failures

------------------------------------------------------------------------

# Practice 15 --- Incident Response Practice

## Scenario

Production API is unavailable.

------------------------------------------------------------------------

## Response Process

    Alert

     ↓

    Create Incident

     ↓

    Investigate

     ↓

    Fix

     ↓

    Verify

     ↓

    RCA

------------------------------------------------------------------------

# Practice 16 --- Root Cause Analysis

Scenario:

Website crashed.

Find root cause.

Use:

## Five Whys

Example:

Why?

    Website crashed

Why?

    Server overloaded

Why?

    Traffic increased

Why?

    No auto scaling

Root cause:

    Missing scaling configuration

------------------------------------------------------------------------

# Practice 17 --- CI/CD Pipeline Design

Design pipeline:

    Developer

     ↓

    Git Repository

     ↓

    CI Build

     ↓

    Automated Tests

     ↓

    Artifact

     ↓

    CD Deployment

     ↓

    Monitoring

------------------------------------------------------------------------

# Practice 18 --- Real-World Project

## Project

Deploy an E-Commerce Application.

Requirements:

-   Git workflow
-   CI pipeline
-   Docker container
-   Environment setup
-   Automated deployment
-   Monitoring
-   Logging
-   Incident handling

------------------------------------------------------------------------

# Project Workflow

    Code

     ↓

    Git

     ↓

    CI Pipeline

     ↓

    Docker Build

     ↓

    Deploy

     ↓

    Monitor

     ↓

    Improve

------------------------------------------------------------------------

# Practice Questions

## Q1. Design a CI/CD pipeline.

Answer:

    Commit

    ↓

    Build

    ↓

    Test

    ↓

    Artifact

    ↓

    Deploy

    ↓

    Monitor

------------------------------------------------------------------------

## Q2. Production deployment failed. What will you do?

Answer:

1.  Check alerts
2.  Analyze logs
3.  Rollback if required
4.  Fix issue
5.  Perform RCA

------------------------------------------------------------------------

## Q3. Application works locally but fails in production.

Possible causes:

-   Configuration mismatch
-   Dependency difference
-   Environment issue

Solutions:

-   Docker
-   Configuration management
-   Environment consistency

------------------------------------------------------------------------

# DevOps Practice Checklist

✓ Git workflow practiced

✓ CI pipeline created

✓ Build automation understood

✓ Testing automated

✓ Docker container created

✓ Environment management practiced

✓ Configuration handled

✓ IaC concepts practiced

✓ Deployment strategies understood

✓ Monitoring configured

✓ Logs analyzed

✓ Incident response practiced

------------------------------------------------------------------------

# Summary

DevOps practice requires combining development, automation,
infrastructure, deployment, and monitoring skills. By practicing
complete workflows from code commit to production monitoring, engineers
gain the ability to build reliable and scalable software delivery
systems.
