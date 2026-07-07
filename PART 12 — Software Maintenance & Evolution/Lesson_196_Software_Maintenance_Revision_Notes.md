# Lesson 196 --- Software Maintenance Revision Notes

# Part 12 --- Software Maintenance

> **Objective**
>
> Revise complete software maintenance concepts including maintenance
> types, legacy systems, technical debt, refactoring, documentation,
> change management, versioning, release management, interview concepts,
> and practical workflows.

------------------------------------------------------------------------

# 1. Software Maintenance Overview

## What is Software Maintenance?

Software Maintenance is the process of modifying, updating, improving,
and managing software after deployment.

It includes:

-   Bug fixing
-   Feature improvements
-   Security updates
-   Environment adaptation
-   Performance improvements

------------------------------------------------------------------------

# Why Software Maintenance is Needed

Software changes because of:

-   New business requirements
-   User feedback
-   Technology evolution
-   Security threats
-   Platform changes

Without maintenance:

    Old Software

          ↓

    Performance Issues

          ↓

    System Failure

------------------------------------------------------------------------

# Software Maintenance Lifecycle

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

------------------------------------------------------------------------

# 2. Types of Software Maintenance

There are four major types:

    Corrective

    Adaptive

    Perfective

    Preventive

------------------------------------------------------------------------

# Corrective Maintenance

## Purpose

Fix existing defects after deployment.

Examples:

-   Bug fixes
-   Application crashes
-   Incorrect calculations

Workflow:

    Bug Found

     ↓

    Analyze

     ↓

    Fix

     ↓

    Test

     ↓

    Deploy

------------------------------------------------------------------------

# Adaptive Maintenance

## Purpose

Modify software according to environmental changes.

Examples:

-   Operating system upgrades
-   Database migration
-   Cloud migration
-   API changes

Workflow:

    Environment Change

     ↓

    Modify Software

     ↓

    Test Compatibility

     ↓

    Deploy

------------------------------------------------------------------------

# Perfective Maintenance

## Purpose

Improve existing software features and performance.

Examples:

-   UI improvements
-   Performance optimization
-   New features

Workflow:

    User Feedback

     ↓

    Improvement

     ↓

    Testing

     ↓

    Release

------------------------------------------------------------------------

# Preventive Maintenance

## Purpose

Prevent future problems.

Examples:

-   Refactoring
-   Dependency updates
-   Security improvements
-   Documentation updates

Workflow:

    Identify Risks

     ↓

    Improve System

     ↓

    Prevent Failures

------------------------------------------------------------------------

# Maintenance Types Comparison

  Type         Purpose                      Example
  ------------ ---------------------------- -----------------
  Corrective   Fix defects                  Bug fix
  Adaptive     Handle environment changes   Cloud migration
  Perfective   Improve features             Better UI
  Preventive   Avoid future issues          Refactoring

------------------------------------------------------------------------

# 3. Legacy Systems

## Definition

A legacy system is an old software system still used by an organization
despite outdated technology.

------------------------------------------------------------------------

# Why Legacy Systems Exist

Reasons:

-   Important business logic
-   High replacement cost
-   Migration risks
-   Business dependency

------------------------------------------------------------------------

# Legacy Challenges

-   Difficult maintenance
-   Security vulnerabilities
-   Poor documentation
-   Integration problems
-   Limited scalability

------------------------------------------------------------------------

# Legacy Modernization Strategies

## Rehosting

Move system to new infrastructure.

Example:

    Server → Cloud

------------------------------------------------------------------------

## Replatforming

Move to new platform with small changes.

------------------------------------------------------------------------

## Refactoring

Improve internal code structure.

------------------------------------------------------------------------

## Reengineering

Redesign system using modern architecture.

------------------------------------------------------------------------

## Replacement

Replace old system completely.

------------------------------------------------------------------------

# 4. Technical Debt

## Definition

Technical debt is the future maintenance cost created by choosing quick
solutions over better long-term solutions.

    Shortcut

     ↓

    Future Cost

     ↓

    Technical Debt

------------------------------------------------------------------------

# Causes of Technical Debt

-   Tight deadlines
-   Poor architecture
-   Lack of testing
-   Missing documentation
-   Outdated dependencies

------------------------------------------------------------------------

# Types of Technical Debt

## Code Debt

Poor code quality.

## Design Debt

Poor architecture decisions.

## Testing Debt

Insufficient testing.

## Documentation Debt

Missing information.

## Infrastructure Debt

Outdated infrastructure.

------------------------------------------------------------------------

# Reducing Technical Debt

Methods:

-   Refactoring
-   Automated testing
-   Documentation improvement
-   Dependency updates
-   Architecture improvements

------------------------------------------------------------------------

# 5. Refactoring

## Definition

Refactoring improves internal code structure without changing external
behavior.

