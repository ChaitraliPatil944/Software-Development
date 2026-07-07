# Lesson 113 --- Low Level Design (LLD)

# Part 8 --- Software Design

> **Objective**
>
> Understand Low Level Design (LLD), why it is required after HLD, how
> it defines detailed implementation structure, classes, objects,
> database details, APIs, and how it helps developers write maintainable
> code.

------------------------------------------------------------------------

# Introduction

High Level Design explains:

**What are the major system components?**

Low Level Design explains:

**How will each component be implemented?**

``` text
Requirements

      ↓

Architecture

      ↓

HLD

      ↓

LLD

      ↓

Code Implementation
```

------------------------------------------------------------------------

# What is Low Level Design?

**Low Level Design (LLD)** describes the detailed internal design of
software components.

It focuses on:

-   Classes
-   Objects
-   Methods
-   Interfaces
-   Database structures
-   Algorithms
-   Component interactions

LLD acts as a blueprint for developers.

------------------------------------------------------------------------

# Why Do We Need LLD?

Without LLD:

``` text
Developers Start Coding

        ↓

Different Design Decisions

        ↓

Inconsistent Code

        ↓

Maintenance Problems
```

LLD helps:

-   Reduce coding confusion
-   Improve code quality
-   Define responsibilities
-   Support teamwork
-   Make implementation predictable

------------------------------------------------------------------------

# LLD in Software Development

``` text
High Level Design

        ↓

Low Level Design

        ↓

Programming

        ↓

Testing
```

------------------------------------------------------------------------

# Components of LLD

A typical LLD contains:

``` text
Low Level Design

        |
--------------------------------
|        |        |             |
Classes  APIs   Database    Algorithms
```

------------------------------------------------------------------------

# 1. Class Design

LLD defines classes and their responsibilities.

Example:

## Banking System

    +----------------+
    | Customer       |
    +----------------+
    | customerId     |
    | name           |
    | email          |
    +----------------+
    | login()        |
    | updateProfile()|
    +----------------+

------------------------------------------------------------------------

# 2. Object Relationships

LLD defines how objects interact.

Example:

``` text
Customer

    |

    owns

    |

Account
```

------------------------------------------------------------------------

# 3. Database Design

LLD includes detailed database structures.

Example:

Customer Table:

    Customer

    customer_id
    name
    email
    password

Account Table:

    Account

    account_id
    customer_id
    balance

------------------------------------------------------------------------

# 4. API Design

LLD defines API details.

Example:

Login API:

    POST /login

Input:

``` json
{
 "email":"user@gmail.com",
 "password":"12345"
}
```

Output:

``` json
{
 "token":"abc123"
}
```

------------------------------------------------------------------------

# 5. Algorithm Design

LLD may define logic steps.

Example:

Money Transfer:

``` text
Check Balance

        ↓

Validate Receiver

        ↓

Transfer Amount

        ↓

Update Transaction
```

------------------------------------------------------------------------

# LLD Example

## Online Shopping System

Classes:

    User

    Product

    Cart

    Order

    Payment

Relationships:

    User

     ↓

    Cart

     ↓

    Order

     ↓

    Payment

------------------------------------------------------------------------

# HLD vs LLD

  HLD                    LLD
  ---------------------- -------------------------
  System overview        Detailed implementation
  Architecture focused   Code focused
  Components             Classes and methods
  Created before LLD     Created before coding

------------------------------------------------------------------------

# LLD and Object-Oriented Design

LLD heavily uses OOP concepts:

## Classes

Blueprint of objects.

## Objects

Instances of classes.

## Encapsulation

Hide internal details.

## Inheritance

Reuse behavior.

## Polymorphism

Multiple behaviors.

------------------------------------------------------------------------

# LLD and SOLID Principles

Good LLD follows SOLID principles:

-   Single Responsibility
-   Open/Closed
-   Liskov Substitution
-   Interface Segregation
-   Dependency Inversion

Example:

A payment class should only handle payment logic.

------------------------------------------------------------------------

# LLD Example: Food Delivery System

Classes:

    Customer

    Restaurant

    Order

    DeliveryPartner

    Payment

Order Flow:

    Customer

     ↓

    Create Order

     ↓

    Restaurant Accepts

     ↓

    Delivery Assigned

     ↓

    Payment Completed

------------------------------------------------------------------------

# Common LLD Mistakes

## Mistake 1

Creating classes without clear responsibility.

Solution:

Follow Single Responsibility Principle.

------------------------------------------------------------------------

## Mistake 2

Making one large class.

Problem:

God Object.

Solution:

Split into smaller components.

------------------------------------------------------------------------

## Mistake 3

Ignoring future changes.

Solution:

Create flexible designs.

------------------------------------------------------------------------

# Best Practices

-   Define clear responsibilities
-   Keep classes focused
-   Use design principles
-   Reduce dependencies
-   Write reusable components
-   Consider scalability

------------------------------------------------------------------------

# Interview Questions

1.  What is Low Level Design?
2.  Difference between HLD and LLD?
3.  What does LLD contain?
4.  Why is LLD important?
5.  How does LLD relate to OOP?
6.  Explain class design.
7.  How does SOLID help LLD?

------------------------------------------------------------------------

# Cheat Sheet

``` text
Low Level Design

Classes

    ↓

Objects

    ↓

Methods

    ↓

Database

    ↓

APIs

    ↓

Code
```

------------------------------------------------------------------------

# Summary

Low Level Design transforms architectural ideas into detailed
implementation plans. It defines classes, objects, APIs, databases, and
algorithms required to build software components. A good LLD improves
code quality, maintainability, scalability, and collaboration among
developers.
