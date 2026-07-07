# Lesson 127 --- Software Design Interview Questions

# Part 8 --- Software Design

> **Objective**
>
> Prepare for Software Design interviews by understanding commonly asked
> questions about design fundamentals, architecture, HLD, LLD, SOLID
> principles, design patterns, UML diagrams, and practical system design
> scenarios.

------------------------------------------------------------------------

# Section 1 --- Software Design Fundamentals

## Q1. What is Software Design?

**Answer:**

Software Design is the process of converting software requirements into
a technical blueprint that defines system structure, components,
interfaces, data flow, and interactions.

It answers:

-   How will the system work?
-   How will components communicate?
-   How will the system be maintained?

------------------------------------------------------------------------

## Q2. Why is Software Design important?

Software design helps:

-   Reduce complexity
-   Improve maintainability
-   Support scalability
-   Increase code quality
-   Improve team collaboration

------------------------------------------------------------------------

## Q3. What are the goals of good software design?

Goals include:

-   Maintainability
-   Scalability
-   Reliability
-   Reusability
-   Performance
-   Security

------------------------------------------------------------------------

# Section 2 --- Architecture Questions

## Q4. What is Software Architecture?

Software Architecture defines the high-level structure of a software
system.

It describes:

-   Major components
-   Communication between components
-   Technology choices
-   System organization

------------------------------------------------------------------------

## Q5. Difference between Architecture and Design?

  Architecture           Design
  ---------------------- -----------------------------
  High-level structure   Detailed implementation
  Defines components     Defines classes and methods
  System view            Module view

------------------------------------------------------------------------

## Q6. Explain Layered Architecture.

Layered Architecture divides software into layers.

Example:

    Presentation Layer

            ↓

    Business Logic Layer

            ↓

    Data Access Layer

            ↓

    Database

Benefits:

-   Separation of concerns
-   Easier maintenance
-   Better organization

------------------------------------------------------------------------

## Q7. Difference between Monolithic and Microservices Architecture?

  Monolithic           Microservices
  -------------------- -------------------------------
  Single application   Multiple independent services
  Simple deployment    Complex deployment
  Harder scaling       Independent scaling

------------------------------------------------------------------------

# Section 3 --- HLD and LLD Questions

## Q8. What is High Level Design (HLD)?

HLD describes the overall system structure.

It includes:

-   Architecture
-   Components
-   Data flow
-   External integrations

------------------------------------------------------------------------

## Q9. What is Low Level Design (LLD)?

LLD describes detailed implementation.

It includes:

-   Classes
-   Methods
-   Database design
-   APIs
-   Algorithms

------------------------------------------------------------------------

## Q10. Difference between HLD and LLD?

  HLD                    LLD
  ---------------------- -----------------
  System overview        Detailed design
  Components             Classes
  Architecture focused   Code focused

------------------------------------------------------------------------

# Section 4 --- Modularity Questions

## Q11. What is Modular Design?

Modular Design divides a large system into smaller independent modules.

Benefits:

-   Easy maintenance
-   Reusability
-   Better testing
-   Scalability

------------------------------------------------------------------------

## Q12. What makes a good module?

A good module has:

-   High cohesion
-   Low coupling
-   Clear responsibility
-   Defined interfaces

------------------------------------------------------------------------

# Section 5 --- Coupling and Cohesion Questions

## Q13. What is Coupling?

Coupling measures dependency between modules.

Good design aims for:

    Low Coupling

because modules become easier to change.

------------------------------------------------------------------------

## Q14. What is Cohesion?

Cohesion measures how closely related elements inside a module are.

Good design aims for:

    High Cohesion

------------------------------------------------------------------------

## Q15. Difference between Coupling and Cohesion?

  Coupling                     Cohesion
  ---------------------------- ----------------------------
  Dependency between modules   Relationship inside module
  Should be low                Should be high

------------------------------------------------------------------------

# Section 6 --- OOP Design Questions

## Q16. What is Abstraction?

Abstraction hides unnecessary complexity and exposes only essential
functionality.

Example:

ATM:

    withdraw()

User does not see internal banking logic.

------------------------------------------------------------------------

## Q17. What is Encapsulation?

Encapsulation bundles data and methods together while restricting direct
access.

Example:

    private balance

    deposit()

    withdraw()

