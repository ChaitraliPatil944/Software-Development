# Lesson 110 --- Software Design Fundamentals

# Part 8 --- Software Design

> **Objective**
>
> Understand Software Design, why it is required after requirements
> analysis, major design activities, design goals, principles, and how
> software engineers convert requirements into a structured solution.

------------------------------------------------------------------------

# Introduction

Requirements tell us:

**What the system should do**

Software Design decides:

**How the system will do it**

``` text
Requirements

      ↓

Software Design

      ↓

Implementation

      ↓

Testing

      ↓

Software Product
```

------------------------------------------------------------------------

# What is Software Design?

**Software Design** is the process of defining the architecture,
components, interfaces, data structures, and interactions required to
build a software system.

It acts as a bridge between:

``` text
Customer Requirements

        ↓

Software Design

        ↓

Source Code
```

------------------------------------------------------------------------

# Why Do We Need Software Design?

Without proper design:

``` text
Coding Starts

      ↓

Poor Structure

      ↓

Complex System

      ↓

Maintenance Problems
```

Good design helps:

-   Improve software quality
-   Reduce complexity
-   Support scalability
-   Make maintenance easier
-   Improve team collaboration

------------------------------------------------------------------------

# Goals of Software Design

A good software design should provide:

## 1. Maintainability

Easy to modify and improve.

Example:

Adding a new payment method without changing the entire system.

------------------------------------------------------------------------

## 2. Scalability

Ability to handle growth.

Example:

Supporting more users as the application grows.

------------------------------------------------------------------------

## 3. Reliability

System should work consistently.

------------------------------------------------------------------------

## 4. Reusability

Components should be reusable.

Example:

Authentication module used by multiple applications.

------------------------------------------------------------------------

## 5. Performance

System should use resources efficiently.

------------------------------------------------------------------------

# Software Design Process

``` text
Requirement Analysis

        ↓

Architectural Design

        ↓

High Level Design

        ↓

Low Level Design

        ↓

Implementation
```

------------------------------------------------------------------------

# Levels of Software Design

Software design is mainly divided into:

``` text
Software Design

        |
--------------------
|                  |
High Level       Low Level
Design           Design
```

------------------------------------------------------------------------

# High Level Design (HLD)

Focuses on overall system structure.

Includes:

-   Architecture
-   Components
-   Modules
-   Data flow

Example:

``` text
Frontend

    ↓

Backend API

    ↓

Database
```

------------------------------------------------------------------------

# Low Level Design (LLD)

Focuses on internal details.

Includes:

-   Classes
-   Methods
-   Algorithms
-   Database tables

Example:

``` text
User Class

Attributes:
- userId
- name
- email

Methods:
- login()
- logout()
```

------------------------------------------------------------------------

# Software Design Activities

## 1. Architectural Design

Defines overall system organization.

Example:

Monolithic architecture

or

Microservices architecture

------------------------------------------------------------------------

## 2. Component Design

Defines system modules.

Example:

``` text
E-Commerce System

├── User Module
├── Product Module
├── Cart Module
└── Payment Module
```

------------------------------------------------------------------------

## 3. Database Design

Defines:

-   Tables
-   Relationships
-   Data storage

------------------------------------------------------------------------

## 4. Interface Design

Defines communication between components.

Example:

API contracts.

------------------------------------------------------------------------

# Design Principles

Important principles:

## 1. Simplicity

Keep design easy to understand.

------------------------------------------------------------------------

## 2. Separation of Concerns

Each component should have a specific responsibility.

Example:

Payment logic should not handle user authentication.

------------------------------------------------------------------------

## 3. Modularity

Divide system into independent modules.

------------------------------------------------------------------------

## 4. Information Hiding

Internal details should be hidden from other components.

------------------------------------------------------------------------

# Software Design Example

## Online Banking System

Requirements:

Customer can transfer money.

Design:

Architecture:

``` text
Mobile App

      ↓

Banking API

      ↓

Transaction Service

      ↓

Database
```

Modules:

-   User Module
-   Account Module
-   Transaction Module
-   Notification Module

------------------------------------------------------------------------

# Software Design vs Software Architecture

  Software Design                    Software Architecture
  ---------------------------------- ------------------------------
  Detailed implementation planning   Overall system structure
  Classes and modules                Components and communication
  Low-level decisions                High-level decisions

------------------------------------------------------------------------

# Common Design Problems

## 1. Tight Coupling

Problem:

Components depend heavily on each other.

Solution:

Reduce dependencies.

------------------------------------------------------------------------

## 2. Low Cohesion

Problem:

One module performs many unrelated tasks.

Solution:

Keep responsibilities focused.

------------------------------------------------------------------------

## 3. Duplicate Logic

Problem:

Same code exists multiple places.

Solution:

Create reusable components.

------------------------------------------------------------------------

# Industry Example

## Food Delivery Application

Design:

Architecture:

``` text
Mobile Application

        ↓

API Gateway

        ↓

Services

        ↓

Database
```

Components:

-   User Service
-   Restaurant Service
-   Order Service
-   Payment Service

------------------------------------------------------------------------

# Interview Questions

1.  What is Software Design?
2.  Why is software design important?
3.  Difference between HLD and LLD?
4.  What are software design goals?
5.  Explain modular design.
6.  What is separation of concerns?
7.  Difference between architecture and design?

------------------------------------------------------------------------

# Cheat Sheet

``` text
Software Design

Requirements

      ↓

Architecture

      ↓

HLD

      ↓

LLD

      ↓

Code
```

------------------------------------------------------------------------

# Summary

Software Design converts requirements into a technical blueprint for
implementation. It defines system structure, components, interactions,
and internal details. Good software design improves maintainability,
scalability, reliability, and overall software quality.
