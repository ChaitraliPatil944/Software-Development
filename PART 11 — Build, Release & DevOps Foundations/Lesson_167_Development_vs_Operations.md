# Lesson 167 --- Development vs Operations

# Part 11 --- DevOps

> **Objective**
>
> Understand the differences between Development and Operations teams,
> their responsibilities, traditional conflicts, how DevOps bridges the
> gap, collaboration models, shared responsibilities, and modern
> software delivery practices.

------------------------------------------------------------------------

# Introduction

Software delivery involves multiple teams.

Two important teams are:

    Development

            +

    Operations

Traditionally, these teams had different goals.

DevOps was created to bring them together.

------------------------------------------------------------------------

# What is Development?

**Development (Dev)** is the team responsible for designing, building,
and improving software applications.

Developers focus on:

-   Writing code
-   Creating features
-   Fixing bugs
-   Improving application logic

------------------------------------------------------------------------

# Development Responsibilities

## 1. Requirement Understanding

Developers analyze:

-   Business requirements
-   User needs
-   Technical requirements

------------------------------------------------------------------------

## 2. Software Design

Developers decide:

-   Application structure
-   Data flow
-   Components

------------------------------------------------------------------------

## 3. Coding

Main activities:

-   Writing source code
-   Implementing features
-   Creating APIs

------------------------------------------------------------------------

## 4. Testing

Developers perform:

-   Unit testing
-   Integration testing
-   Debugging

------------------------------------------------------------------------

## 5. Version Control

Developers use tools like:

-   Git
-   GitHub
-   GitLab

to manage code changes.

------------------------------------------------------------------------

# What is Operations?

**Operations (Ops)** is the team responsible for deploying, managing,
maintaining, and monitoring software systems.

Operations focus on:

-   Infrastructure
-   Deployment
-   Reliability
-   Availability

------------------------------------------------------------------------

# Operations Responsibilities

## 1. Infrastructure Management

Managing:

-   Servers
-   Networks
-   Databases
-   Cloud resources

------------------------------------------------------------------------

## 2. Deployment

Operations handle:

-   Application releases
-   Production deployment
-   Rollbacks

------------------------------------------------------------------------

## 3. System Monitoring

Monitoring:

-   Performance
-   Availability
-   Errors

------------------------------------------------------------------------

## 4. Security Management

Managing:

-   Access control
-   Security policies
-   Compliance

------------------------------------------------------------------------

## 5. Incident Response

Handling:

-   System failures
-   Outages
-   Production issues

------------------------------------------------------------------------

# Traditional Development and Operations Model

Before DevOps:

    Developer

       Writes Code

            ↓

    Operations

       Deploys Code

Teams worked separately.

------------------------------------------------------------------------

# Problems Between Dev and Ops

## Problem 1 --- Different Goals

Development:

    Release Features Quickly

Operations:

    Keep System Stable

Conflict:

    Speed vs Stability

------------------------------------------------------------------------

# Problem 2 --- Poor Communication

Developers may not understand:

-   Production environment
-   Infrastructure limitations

Operations may not understand:

-   Application design
-   Code changes

------------------------------------------------------------------------

# Problem 3 --- Deployment Issues

Developers:

    "It works on my machine"

Operations:

    "Production behaves differently"

------------------------------------------------------------------------

# Problem 4 --- Responsibility Gap

When problems occurred:

Development:

    Infrastructure issue

Operations:

    Application issue

No shared ownership existed.

------------------------------------------------------------------------

# DevOps Solution

DevOps combines Dev and Ops into a collaborative approach.

Before:

    Development

          X

    Operations

After:

    Development

          +

    Operations

          ↓

    DevOps Culture

------------------------------------------------------------------------

# Shared Responsibilities in DevOps

Modern teams share responsibility for:

-   Code quality
-   Deployment
-   Monitoring
-   Security
-   Reliability

------------------------------------------------------------------------

# DevOps Team Model

A DevOps team includes:

    Developers

         +

    Operations Engineers

         +

    QA Engineers

         +

    Security Engineers

         +

    Cloud Engineers

------------------------------------------------------------------------

# Development vs Operations Comparison

  Development              Operations
  ------------------------ ------------------------
  Builds software          Runs software
  Writes code              Manages infrastructure
  Creates features         Maintains availability
  Fixes application bugs   Handles system issues
  Focuses on delivery      Focuses on reliability

------------------------------------------------------------------------

# DevOps Responsibilities

DevOps combines both areas:

## Development Side

-   Code management
-   Automated testing
-   Application design

## Operations Side

-   Deployment automation
-   Infrastructure management
-   Monitoring

------------------------------------------------------------------------

# DevOps Collaboration Workflow

Modern workflow:

    Developer

     ↓

    Git Repository

     ↓

    CI Pipeline

     ↓

    Testing

     ↓

    Deployment

     ↓

    Operations Monitoring

     ↓

    Feedback

     ↓

    Development Improvement

------------------------------------------------------------------------

# Example: New Feature Release

## Traditional Approach

    Developer Creates Feature

            ↓

    Testing Team

            ↓

    Operations Team

            ↓

    Manual Deployment

------------------------------------------------------------------------

## DevOps Approach

    Developer

            ↓

    Automated Build

            ↓

    Automated Tests

            ↓

    Deployment Pipeline

            ↓

    Monitoring

------------------------------------------------------------------------

# Benefits of Dev and Ops Collaboration

## Faster Delivery

Teams release features quickly.

------------------------------------------------------------------------

## Better Stability

Operations knowledge improves development decisions.

------------------------------------------------------------------------

## Faster Problem Resolution

Teams solve issues together.

------------------------------------------------------------------------

## Improved Communication

Everyone understands the complete lifecycle.

------------------------------------------------------------------------

# DevOps Culture Changes

Old mindset:

    My Code

    Your Problem

New mindset:

    Our Application

    Our Responsibility

------------------------------------------------------------------------

# Interview Questions

## 1. Difference between Development and Operations?

Development creates and improves software, while Operations deploys,
manages, and maintains software systems.

------------------------------------------------------------------------

## 2. Why did DevOps combine Dev and Ops?

To improve collaboration, automate processes, and deliver software
faster with better reliability.

------------------------------------------------------------------------

## 3. What conflicts existed between Dev and Ops?

Common conflicts:

-   Speed vs stability
-   Poor communication
-   Deployment responsibility issues

------------------------------------------------------------------------

## 4. What is shared responsibility in DevOps?

All teams are responsible for software quality, deployment, monitoring,
and reliability.

------------------------------------------------------------------------

# Cheat Sheet

``` text
Traditional Model

Development

      ↓

Operations


DevOps Model

Development

      +

Operations

      ↓

Collaboration

      ↓

Reliable Delivery
```

------------------------------------------------------------------------

# Summary

Development focuses on building software, while Operations focuses on
running and maintaining software systems. Traditional separation created
communication gaps and deployment problems. DevOps bridges this gap by
creating collaboration, automation, shared responsibility, and
continuous software delivery.

Understanding the difference between Dev and Ops is the foundation for
learning CI/CD, automation, cloud, monitoring, and modern software
engineering practices.
