# Lesson 129 --- Software Design Revision Notes

# Part 8 --- Software Design

> **Objective**
>
> Revise complete Software Design concepts including fundamentals,
> architecture, HLD, LLD, modular design, coupling, cohesion, OOP
> principles, SOLID principles, design patterns, UML diagrams, and
> design practices.

------------------------------------------------------------------------

# 1. Software Design Fundamentals

Software Design converts:

``` text
Requirements

      ↓

Technical Blueprint

      ↓

Implementation
```

It defines:

-   Architecture
-   Components
-   Interfaces
-   Data structures
-   Interactions

------------------------------------------------------------------------

# 2. Goals of Good Software Design

A good design should provide:

## Maintainability

Easy modification and improvement.

## Scalability

Ability to handle growth.

## Reliability

Consistent system behavior.

## Reusability

Components can be reused.

## Performance

Efficient resource usage.

------------------------------------------------------------------------

# 3. Software Architecture

Architecture defines the high-level structure of software.

It includes:

-   Components
-   Communication
-   Technology decisions
-   System organization

Common architectures:

``` text
Layered Architecture

Client-Server

MVC

Monolithic

Microservices
```

------------------------------------------------------------------------

# 4. High Level Design (HLD)

HLD focuses on system structure.

Includes:

-   Architecture
-   Components
-   Services
-   Data flow
-   External systems

Example:

``` text
Frontend

   ↓

Backend API

   ↓

Database
```

------------------------------------------------------------------------

# 5. Low Level Design (LLD)

LLD focuses on implementation details.

Includes:

-   Classes
-   Objects
-   Methods
-   APIs
-   Algorithms
-   Database design

Example:

    User Class

    Attributes:

    userId

    name

    email

    Methods:

    login()

    logout()

------------------------------------------------------------------------

# 6. HLD vs LLD

  HLD                    LLD
  ---------------------- -------------------------
  System overview        Detailed implementation
  Architecture focused   Code focused
  Components             Classes
  Before LLD             Before coding

------------------------------------------------------------------------

# 7. Modular Design

Modular design divides software into independent modules.

Benefits:

-   Maintainability
-   Reusability
-   Testing
-   Scalability

Good modules have:

``` text
High Cohesion

+

Low Coupling
```

------------------------------------------------------------------------

# 8. Coupling

Coupling measures dependency between modules.

Good design:

    Low Coupling

Types:

    Content Coupling

    Common Coupling

    Control Coupling

    Stamp Coupling

    Data Coupling

------------------------------------------------------------------------

# 9. Cohesion

Cohesion measures relationship inside a module.

Good design:

    High Cohesion

Highest:

    Functional Cohesion

Lowest:

    Coincidental Cohesion

------------------------------------------------------------------------

# 10. Abstraction

Abstraction hides unnecessary complexity.

Focus:

    What an object does

Example:

ATM:

    withdraw()

User does not see internal banking logic.

Implemented using:

-   Abstract classes
-   Interfaces

------------------------------------------------------------------------

# 11. Encapsulation

Encapsulation protects internal data.

Focus:

    How data is controlled

Uses:

-   Classes
-   Access modifiers
-   Getters
-   Setters

Example:

    private balance

    deposit()

    withdraw()

------------------------------------------------------------------------

# 12. Abstraction vs Encapsulation

  Abstraction        Encapsulation
  ------------------ --------------------------
  Hides complexity   Hides data
  Design concept     Implementation technique
  Focuses behavior   Focuses protection

------------------------------------------------------------------------

# 13. SOLID Principles

SOLID improves object-oriented design.

------------------------------------------------------------------------

## S --- Single Responsibility Principle

One class should have one responsibility.

------------------------------------------------------------------------

## O --- Open Closed Principle

Open for extension, closed for modification.

------------------------------------------------------------------------

## L --- Liskov Substitution Principle

Child objects should replace parent objects safely.

------------------------------------------------------------------------

## I --- Interface Segregation Principle

Clients should not depend on unused methods.

------------------------------------------------------------------------

## D --- Dependency Inversion Principle

Depend on abstractions, not concrete implementations.

------------------------------------------------------------------------

# 14. Design Patterns

Design patterns are reusable solutions to common problems.

Categories:

``` text
Creational

Structural

Behavioral
```

