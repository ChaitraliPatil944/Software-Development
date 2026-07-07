# Lesson 120 --- Design Patterns Overview

# Part 8 --- Software Design

> **Objective**
>
> Understand Design Patterns, why they are used, their history,
> categories, common patterns, real-world examples, and how they help
> developers create reusable and maintainable software designs.

------------------------------------------------------------------------

# Introduction

Software developers often face similar design problems repeatedly.

Instead of solving every problem from scratch, experienced developers
use proven solutions called **Design Patterns**.

``` text
Design Problem

        ↓

Reusable Solution

        ↓

Better Software Design
```

------------------------------------------------------------------------

# What are Design Patterns?

A **Design Pattern** is a reusable solution to a commonly occurring
software design problem.

It is not ready-made code.

It is a general approach or template that can be adapted to different
situations.

------------------------------------------------------------------------

# Why Do We Need Design Patterns?

Without design patterns:

``` text
Repeated Problems

        ↓

Different Solutions

        ↓

Inconsistent Design

        ↓

Maintenance Issues
```

Design patterns provide:

-   Reusable solutions
-   Better communication
-   Proven approaches
-   Flexible designs
-   Improved maintainability

------------------------------------------------------------------------

# History of Design Patterns

The concept became popular through the book:

**"Design Patterns: Elements of Reusable Object-Oriented Software"**

by the **Gang of Four (GoF)**:

-   Erich Gamma
-   Richard Helm
-   Ralph Johnson
-   John Vlissides

The book introduced 23 classic design patterns.

------------------------------------------------------------------------

# Design Pattern Structure

A pattern usually contains:

``` text
Pattern Name

        ↓

Problem

        ↓

Solution

        ↓

Consequences
```

------------------------------------------------------------------------

# Types of Design Patterns

Design Patterns are mainly divided into three categories:

``` text
Design Patterns

        |
--------------------------------
|              |               |
Creational   Structural   Behavioral
```

------------------------------------------------------------------------

# 1. Creational Design Patterns

Focus:

Object creation.

They provide flexible ways to create objects.

Examples:

-   Singleton
-   Factory Method
-   Abstract Factory
-   Builder
-   Prototype

------------------------------------------------------------------------

# Singleton Pattern

## Purpose

Ensures only one instance of a class exists.

Example:

Configuration Manager

``` text
Application

      ↓

Single Configuration Object
```

Uses:

-   Database connection manager
-   Logging system

------------------------------------------------------------------------

## Benefits

-   Controls object creation
-   Saves resources

------------------------------------------------------------------------

## Problems

-   Can create global state issues
-   Difficult testing if overused

------------------------------------------------------------------------

# Factory Pattern

## Purpose

Creates objects without exposing creation logic.

Example:

``` text
Payment Factory

        |

------------------

Card Payment

UPI Payment

Wallet Payment
```

Client requests an object without knowing implementation details.

------------------------------------------------------------------------

# 2. Structural Design Patterns

Focus:

How classes and objects are combined.

Examples:

-   Adapter
-   Decorator
-   Facade
-   Proxy
-   Composite

------------------------------------------------------------------------

# Adapter Pattern

## Purpose

Allows incompatible interfaces to work together.

Real-world example:

Power adapter:

``` text
US Plug

    ↓

Adapter

    ↓

Indian Socket
```

Software example:

Connecting old API with new system.

------------------------------------------------------------------------

# Facade Pattern

## Purpose

Provides a simple interface to a complex system.

Example:

Online Shopping:

Instead of calling:

    Inventory Service

    Payment Service

    Shipping Service

User calls:

    Place Order()

------------------------------------------------------------------------

# 3. Behavioral Design Patterns

Focus:

Communication between objects.

Examples:

-   Observer
-   Strategy
-   Command
-   Iterator
-   State

------------------------------------------------------------------------

# Observer Pattern

## Purpose

One object notifies multiple dependent objects about changes.

Example:

YouTube subscription:

``` text
Channel

    ↓

Subscribers
```

When new content is uploaded, subscribers receive notifications.

------------------------------------------------------------------------

# Strategy Pattern

## Purpose

Allows changing behavior dynamically.

Example:

Payment methods:

``` text
Payment Strategy

       |

----------------

Credit Card

UPI

Wallet
```

------------------------------------------------------------------------

# Design Patterns Example

## E-Commerce System

Possible patterns:

Singleton:

    Application Configuration

Factory:

    Create Payment Method

Observer:

    Order Status Notification

Strategy:

    Payment Selection

------------------------------------------------------------------------

# Design Patterns and SOLID Principles

Design patterns work well with SOLID.

Example:

Strategy Pattern uses:

-   Open/Closed Principle
-   Dependency Inversion Principle

Factory Pattern improves:

-   Loose coupling

------------------------------------------------------------------------

# Design Pattern vs Algorithm

  Design Pattern          Algorithm
  ----------------------- ------------------------
  Design solution         Problem-solving steps
  Focuses on structure    Focuses on computation
  Reusable architecture   Specific procedure

------------------------------------------------------------------------

# Design Pattern vs Framework

  Design Pattern         Framework
  ---------------------- -----------------------------
  Concept/template       Complete software structure
  Developer implements   Framework controls flow
  Smaller solution       Larger system

------------------------------------------------------------------------

# Advantages of Design Patterns

-   Proven solutions
-   Better code organization
-   Improved flexibility
-   Easier communication
-   Reduced design errors

------------------------------------------------------------------------

# Disadvantages of Design Patterns

-   Overuse increases complexity
-   Requires understanding
-   Not every problem needs a pattern

------------------------------------------------------------------------

# Common Mistakes

## Mistake 1

Using patterns everywhere.

Solution:

Use only when they solve a real problem.

------------------------------------------------------------------------

## Mistake 2

Memorizing patterns without understanding.

Solution:

Understand the problem each pattern solves.

------------------------------------------------------------------------

## Mistake 3

Making simple systems unnecessarily complex.

Solution:

Prefer simplicity.

------------------------------------------------------------------------

# Industry Examples

## Banking Application

Singleton:

-   Configuration management

Factory:

-   Account creation

Strategy:

-   Payment processing

Observer:

-   Transaction alerts

------------------------------------------------------------------------

# Interview Questions

1.  What are Design Patterns?
2.  Why are design patterns used?
3.  What are GoF patterns?
4.  Explain types of design patterns.
5.  Difference between Factory and Singleton?
6.  Explain Observer Pattern.
7.  How are design patterns related to SOLID principles?

------------------------------------------------------------------------

# Cheat Sheet

``` text
Design Patterns

Creational

    ↓
Object Creation

Structural

    ↓
Object Organization

Behavioral

    ↓
Object Communication
```

------------------------------------------------------------------------

# Summary

Design Patterns provide reusable solutions to common software design
problems. They help developers create flexible, maintainable, and
scalable systems by applying proven approaches. However, patterns should
be used carefully because unnecessary complexity is still complexity
wearing a fancy design-pattern costume.
