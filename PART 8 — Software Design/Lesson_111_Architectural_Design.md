# Lesson 111 --- Architectural Design

# Part 8 --- Software Design

> **Objective**
>
> Understand Software Architectural Design, why architecture is
> important, common architectural styles, trade-offs, and how architects
> design scalable software systems.

------------------------------------------------------------------------

# Introduction

Software architecture defines the high-level structure of a software
system.

It answers:

-   What are the major components?
-   How do components communicate?
-   How will the system scale?
-   How will quality requirements be achieved?

``` text
Requirements

      ↓

Software Architecture

      ↓

Detailed Design

      ↓

Implementation

      ↓

Software System
```

------------------------------------------------------------------------

# What is Software Architecture?

**Software Architecture** is the high-level organization of a software
system that defines:

-   Components
-   Relationships
-   Communication patterns
-   Technology decisions

It provides the blueprint of the system.

------------------------------------------------------------------------

# Why Do We Need Software Architecture?

Without proper architecture:

``` text
More Features

      ↓

Complex System

      ↓

Poor Performance

      ↓

Maintenance Problems
```

Good architecture provides:

-   Scalability
-   Security
-   Performance
-   Maintainability
-   Reliability

------------------------------------------------------------------------

# Software Architecture vs Software Design

  Software Architecture   Software Design
  ----------------------- -----------------------------
  High-level structure    Detailed implementation
  Defines components      Defines classes and methods
  System organization     Module behavior

Example:

Architecture:

    Frontend
       ↓
    Backend
       ↓
    Database

Design:

    UserController

    UserService

    UserRepository

------------------------------------------------------------------------

# Architectural Design Process

``` text
Understand Requirements

        ↓

Identify Components

        ↓

Choose Architecture Style

        ↓

Define Communication

        ↓

Evaluate Trade-offs
```

------------------------------------------------------------------------

# Important Architecture Quality Attributes

## 1. Scalability

Ability to handle increasing users or workload.

Example:

A shopping website supporting millions of users.

------------------------------------------------------------------------

## 2. Performance

System should respond quickly.

Example:

Optimized APIs and caching.

------------------------------------------------------------------------

## 3. Security

Protect data and resources.

Example:

Authentication and encryption.

------------------------------------------------------------------------

## 4. Availability

System should remain accessible.

Example:

Backup servers and fault tolerance.

------------------------------------------------------------------------

## 5. Maintainability

Easy to modify and extend.

------------------------------------------------------------------------

# Common Architectural Styles

``` text
Software Architecture

        |
--------------------------------
|              |                |
Layered    Client-Server    Microservices
```

------------------------------------------------------------------------

# 1. Layered Architecture

A system is divided into layers.

Common layers:

    Presentation Layer

            ↓

    Business Logic Layer

            ↓

    Data Access Layer

            ↓

    Database

------------------------------------------------------------------------

## Advantages

-   Easy maintenance
-   Clear separation
-   Simple understanding

## Disadvantages

-   Can become slow
-   Changes may affect multiple layers

------------------------------------------------------------------------

# Example

Enterprise applications often use:

    React Frontend

            ↓

    Spring Boot Backend

            ↓

    MySQL Database

------------------------------------------------------------------------

# 2. Client-Server Architecture

A client requests services from a server.

    Client

      ↓ Request

    Server

      ↓

    Response

Examples:

-   Web applications
-   Mobile applications

------------------------------------------------------------------------

## Advantages

-   Centralized management
-   Easy resource sharing

## Disadvantages

-   Server dependency
-   Possible bottleneck

------------------------------------------------------------------------

# 3. MVC Architecture

MVC separates application responsibilities.

            User

             ↓

           View

             ↓

        Controller

             ↓

           Model

Components:

## Model

Handles data.

## View

Handles user interface.

## Controller

Handles requests.

------------------------------------------------------------------------

# 4. Monolithic Architecture

All application components exist as one application.

    ---------------------
    |  User Module       |
    |  Order Module      |
    |  Payment Module    |
    |  Database          |
    ---------------------

------------------------------------------------------------------------

## Advantages

-   Simple development
-   Easy deployment initially

## Disadvantages

-   Difficult scaling
-   Large codebase

------------------------------------------------------------------------

# 5. Microservices Architecture

Application is divided into independent services.

                 API Gateway

                      |
    --------------------------------
    |          |          |         |
    User    Order    Payment   Product
    Service Service  Service   Service

------------------------------------------------------------------------

## Advantages

-   Independent scaling
-   Easier deployment
-   Technology flexibility

## Disadvantages

-   Complex communication
-   Distributed system challenges

------------------------------------------------------------------------

# Architecture Trade-offs

Every architecture has advantages and disadvantages.

Example:

Microservices:

Benefit:

Independent scaling

Cost:

More operational complexity

------------------------------------------------------------------------

# Architectural Decision Example

## Food Delivery Application

Requirements:

-   Millions of users
-   Fast response
-   Independent feature updates

Possible architecture:

    Mobile App

          ↓

    API Gateway

          ↓

    Microservices

          ↓

    Database

Services:

-   User Service
-   Restaurant Service
-   Order Service
-   Payment Service

------------------------------------------------------------------------

# Architecture Documentation

Common documentation includes:

-   Component diagrams
-   Deployment diagrams
-   Data flow diagrams
-   Architecture diagrams

------------------------------------------------------------------------

# Common Architecture Mistakes

## Mistake 1

Choosing complex architecture too early.

Solution:

Select based on actual requirements.

------------------------------------------------------------------------

## Mistake 2

Ignoring quality attributes.

Solution:

Consider performance, security, scalability.

------------------------------------------------------------------------

## Mistake 3

No clear communication between components.

Solution:

Define interfaces and contracts.

------------------------------------------------------------------------

# Interview Questions

1.  What is Software Architecture?
2.  Why is architecture important?
3.  Difference between architecture and design?
4.  Explain layered architecture.
5.  What is MVC architecture?
6.  Difference between monolithic and microservices?
7.  What factors influence architecture decisions?

------------------------------------------------------------------------

# Cheat Sheet

``` text
Software Architecture

Defines:

✓ Components
✓ Communication
✓ Structure
✓ Quality Attributes


Styles:

Layered
Client-Server
MVC
Monolithic
Microservices
```

------------------------------------------------------------------------

# Summary

Architectural Design defines the foundation of a software system. It
determines how components are organized, how they communicate, and how
the system achieves quality goals such as scalability, performance,
security, and maintainability. Choosing the right architecture requires
balancing business needs, technical requirements, and future growth.