------------------------------------------------------------------------

# Goals of Refactoring

-   Better readability
-   Easier maintenance
-   Reduced technical debt
-   Improved testing
-   Better design

------------------------------------------------------------------------

# Code Smells

Indicators of poor code:

-   Duplicate code
-   Long methods
-   Large classes
-   Complex conditions
-   Poor naming

------------------------------------------------------------------------

# Common Refactoring Techniques

-   Extract Method
-   Rename Variables
-   Remove Duplicate Code
-   Extract Class
-   Simplify Conditions

------------------------------------------------------------------------

# Refactoring vs Rewriting

  Refactoring              Rewriting
  ------------------------ ---------------------
  Improves existing code   Creates new system
  Lower risk               Higher risk
  Keeps behavior           May change behavior

------------------------------------------------------------------------

# 6. Software Documentation

## Definition

Documentation explains software design, usage, development, and
maintenance.

------------------------------------------------------------------------

# Types of Documentation

## Technical Documentation

Examples:

-   Architecture documents
-   Code documentation
-   Database documentation
-   API documentation

------------------------------------------------------------------------

## User Documentation

Examples:

-   User manuals
-   Tutorials
-   FAQs

------------------------------------------------------------------------

## Process Documentation

Examples:

-   Development process
-   Deployment process

------------------------------------------------------------------------

# Documentation Best Practices

-   Keep updated
-   Write clearly
-   Include examples
-   Use version control
-   Maintain regularly

------------------------------------------------------------------------

# 7. Change Management

## Definition

Change Management controls software modifications through planning,
approval, implementation, and tracking.

------------------------------------------------------------------------

# Change Management Process

    Change Request

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

------------------------------------------------------------------------

# Change Control Board (CCB)

Responsible for:

-   Reviewing changes
-   Evaluating risks
-   Approving modifications
-   Maintaining records

------------------------------------------------------------------------

# Change Management Best Practices

-   Document changes
-   Analyze impact
-   Automate testing
-   Maintain rollback plans
-   Use version control

------------------------------------------------------------------------

# 8. Versioning

## Definition

Versioning assigns identifiers to software releases.

------------------------------------------------------------------------

# Semantic Versioning

Format:

    MAJOR.MINOR.PATCH

Example:

    2.5.1

------------------------------------------------------------------------

# Version Types

## Major

Breaking changes.

Example:

    3.0.0

------------------------------------------------------------------------

## Minor

New features.

Example:

    3.1.0

------------------------------------------------------------------------

## Patch

Bug fixes.

Example:

    3.1.1

------------------------------------------------------------------------

# 9. Release Management

## Definition

Release Management plans, coordinates, tests, and delivers software
releases.

------------------------------------------------------------------------

# Release Lifecycle

    Planning

     ↓

    Development

     ↓

    Testing

     ↓

    Approval

     ↓

    Deployment

     ↓

    Monitoring

------------------------------------------------------------------------

# Release Types

-   Major Release
-   Minor Release
-   Patch Release
-   Emergency Release

------------------------------------------------------------------------

# Release Strategies

## Rolling Release

Gradual update.

## Blue-Green Release

Switch between two environments.

## Canary Release

Small user rollout first.

## Big Bang Release

Complete release at once.

------------------------------------------------------------------------

# 10. Maintenance Workflow

Complete workflow:

    Problem

     ↓

    Identify Maintenance Type

     ↓

    Analyze Impact

     ↓

    Implement Change

     ↓

    Test

     ↓

    Release

     ↓

    Monitor

     ↓

    Improve

------------------------------------------------------------------------

# Interview Quick Notes

## What are four maintenance types?

-   Corrective
-   Adaptive
-   Perfective
-   Preventive

------------------------------------------------------------------------

## What is technical debt?

Future maintenance cost caused by shortcuts.

------------------------------------------------------------------------

## What is refactoring?

Improving code structure without changing behavior.

------------------------------------------------------------------------

## Why is documentation important?

It preserves knowledge and improves maintenance.

------------------------------------------------------------------------

## Why is change management required?

To safely control software modifications.

------------------------------------------------------------------------

# Final Revision Checklist

✓ Software Maintenance concepts

✓ Maintenance lifecycle

✓ Four maintenance types

✓ Legacy systems

✓ Modernization strategies

✓ Technical debt

✓ Refactoring

✓ Documentation

✓ Change management

✓ Versioning

✓ Release management

✓ Interview preparation

✓ Practical workflows

------------------------------------------------------------------------

# Summary

Software Maintenance ensures that software remains reliable, secure, and
useful after deployment. It includes fixing defects, adapting to
changes, improving features, preventing future problems, managing
changes, and delivering controlled releases.

A successful software engineer understands not only how to build
software but also how to maintain and evolve it throughout its
lifecycle.