------------------------------------------------------------------------

# Creational Patterns

Object creation.

Examples:

-   Singleton
-   Factory
-   Builder

------------------------------------------------------------------------

# Structural Patterns

Object organization.

Examples:

-   Adapter
-   Facade
-   Decorator

------------------------------------------------------------------------

# Behavioral Patterns

Object communication.

Examples:

-   Observer
-   Strategy
-   Command

------------------------------------------------------------------------

# 15. UML Diagrams

UML visualizes software systems.

------------------------------------------------------------------------

# Structural Diagrams

Show system structure.

Examples:

-   Class Diagram
-   Object Diagram
-   Component Diagram
-   Deployment Diagram

------------------------------------------------------------------------

# Behavioral Diagrams

Show system behavior.

Examples:

-   Use Case Diagram
-   Sequence Diagram
-   Activity Diagram
-   State Diagram

------------------------------------------------------------------------

# 16. ER Diagrams

ER diagrams model databases.

Components:

    Entity

    Attribute

    Relationship

Relationships:

    1:1

    1:N

    N:M

------------------------------------------------------------------------

# 17. Flowcharts

Flowcharts represent process logic.

Symbols:

-   Start/End
-   Process
-   Decision
-   Input/Output

Used for:

-   Algorithms
-   Workflows
-   Logic planning

------------------------------------------------------------------------

# 18. Sequence Diagrams

Show object communication over time.

Components:

-   Objects
-   Lifelines
-   Messages

Example:

    User

     ↓

    Controller

     ↓

    Database

------------------------------------------------------------------------

# 19. Activity Diagrams

Show workflows.

Components:

-   Activities
-   Decisions
-   Fork
-   Join
-   Swimlanes

------------------------------------------------------------------------

# 20. State Diagrams

Show object lifecycle.

Components:

-   States
-   Events
-   Transitions

Example:

    Created

     ↓

    Paid

     ↓

    Delivered

------------------------------------------------------------------------

# 21. Complete Software Design Flow

``` text
Requirements

      ↓

Architecture

      ↓

HLD

      ↓

LLD

      ↓

Classes

      ↓

Code

      ↓

Testing
```

------------------------------------------------------------------------

# 22. Design Quality Checklist

Before finalizing design:

✓ Requirements understood

✓ Components identified

✓ Responsibilities separated

✓ Coupling minimized

✓ Cohesion improved

✓ SOLID applied

✓ Scalability considered

✓ Security considered

✓ Documentation created

------------------------------------------------------------------------

# 23. Interview Quick Revision

## What is HLD?

High-level system structure.

------------------------------------------------------------------------

## What is LLD?

Detailed implementation design.

------------------------------------------------------------------------

## What is SOLID?

Five principles for maintainable object-oriented design.

------------------------------------------------------------------------

## What is Coupling?

Dependency between modules.

------------------------------------------------------------------------

## What is Cohesion?

Relationship inside a module.

------------------------------------------------------------------------

## What are Design Patterns?

Reusable design solutions.

------------------------------------------------------------------------

# Complete Software Design Memory Map

``` text
                 SOFTWARE DESIGN

                        |

        --------------------------------

        Architecture

             |

        HLD

             |

        LLD

             |

     ----------------------

     |                    |

  OOP Design          UML


     |

 ------------------------

 |          |            |

SOLID   Patterns    Principles


     |

 Quality Software
```

------------------------------------------------------------------------

# Part 8 Summary

You now understand:

✓ Software Design Fundamentals\
✓ Architectural Design\
✓ HLD\
✓ LLD\
✓ Modular Design\
✓ Coupling\
✓ Cohesion\
✓ Abstraction\
✓ Encapsulation\
✓ SOLID Principles\
✓ Design Patterns\
✓ UML Diagrams\
✓ ER Diagrams\
✓ Flowcharts\
✓ Sequence Diagrams\
✓ Activity Diagrams\
✓ State Diagrams

Software Design is the foundation that transforms requirements into
scalable, maintainable, and reliable software systems.

------------------------------------------------------------------------

# Next Topic

## Part 9 --- Object Oriented Design

Upcoming lessons:

-   OOP Fundamentals
-   Classes and Objects
-   Inheritance
-   Polymorphism
-   Interfaces
-   Composition
-   Advanced OOP Design