------------------------------------------------------------------------

## Q18. Difference between Abstraction and Encapsulation?

  Abstraction        Encapsulation
  ------------------ --------------------------
  Hides complexity   Hides data
  Design concept     Implementation technique

------------------------------------------------------------------------

# Section 7 --- SOLID Principle Questions

## Q19. What are SOLID Principles?

SOLID is a set of object-oriented design principles.

They are:

-   Single Responsibility Principle
-   Open/Closed Principle
-   Liskov Substitution Principle
-   Interface Segregation Principle
-   Dependency Inversion Principle

------------------------------------------------------------------------

## Q20. Explain Single Responsibility Principle.

A class should have only one reason to change.

Example:

Bad:

    Employee class

    Salary
    Database
    Email

Better:

    Employee

    Salary Service

    Email Service

------------------------------------------------------------------------

## Q21. Explain Open/Closed Principle.

Software should be open for extension but closed for modification.

Example:

Adding a new payment method without changing existing payment logic.

------------------------------------------------------------------------

## Q22. Explain Dependency Inversion Principle.

High-level modules should depend on abstractions instead of concrete
implementations.

Example:

    Service

     ↓

    Database Interface

     ↓

    MySQL

------------------------------------------------------------------------

# Section 8 --- Design Pattern Questions

## Q23. What are Design Patterns?

Design Patterns are reusable solutions to common software design
problems.

------------------------------------------------------------------------

## Q24. Types of Design Patterns?

Three categories:

### Creational

Object creation.

Examples:

-   Singleton
-   Factory

### Structural

Object organization.

Examples:

-   Adapter
-   Facade

### Behavioral

Object communication.

Examples:

-   Observer
-   Strategy

------------------------------------------------------------------------

## Q25. Explain Singleton Pattern.

Singleton ensures only one instance of a class exists.

Examples:

-   Logger
-   Configuration manager

------------------------------------------------------------------------

## Q26. Explain Factory Pattern.

Factory creates objects without exposing object creation logic.

Example:

    Payment Factory

    Card Payment

    UPI Payment

------------------------------------------------------------------------

# Section 9 --- UML Questions

## Q27. What is UML?

UML is a standardized modeling language used to visualize and document
software systems.

------------------------------------------------------------------------

## Q28. Name common UML diagrams.

Structural:

-   Class Diagram
-   Component Diagram
-   Deployment Diagram

Behavioral:

-   Use Case Diagram
-   Sequence Diagram
-   Activity Diagram
-   State Diagram

------------------------------------------------------------------------

## Q29. Difference between Sequence and Activity Diagram?

  Sequence Diagram     Activity Diagram
  -------------------- ------------------
  Object interaction   Workflow
  Time-based           Process-based

------------------------------------------------------------------------

# Section 10 --- Scenario Based Questions

## Q30. Design a Food Delivery System.

Possible components:

    User Service

    Restaurant Service

    Order Service

    Payment Service

    Delivery Service

Architecture:

    Mobile App

     ↓

    API Gateway

     ↓

    Services

     ↓

    Database

------------------------------------------------------------------------

## Q31. How would you design a scalable system?

Consider:

-   Load balancing
-   Database optimization
-   Caching
-   Horizontal scaling
-   Microservices
-   Monitoring

------------------------------------------------------------------------

## Q32. How do you reduce system dependency?

Use:

-   Interfaces
-   Dependency Injection
-   APIs
-   Modular design

------------------------------------------------------------------------

# Quick Revision Questions

1.  What is HLD?
2.  What is LLD?
3.  Explain SOLID principles.
4.  What is coupling?
5.  What is cohesion?
6.  Explain abstraction.
7.  Explain encapsulation.
8.  What are design patterns?
9.  Explain UML diagrams.
10. Explain modular design.

------------------------------------------------------------------------

# Interview Tips

For design questions:

1.  Understand requirements first.
2.  Identify major components.
3.  Explain architecture.
4.  Discuss scalability.
5.  Mention trade-offs.

------------------------------------------------------------------------

# Summary

Software Design interviews evaluate whether a candidate can convert
requirements into maintainable technical solutions. Strong answers
should connect concepts like architecture, HLD, LLD, SOLID principles,
design patterns, and UML diagrams with practical system examples.
