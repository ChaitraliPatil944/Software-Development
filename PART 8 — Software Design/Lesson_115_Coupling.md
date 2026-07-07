# Lesson 115 --- Coupling

# Part 8 --- Software Design

> **Objective**
>
> Understand Coupling in software design, why dependency management
> matters, types of coupling, tight vs loose coupling, and techniques
> used to create flexible and maintainable software systems.

------------------------------------------------------------------------

# Introduction

Software modules rarely work completely alone.

Modules communicate with each other, but the amount of dependency
between them affects software quality.

This dependency is called **Coupling**.

``` text
Module A

    ↓ depends on

Module B
```

The stronger the dependency, the harder the system becomes to change.

------------------------------------------------------------------------

# What is Coupling?

**Coupling** refers to the degree of dependency between software
modules.

It measures:

-   How strongly modules depend on each other
-   How much one module knows about another module

------------------------------------------------------------------------

# Why Do We Need to Understand Coupling?

High dependency creates problems:

``` text
Strong Dependency

        ↓

Small Change

        ↓

Multiple Modules Affected

        ↓

Maintenance Difficulty
```

Good software design aims for:

``` text
Low Coupling

        ↓

Flexible System

        ↓

Easy Maintenance
```

------------------------------------------------------------------------

# Types of Coupling

Coupling is commonly classified from strongest to weakest.

``` text
High Coupling

        ↓

Content Coupling

Common Coupling

Control Coupling

Stamp Coupling

Data Coupling

        ↓

Low Coupling
```

------------------------------------------------------------------------

# 1. Content Coupling

The highest and worst form of coupling.

One module directly accesses another module's internal data.

Example:

``` text
Module A

directly modifies

Module B internal variables
```

Problems:

-   Very difficult to maintain
-   Changes break other modules

------------------------------------------------------------------------

# 2. Common Coupling

Multiple modules share global data.

Example:

``` text
Global Variable

      ↓

Module A

Module B

Module C
```

Problem:

Any change to shared data affects many modules.

------------------------------------------------------------------------

# 3. Control Coupling

One module controls another using flags or commands.

Example:

``` text
processPayment(type)
```

Where:

    type = credit
    type = debit

Problem:

Modules know internal control logic.

------------------------------------------------------------------------

# 4. Stamp Coupling

Modules share complex data structures.

Example:

Passing an entire customer object when only email is needed.

``` text
Customer Object

Name
Email
Address
Phone
```

Only:

    Email

is required.

------------------------------------------------------------------------

# 5. Data Coupling

The best form of coupling.

Modules communicate only through required data.

Example:

``` text
Payment Service

receives:

amount
transactionId
```

Benefits:

-   Simple communication
-   Easy changes

------------------------------------------------------------------------

# Tight Coupling

## Definition

Modules are highly dependent on each other.

Example:

``` text
Class A

directly creates

Class B
```

------------------------------------------------------------------------

## Problems

-   Difficult testing
-   Difficult replacement
-   Hard maintenance
-   Low flexibility

------------------------------------------------------------------------

# Loose Coupling

## Definition

Modules interact through abstractions or interfaces.

Example:

``` text
Payment Interface

        |
----------------
|              |
Card Payment  UPI Payment
```

------------------------------------------------------------------------

## Benefits

-   Easy modification
-   Better scalability
-   Easier testing
-   Better reuse

------------------------------------------------------------------------

# Coupling and Modularity

Good modular design requires:

``` text
High Cohesion

        +

Low Coupling

        ↓

Better Software Design
```

------------------------------------------------------------------------

# Coupling Example

## Bad Design

``` text
Order Module

directly uses

Payment Database

directly uses

User Database
```

Changes become risky.

------------------------------------------------------------------------

# Better Design

``` text
Order Module

       ↓

Payment Interface

       ↓

Payment Service
```

Modules communicate through contracts.

------------------------------------------------------------------------

# Techniques to Reduce Coupling

## 1. Use Interfaces

Instead of depending on concrete classes.

Example:

``` text
Payment Interface

        ↓

Payment Implementation
```

------------------------------------------------------------------------

## 2. Dependency Injection

Provide dependencies from outside.

Example:

Instead of:

``` text
Class creates object
```

Use:

``` text
Object provided to class
```

------------------------------------------------------------------------

## 3. Encapsulation

Hide internal details.

------------------------------------------------------------------------

## 4. Modular Architecture

Separate responsibilities.

------------------------------------------------------------------------

## 5. API-Based Communication

Use defined contracts between systems.

------------------------------------------------------------------------

# Coupling in Different Architectures

## Monolithic System

Higher chance of tight coupling.

    Large Application

    All modules connected

------------------------------------------------------------------------

## Microservices System

Services communicate through APIs.

    User Service

          ↓ API

    Order Service

This promotes loose coupling.

------------------------------------------------------------------------

# Coupling vs Cohesion

  Coupling                     Cohesion
  ---------------------------- ----------------------------
  Dependency between modules   Relationship inside module
  Should be low                Should be high
  External focus               Internal focus

------------------------------------------------------------------------

# Industry Example

## E-Commerce System

Bad:

Order service directly accesses payment database.

Good:

    Order Service

          ↓

    Payment API

          ↓

    Payment Service

------------------------------------------------------------------------

# Common Mistakes

## Mistake 1

Creating modules that know too much about each other.

Solution:

Use clear interfaces.

------------------------------------------------------------------------

## Mistake 2

Sharing global data everywhere.

Solution:

Encapsulate data.

------------------------------------------------------------------------

## Mistake 3

Ignoring future changes.

Solution:

Design for flexibility.

------------------------------------------------------------------------

# Interview Questions

1.  What is Coupling?
2.  Why should coupling be low?
3.  Difference between tight and loose coupling?
4.  Explain types of coupling.
5.  What is data coupling?
6.  How can coupling be reduced?
7.  Relationship between coupling and cohesion?

------------------------------------------------------------------------

# Cheat Sheet

``` text
Good Software Design

High Cohesion

        +

Low Coupling

        ↓

Maintainable System
```

------------------------------------------------------------------------

# Summary

Coupling measures dependency between software modules. Good software
design minimizes coupling by creating independent modules that
communicate through clear interfaces. Loose coupling improves
flexibility, testing, scalability, and maintainability, making systems
easier to evolve over time.
