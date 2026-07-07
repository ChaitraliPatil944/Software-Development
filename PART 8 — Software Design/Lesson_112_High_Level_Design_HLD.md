# Lesson 112 --- High Level Design (HLD)

# Part 8 --- Software Design

> **Objective**
>
> Understand High Level Design (HLD), why it is created, its components,
> architecture representation, system components, data flow, and how it
> helps teams build scalable software systems.

------------------------------------------------------------------------

# Introduction

After requirements are collected and software architecture is selected,
teams create a high-level blueprint of the system.

This blueprint is called **High Level Design (HLD)**.

``` text
Requirements

      ↓

Architecture

      ↓

High Level Design

      ↓

Low Level Design

      ↓

Code
```

------------------------------------------------------------------------

# What is High Level Design?

**High Level Design (HLD)** describes the overall structure of a
software system.

It focuses on:

-   Major components
-   System architecture
-   Module interaction
-   Data flow
-   External integrations

HLD answers:

-   What are the major parts of the system?
-   How do components communicate?
-   Where will data flow?

------------------------------------------------------------------------

# Why Do We Need HLD?

Without HLD:

``` text
Development Starts

        ↓

No Clear Structure

        ↓

Design Conflicts

        ↓

Implementation Problems
```

HLD helps:

-   Create system understanding
-   Guide developers
-   Improve communication
-   Identify design risks early
-   Support scalability planning

------------------------------------------------------------------------

# HLD in Software Development

``` text
Requirement Analysis

        ↓

Architectural Design

        ↓

High Level Design

        ↓

Low Level Design

        ↓

Development
```

------------------------------------------------------------------------

# Components of HLD

A typical HLD contains:

``` text
High Level Design

        |
-------------------------
|       |       |       |
Architecture Components Data Flow Interfaces
```

------------------------------------------------------------------------

# 1. System Architecture

Defines overall system organization.

Example:

``` text
User

 ↓

Frontend Application

 ↓

Backend Services

 ↓

Database
```

------------------------------------------------------------------------

# 2. Components and Modules

HLD identifies major modules.

Example:

## E-Commerce System

``` text
E-Commerce Platform

├── User Service
├── Product Service
├── Cart Service
├── Order Service
├── Payment Service
└── Notification Service
```

------------------------------------------------------------------------

# 3. Data Flow Design

Shows how information moves through the system.

Example:

``` text
Customer

   ↓

Order API

   ↓

Order Service

   ↓

Database

   ↓

Confirmation
```

------------------------------------------------------------------------

# 4. External System Integration

HLD defines connections with external systems.

Examples:

-   Payment Gateway
-   Email Service
-   Authentication Provider
-   Cloud Storage

------------------------------------------------------------------------

# 5. Technology Selection

HLD may specify:

Frontend:

-   React
-   Angular

Backend:

-   Java Spring Boot
-   Node.js

Database:

-   MySQL
-   PostgreSQL

Cloud:

-   AWS
-   Azure

------------------------------------------------------------------------

# HLD Example

## Online Banking System

Architecture:

``` text
Mobile Application

        ↓

API Gateway

        ↓

Banking Services

        ↓

Database
```

Major Components:

``` text
User Service

Account Service

Transaction Service

Notification Service
```

External Systems:

``` text
Payment Network

SMS Gateway

Authentication System
```

------------------------------------------------------------------------

# HLD Diagram Example

``` text
              User

                |

                ↓

        Web/Mobile Application

                |

                ↓

            API Gateway

                |

    -----------------------

    |          |          |

 User      Order     Payment

Service   Service   Service

    |          |          |

    -----------------------

                |

             Database
```

------------------------------------------------------------------------

# HLD vs LLD

  High Level Design              Low Level Design
  ------------------------------ -------------------------
  System overview                Detailed implementation
  Architecture focused           Code focused
  Components and communication   Classes and methods
  Created before LLD             Created before coding

------------------------------------------------------------------------

# HLD vs Architecture

  Architecture                   HLD
  ------------------------------ --------------------------------------
  Defines overall system style   Defines implementation structure
  More abstract                  More detailed
  Example: Microservices         Example: User service, Order service

------------------------------------------------------------------------

# HLD and Scalability

HLD considers:

## Horizontal Scaling

Adding more servers.

Example:

    Server 1
    Server 2
    Server 3

------------------------------------------------------------------------

## Vertical Scaling

Increasing server capacity.

Example:

    More CPU
    More RAM

------------------------------------------------------------------------

# HLD and Security

Security decisions include:

-   Authentication service
-   Authorization
-   Encryption
-   Secure communication

Example:

``` text
User

 ↓

Authentication Service

 ↓

Protected APIs
```

------------------------------------------------------------------------

# Industry Example

## Food Delivery Application

HLD:

``` text
Mobile App

      ↓

API Gateway

      ↓

Microservices

      ↓

Database
```

Services:

-   User Service
-   Restaurant Service
-   Order Service
-   Delivery Service
-   Payment Service

This design allows individual services to scale independently.

------------------------------------------------------------------------

# Common HLD Mistakes

## Mistake 1

Creating HLD without understanding requirements.

Solution:

Start with business needs.

------------------------------------------------------------------------

## Mistake 2

Ignoring future scalability.

Solution:

Consider growth early.

------------------------------------------------------------------------

## Mistake 3

Making HLD too detailed.

Solution:

Keep implementation details for LLD.

------------------------------------------------------------------------

# Best Practices

-   Keep architecture simple
-   Define clear component boundaries
-   Document communication flow
-   Consider scalability
-   Consider security
-   Review with stakeholders

------------------------------------------------------------------------

# Interview Questions

1.  What is High Level Design?
2.  Why is HLD important?
3.  What components are included in HLD?
4.  Difference between HLD and LLD?
5.  What information does an HLD diagram contain?
6.  How does HLD support scalability?
7.  Explain HLD of an e-commerce system.

------------------------------------------------------------------------

# Cheat Sheet

``` text
High Level Design

Architecture

      ↓

Components

      ↓

Communication

      ↓

Data Flow

      ↓

System Blueprint
```

------------------------------------------------------------------------

# Summary

High Level Design provides a broad view of a software system by defining
architecture, major components, communication patterns, and data flow.
It acts as a bridge between requirements and detailed implementation,
helping teams build scalable, maintainable, and reliable software
systems.
