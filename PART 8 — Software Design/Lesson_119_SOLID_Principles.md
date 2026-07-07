# Lesson 119 --- SOLID Principles

# Part 8 --- Software Design

> **Objective**
>
> Understand SOLID Principles, why they are important in software
> design, each principle in detail, examples, benefits, and how they
> help developers create maintainable and flexible software systems.

------------------------------------------------------------------------

# Introduction

As software grows, code becomes harder to manage.

Poor design creates:

``` text
More Features

      ↓

More Complexity

      ↓

More Bugs

      ↓

Difficult Maintenance
```

SOLID principles provide guidelines for writing clean, flexible, and
maintainable object-oriented software.

------------------------------------------------------------------------

# What are SOLID Principles?

**SOLID** is a set of five object-oriented design principles introduced
to improve software design quality.

SOLID stands for:

``` text
S → Single Responsibility Principle

O → Open/Closed Principle

L → Liskov Substitution Principle

I → Interface Segregation Principle

D → Dependency Inversion Principle
```

------------------------------------------------------------------------

# Why Do We Need SOLID Principles?

SOLID helps achieve:

-   Maintainable code
-   Flexible design
-   Easier testing
-   Reduced dependency
-   Better scalability
-   Reusable components

------------------------------------------------------------------------

# 1. Single Responsibility Principle (SRP)

## Definition

A class should have only one reason to change.

Meaning:

A class should have one responsibility.

------------------------------------------------------------------------

# Bad Design Example

``` text
Employee Class

- Store employee data
- Calculate salary
- Generate reports
- Send emails
```

Problem:

One class handles multiple responsibilities.

------------------------------------------------------------------------

# Better Design

``` text
Employee

      ↓

Salary Service

      ↓

Report Service

      ↓

Email Service
```

Each class has one responsibility.

------------------------------------------------------------------------

# Benefits of SRP

-   Easier maintenance
-   Easier testing
-   Less code dependency

------------------------------------------------------------------------

# 2. Open/Closed Principle (OCP)

## Definition

Software entities should be:

-   Open for extension
-   Closed for modification

Meaning:

Add new features without changing existing code.

------------------------------------------------------------------------

# Bad Example

``` text
Payment Class

if paymentType == Card

else if paymentType == UPI

else if paymentType == Wallet
```

Every new payment requires modifying the class.

------------------------------------------------------------------------

# Better Design

``` text
Payment Interface

        |
------------------

Card Payment

UPI Payment

Wallet Payment
```

New payment methods can be added easily.

------------------------------------------------------------------------

# Benefits of OCP

-   Reduces bugs
-   Supports scalability
-   Improves flexibility

------------------------------------------------------------------------

# 3. Liskov Substitution Principle (LSP)

## Definition

Objects of a subclass should be replaceable with objects of the parent
class without breaking the system.

------------------------------------------------------------------------

# Example

Parent:

``` text
Bird
```

Child:

``` text
FlyingBird
```

Problem:

Not every bird can fly.

Example:

``` text
Penguin
```

A better design separates flying behavior.

------------------------------------------------------------------------

# Benefits of LSP

-   Reliable inheritance
-   Better object design
-   Prevents unexpected behavior

------------------------------------------------------------------------

# 4. Interface Segregation Principle (ISP)

## Definition

Clients should not be forced to depend on interfaces they do not use.

------------------------------------------------------------------------

# Bad Design

``` text
Machine Interface

print()

scan()

fax()
```

A simple printer does not need all methods.

------------------------------------------------------------------------

# Better Design

``` text
Printer Interface

Scan Interface

Fax Interface
```

Classes implement only required behavior.

------------------------------------------------------------------------

# Benefits of ISP

-   Smaller interfaces
-   Less dependency
-   Cleaner design

------------------------------------------------------------------------

# 5. Dependency Inversion Principle (DIP)

## Definition

High-level modules should not depend on low-level modules. Both should
depend on abstractions.

------------------------------------------------------------------------

# Bad Design

``` text
Order Service

      ↓

MySQL Database
```

Order service is tightly connected to MySQL.

------------------------------------------------------------------------

# Better Design

``` text
Order Service

      ↓

Database Interface

      ↓

MySQL / PostgreSQL
```

The service depends on abstraction.

------------------------------------------------------------------------

# Benefits of DIP

-   Loose coupling
-   Easier testing
-   Easy technology changes

------------------------------------------------------------------------

# SOLID Principles Relationship

``` text
Single Responsibility

        ↓

Better Modules

        ↓

Low Coupling

        ↓

Flexible System
```

------------------------------------------------------------------------

# SOLID Example: E-Commerce System

Without SOLID:

``` text
Order Class

Handles:

- Order creation
- Payment
- Email
- Database
```

Problem:

Too many responsibilities.

------------------------------------------------------------------------

With SOLID:

``` text
Order Service

Payment Service

Notification Service

Repository Service
```

Each component has a clear role.

------------------------------------------------------------------------

# SOLID and Design Patterns

SOLID principles are used with:

-   Factory Pattern
-   Strategy Pattern
-   Observer Pattern
-   Dependency Injection

They help create reusable designs.

------------------------------------------------------------------------

# SOLID vs Normal Coding

  Without SOLID       With SOLID
  ------------------- -----------------
  Tightly coupled     Loosely coupled
  Hard changes        Easy extension
  Difficult testing   Easier testing
  Less reusable       More reusable

------------------------------------------------------------------------

# Common Mistakes

## Mistake 1

Creating large classes.

Solution:

Apply Single Responsibility Principle.

------------------------------------------------------------------------

## Mistake 2

Overusing inheritance.

Solution:

Prefer composition where suitable.

------------------------------------------------------------------------

## Mistake 3

Creating unnecessary interfaces.

Solution:

Keep design simple.

------------------------------------------------------------------------

# Best Practices

-   Keep classes focused
-   Depend on abstractions
-   Prefer composition
-   Design for change
-   Write testable code

------------------------------------------------------------------------

# Interview Questions

1.  What are SOLID principles?
2.  Explain Single Responsibility Principle.
3.  What is Open/Closed Principle?
4.  Explain Liskov Substitution Principle.
5.  What is Interface Segregation Principle?
6.  Explain Dependency Inversion Principle.
7.  How do SOLID principles improve software design?

------------------------------------------------------------------------

# Cheat Sheet

``` text
SOLID

S → One responsibility

O → Extend without modifying

L → Replace parent with child

I → Small focused interfaces

D → Depend on abstractions
```

------------------------------------------------------------------------

# Summary

SOLID principles are fundamental guidelines for creating clean
object-oriented software. They help developers design systems that are
easier to maintain, test, extend, and scale. By following SOLID
principles, software becomes more flexible and resistant to change.
