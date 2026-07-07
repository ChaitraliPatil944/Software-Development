# Lesson 116 --- Cohesion

# Part 8 --- Software Design

> **Objective**
>
> Understand Cohesion in software design, why highly focused modules are
> important, types of cohesion, high vs low cohesion, and how cohesion
> improves software maintainability.

------------------------------------------------------------------------

# Introduction

A good software module should have a clear purpose.

All elements inside a module should work together toward a common goal.

This internal relationship is called **Cohesion**.

``` text
Module

 ├── Component A
 ├── Component B
 └── Component C

All support one responsibility
```

------------------------------------------------------------------------

# What is Cohesion?

**Cohesion** refers to the degree to which elements inside a software
module belong together.

It measures:

-   How focused a module is
-   Whether its responsibilities are related
-   How well its components work together

------------------------------------------------------------------------

# Why Do We Need High Cohesion?

Low cohesion creates problems:

``` text
One Module

Handles Many Unrelated Tasks

        ↓

Complex Code

        ↓

Hard Maintenance
```

High cohesion provides:

-   Better readability
-   Easier testing
-   Easier maintenance
-   Better reusability
-   Improved understanding

------------------------------------------------------------------------

# High Cohesion

A module has high cohesion when it performs one specific responsibility.

Example:

    Payment Module

    Handles:

    ✓ Payment Processing

    ✓ Transaction Validation

    ✓ Payment Confirmation

All functions are related.

------------------------------------------------------------------------

# Low Cohesion

A module has low cohesion when it handles unrelated responsibilities.

Example:

    User Module

    Handles:

    - Login
    - Payment
    - Report Generation
    - Email Sending

Problems:

-   Difficult to modify
-   Hard to test
-   Poor design

------------------------------------------------------------------------

# Types of Cohesion

Cohesion levels are classified from lowest to highest.

``` text
Low Cohesion

        ↓

Coincidental

Logical

Temporal

Procedural

Communicational

Sequential

Functional

        ↓

High Cohesion
```

------------------------------------------------------------------------

# 1. Coincidental Cohesion

Lowest level of cohesion.

Unrelated tasks are placed together.

Example:

    Utility Class

    contains:

    Login()
    CalculateTax()
    PrintReport()

Problems:

-   No clear purpose
-   Difficult maintenance

------------------------------------------------------------------------

# 2. Logical Cohesion

Similar categories of tasks are grouped.

Example:

    Input Handler

    handles:

    Keyboard Input

    Mouse Input

    File Input

Problem:

Responsibilities are still different.

------------------------------------------------------------------------

# 3. Temporal Cohesion

Tasks are grouped because they happen at the same time.

Example:

Startup Module:

    Load Configuration

    Initialize Database

    Create Logs

------------------------------------------------------------------------

# 4. Procedural Cohesion

Tasks are grouped because they follow a sequence.

Example:

    Process Order:

    Validate User

    Check Stock

    Create Order

------------------------------------------------------------------------

# 5. Communicational Cohesion

Tasks operate on the same data.

Example:

Customer Module:

    Update Customer

    View Customer

    Delete Customer

All use customer data.

------------------------------------------------------------------------

# 6. Sequential Cohesion

Output of one operation becomes input of another.

Example:

    Read Data

          ↓

    Process Data

          ↓

    Generate Report

------------------------------------------------------------------------

# 7. Functional Cohesion

Highest level of cohesion.

A module performs one specific function.

Example:

    Payment Processing Module

Only handles payment.

------------------------------------------------------------------------

# Cohesion and Coupling Relationship

Good software design follows:

``` text
High Cohesion

        +

Low Coupling

        ↓

Quality Software
```

------------------------------------------------------------------------

# Cohesion Example

## Bad Design

    Common Module

    Login

    Payment

    Reports

    Email

Low cohesion.

------------------------------------------------------------------------

## Better Design

    Authentication Module

    Payment Module

    Report Module

    Notification Module

High cohesion.

------------------------------------------------------------------------

# Cohesion in Object-Oriented Design

Classes should have:

-   One responsibility
-   Related methods
-   Clear purpose

This connects with:

**Single Responsibility Principle (SRP)**

from SOLID principles.

------------------------------------------------------------------------

# Cohesion and SOLID

Example:

Bad:

    Employee Class

    calculateSalary()

    saveEmployee()

    sendEmail()

Too many responsibilities.

------------------------------------------------------------------------

Better:

    Employee Class

            ↓

    Salary Service

            ↓

    Employee Repository

            ↓

    Email Service

------------------------------------------------------------------------

# Industry Example

## Banking System

Good module design:

    Account Module

    Handles:

    - Account Creation
    - Account Update
    - Account Details

    Transaction Module

    Handles:

    - Transfer
    - Deposit
    - Withdrawal

Each module has a focused responsibility.

------------------------------------------------------------------------

# Common Mistakes

## Mistake 1

Creating "God Classes".

Solution:

Split responsibilities.

------------------------------------------------------------------------

## Mistake 2

Mixing unrelated features.

Solution:

Create separate modules.

------------------------------------------------------------------------

## Mistake 3

Ignoring design principles.

Solution:

Follow SOLID and modular design.

------------------------------------------------------------------------

# Best Practices

-   Give each module one clear purpose
-   Keep related functionality together
-   Avoid unnecessary responsibilities
-   Combine with low coupling
-   Review module boundaries regularly

------------------------------------------------------------------------

# Interview Questions

1.  What is Cohesion?
2.  Why is high cohesion preferred?
3.  Difference between cohesion and coupling?
4.  Explain types of cohesion.
5.  Which type of cohesion is best?
6.  How does cohesion improve maintainability?
7.  Explain cohesion with an example.

------------------------------------------------------------------------

# Cheat Sheet

``` text
Good Module

One Responsibility

        ↓

Related Components

        ↓

High Cohesion

        +

Low Coupling

        ↓

Better Design
```

------------------------------------------------------------------------

# Summary

Cohesion measures how closely related the responsibilities inside a
module are. High cohesion creates focused, understandable, and
maintainable components. Combined with low coupling, high cohesion is a
fundamental principle of good software design and helps teams build
flexible and scalable systems.
