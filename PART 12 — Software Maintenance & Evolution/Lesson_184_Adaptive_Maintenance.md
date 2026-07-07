# Lesson 184 --- Adaptive Maintenance

# Part 12 --- Software Maintenance

> **Objective**
>
> Understand Adaptive Maintenance, why software needs adaptation,
> environmental changes, platform migration, technology upgrades, cloud
> migration, adaptive maintenance process, challenges, best practices,
> and its role in software evolution.

------------------------------------------------------------------------

# Introduction

Software does not run in a fixed environment forever.

Over time, changes occur:

-   New operating systems
-   New hardware
-   New browsers
-   New databases
-   New business regulations
-   Cloud adoption

Software must adapt to these changes.

This process is called **Adaptive Maintenance**.

``` text
Environment Change

        ↓

Software Modification

        ↓

Compatible System
```

------------------------------------------------------------------------

# What is Adaptive Maintenance?

**Adaptive Maintenance** is the process of modifying software to keep it
compatible with changes in its environment.

Simple definition:

    Adaptive Maintenance = Changing Software for a New Environment

------------------------------------------------------------------------

# Why is Adaptive Maintenance Needed?

Software environments continuously evolve.

Examples:

-   Operating system upgrades
-   Database version changes
-   Hardware replacement
-   Cloud migration
-   Third-party API changes

Without adaptation:

    Environment Changes

            ↓

    Software Failure

            ↓

    System Becomes Outdated

------------------------------------------------------------------------

# Examples of Adaptive Maintenance

## Example 1 --- Operating System Upgrade

Old:

    Windows 10

New:

    Windows 11

Software may require updates to work correctly.

------------------------------------------------------------------------

## Example 2 --- Database Migration

Old:

    MySQL 5

New:

    MySQL 8

Application queries may need modification.

------------------------------------------------------------------------

## Example 3 --- Cloud Migration

Before:

    On-Premise Server

            ↓

    Cloud Infrastructure

Software must adapt to cloud services.

------------------------------------------------------------------------

## Example 4 --- Browser Compatibility

Example:

    Old Browser Version

            ↓

    New Browser Standards

Frontend code may need updates.

------------------------------------------------------------------------

# Adaptive Maintenance Process

``` text
Identify Environmental Change

        ↓

Analyze Impact

        ↓

Modify Software

        ↓

Test Compatibility

        ↓

Deploy Update

        ↓

Monitor System
```

------------------------------------------------------------------------

# Step 1 --- Identify Change

Changes are detected from:

-   Technology updates
-   Business requirements
-   Vendor changes
-   Security requirements

Example:

    Database Version End of Support

------------------------------------------------------------------------

# Step 2 --- Impact Analysis

Teams analyze:

-   Affected components
-   Required modifications
-   Possible risks

------------------------------------------------------------------------

# Step 3 --- Software Modification

Developers update:

-   Code
-   Configuration
-   Dependencies
-   Infrastructure

------------------------------------------------------------------------

# Step 4 --- Testing

Testing ensures compatibility.

Types:

-   Integration testing
-   Compatibility testing
-   Regression testing

------------------------------------------------------------------------

# Step 5 --- Deployment

Updated software is released.

Process:

    Update

     ↓

    Test

     ↓

    Deploy

     ↓

    Monitor

------------------------------------------------------------------------

# Adaptive Maintenance vs Corrective Maintenance

  Adaptive                        Corrective
  ------------------------------- ------------------------
  Handles environment changes     Fixes existing defects
  Proactive                       Reactive
  Triggered by external changes   Triggered by failures

------------------------------------------------------------------------

# Adaptive Maintenance vs Perfective Maintenance

  Adaptive                     Perfective
  ---------------------------- -------------------
  Changes due to environment   Improves features
  Compatibility focus          Enhancement focus

------------------------------------------------------------------------

# Common Areas of Adaptive Maintenance

## 1. Platform Changes

Examples:

-   Operating systems
-   Hardware
-   Browsers

------------------------------------------------------------------------

## 2. Database Changes

Examples:

-   Database upgrades
-   Schema changes

------------------------------------------------------------------------

## 3. Infrastructure Changes

Examples:

-   Server migration
-   Cloud adoption

------------------------------------------------------------------------

## 4. External Service Changes

Examples:

-   API changes
-   Payment gateway updates

------------------------------------------------------------------------

# Challenges in Adaptive Maintenance

## 1. Compatibility Issues

New environments may behave differently.

------------------------------------------------------------------------

## 2. Legacy Software

Old systems may not support modern technologies.

------------------------------------------------------------------------

## 3. Testing Complexity

Changes can affect existing functionality.

------------------------------------------------------------------------

## 4. Cost and Time

Large migrations require significant resources.

------------------------------------------------------------------------

# Adaptive Maintenance Best Practices

## 1. Monitor Technology Changes

Stay updated with platforms and dependencies.

------------------------------------------------------------------------

## 2. Use Modular Design

Modular systems are easier to adapt.

------------------------------------------------------------------------

## 3. Maintain Documentation

Helps understand existing systems.

------------------------------------------------------------------------

## 4. Automate Testing

Ensures safe modifications.

------------------------------------------------------------------------

## 5. Plan Migration Carefully

Analyze risks before major changes.

------------------------------------------------------------------------

# Adaptive Maintenance in SDLC

``` text
Development

      ↓

Deployment

      ↓

Environment Change

      ↓

Adaptive Maintenance

      ↓

Updated Software
```

------------------------------------------------------------------------

# Real-World Example

## Banking System Migration

Scenario:

Bank moves from on-premise servers to cloud.

Old:

    Local Servers

    Database

    Application

New:

    Cloud Servers

    Managed Database

    Cloud Services

Adaptive maintenance activities:

-   Update configurations
-   Modify infrastructure
-   Test application
-   Deploy cloud version

------------------------------------------------------------------------

# Tools Used

Common tools:

-   Docker
-   Kubernetes
-   Terraform
-   Ansible
-   Cloud migration tools

------------------------------------------------------------------------

# Interview Questions

## 1. What is Adaptive Maintenance?

Adaptive Maintenance modifies software to remain compatible with changes
in its environment.

------------------------------------------------------------------------

## 2. Give examples of adaptive maintenance.

Examples:

-   Operating system upgrade
-   Database migration
-   Cloud migration
-   API changes

------------------------------------------------------------------------

## 3. Difference between adaptive and corrective maintenance?

Adaptive handles environmental changes.

Corrective fixes existing defects.

------------------------------------------------------------------------

## 4. Why is adaptive maintenance important?

It keeps software useful and compatible with evolving technology.

------------------------------------------------------------------------

## 5. What challenges occur during adaptive maintenance?

Challenges include:

-   Compatibility issues
-   Legacy systems
-   Testing complexity
-   Migration cost

------------------------------------------------------------------------

# Cheat Sheet

``` text
Adaptive Maintenance

Environment Change

        ↓

Analyze Impact

        ↓

Modify Software

        ↓

Test

        ↓

Deploy

        ↓

Compatible System
```

------------------------------------------------------------------------

# Summary

Adaptive Maintenance ensures software continues to work when its
environment changes. It allows systems to survive technology evolution,
platform upgrades, infrastructure changes, and business requirements.

Without adaptive maintenance, software gradually becomes outdated and
difficult to use.
