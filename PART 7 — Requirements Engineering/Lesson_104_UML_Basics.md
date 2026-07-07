# Lesson 104 --- UML Basics

# Part 7 --- Requirements Engineering

> **Objective**
>
> Understand UML (Unified Modeling Language), why it is used in software
> engineering, major UML diagrams, their purpose, and how they help
> teams visualize software systems.

------------------------------------------------------------------------

# Introduction

Software systems are complex.

Before implementation, teams need ways to visualize:

-   System structure
-   User interactions
-   Object relationships
-   System behavior

UML provides a standard visual language for this purpose.

``` text
Requirements

      ↓

UML Models

      ↓

System Design

      ↓

Implementation
```

------------------------------------------------------------------------

# What is UML?

**UML (Unified Modeling Language)** is a standardized modeling language
used to visualize, design, and document software systems.

It provides diagrams that represent:

-   Structure
-   Behavior
-   Interaction

------------------------------------------------------------------------

# Why Do We Need UML?

Without modeling:

``` text
Complex System

      ↓

Poor Understanding

      ↓

Design Problems

      ↓

Implementation Issues
```

UML helps:

-   Improve communication
-   Visualize architecture
-   Document systems
-   Identify design problems early
-   Support development and maintenance

------------------------------------------------------------------------

# UML in Software Development

UML is used during:

``` text
Requirement Analysis

        ↓

System Design

        ↓

Development

        ↓

Testing

        ↓

Maintenance
```

------------------------------------------------------------------------

# Types of UML Diagrams

UML diagrams are mainly divided into:

``` text
UML Diagrams

       |
       |
--------------------
|                  |
Structural      Behavioral
Diagrams       Diagrams
```

------------------------------------------------------------------------

# 1. Structural Diagrams

Structural diagrams show the static structure of a system.

They describe:

-   Classes
-   Objects
-   Components
-   Relationships

Examples:

-   Class Diagram
-   Component Diagram
-   Object Diagram
-   Deployment Diagram

------------------------------------------------------------------------

# 2. Behavioral Diagrams

Behavioral diagrams show how the system behaves.

They describe:

-   Activities
-   Events
-   Interactions
-   State changes

Examples:

-   Use Case Diagram
-   Sequence Diagram
-   Activity Diagram
-   State Diagram

------------------------------------------------------------------------

# Important UML Diagrams

# 1. Use Case Diagram

Shows:

-   Actors
-   System functions
-   User interactions

Example:

``` text
        Customer

            |
            |
     ----------------
     |              |
   Login        Payment

     Banking System
```

Used during:

-   Requirement analysis
-   Understanding user goals

------------------------------------------------------------------------

# 2. Class Diagram

Shows the structure of classes and relationships.

Example:

``` text
+-------------+
|  Customer   |
+-------------+
| name        |
| email       |
+-------------+
| login()     |
| order()     |
+-------------+

        |
        |
        ↓

+-------------+
|   Order     |
+-------------+
| orderId     |
| amount      |
+-------------+
```

Contains:

-   Classes
-   Attributes
-   Methods
-   Relationships

------------------------------------------------------------------------

# 3. Sequence Diagram

Shows interaction between objects over time.

Example:

``` text
Customer      System       Database

   |             |              |
   | Login       |              |
   |-----------> |              |
   |             | Check User   |
   |             |----------->  |
   |             | Response     |
   |<----------- |              |
```

Used for:

-   API flows
-   System interactions

------------------------------------------------------------------------

# 4. Activity Diagram

Shows workflow or process flow.

Example:

``` text
Start

 ↓

Login

 ↓

Validate User

 ↓

Success?

 ↓

Dashboard

 ↓

End
```

Used for:

-   Business processes
-   Workflows

------------------------------------------------------------------------

# 5. State Diagram

Shows how an object changes states.

Example:

Order System:

``` text
Created

   ↓

Paid

   ↓

Shipped

   ↓

Delivered
```

Used for:

-   Lifecycle modeling
-   Event-driven systems

------------------------------------------------------------------------

# UML Relationships

## Association

Shows connection between objects.

Example:

Customer places Order.

------------------------------------------------------------------------

## Inheritance

Shows parent-child relationship.

Example:

``` text
        User

         |
  ----------------
  |              |
Customer       Admin
```

------------------------------------------------------------------------

## Dependency

One component depends on another.

------------------------------------------------------------------------

## Aggregation

Represents a weak whole-part relationship.

Example:

Department has Employees.

------------------------------------------------------------------------

## Composition

Represents a strong ownership relationship.

Example:

House contains Rooms.

------------------------------------------------------------------------

# UML Example

## Online Shopping System

Actors:

-   Customer
-   Admin

Use Cases:

-   Login
-   Search Product
-   Place Order

Classes:

``` text
Customer

Product

Cart

Order

Payment
```

Sequence:

``` text
Customer

 ↓

Cart

 ↓

Payment

 ↓

Order Confirmation
```

------------------------------------------------------------------------

# UML vs Flowchart

  UML                       Flowchart
  ------------------------- ---------------------
  Models software systems   Shows processes
  Multiple diagram types    Mainly process flow
  Used in software design   General purpose

------------------------------------------------------------------------

# UML vs ER Diagram

  UML                         ER Diagram
  --------------------------- --------------------------
  Models software objects     Models database entities
  Classes and relationships   Tables and relationships

------------------------------------------------------------------------

# Industry Example

## Banking Application

UML helps design:

Use Case:

-   Transfer Money

Class Diagram:

-   Customer
-   Account
-   Transaction

Sequence Diagram:

-   Customer → Banking System → Database

Activity Diagram:

-   Transfer workflow

------------------------------------------------------------------------

# Common Mistakes

## Mistake 1

Creating diagrams without purpose.

Solution:

Use UML to solve communication problems.

------------------------------------------------------------------------

## Mistake 2

Making diagrams unnecessarily complex.

Solution:

Keep models understandable.

------------------------------------------------------------------------

## Mistake 3

Ignoring updates.

Solution:

Maintain diagrams as systems evolve.

------------------------------------------------------------------------

# Best Practices

-   Choose the correct UML diagram
-   Keep diagrams simple
-   Use meaningful names
-   Update documentation
-   Discuss diagrams with stakeholders

------------------------------------------------------------------------

# Interview Questions

1.  What is UML?
2.  Why is UML used?
3.  Difference between structural and behavioral diagrams?
4.  What is a Class Diagram?
5.  What is a Sequence Diagram?
6.  Difference between UML and ER Diagram?
7.  Explain Use Case Diagram.

------------------------------------------------------------------------

# Cheat Sheet

``` text
UML

Structure
   |
   ├── Class Diagram
   ├── Component Diagram
   └── Deployment Diagram


Behavior
   |
   ├── Use Case Diagram
   ├── Sequence Diagram
   ├── Activity Diagram
   └── State Diagram
```

------------------------------------------------------------------------

# Summary

UML provides a standardized way to visualize and document software
systems. Through different diagrams, teams can understand requirements,
design architecture, communicate ideas, and reduce complexity before
implementation. UML acts as a bridge between requirements and actual
software development.
