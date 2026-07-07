# Lesson 109 --- Requirement Engineering Revision Notes

# Part 7 --- Requirements Engineering

> **Objective**
>
> Revise complete Requirement Engineering concepts including processes,
> requirement types, elicitation, documentation, modeling, validation,
> traceability, and interview-focused concepts.

------------------------------------------------------------------------

# 1. What is Requirement Engineering?

Requirement Engineering is the process of:

-   Discovering
-   Analyzing
-   Documenting
-   Validating
-   Managing

software requirements.

It connects:

``` text
Stakeholders

      ↓

Requirements

      ↓

Development Team

      ↓

Software Product
```

------------------------------------------------------------------------

# 2. Requirement Engineering Process

Complete workflow:

``` text
Requirement Elicitation

        ↓

Requirement Analysis

        ↓

Requirement Specification

        ↓

Requirement Validation

        ↓

Requirement Management
```

------------------------------------------------------------------------

# 3. Requirement Elicitation

Purpose:

Collect requirements from stakeholders.

Sources:

-   Customers
-   Users
-   Business teams
-   Domain experts
-   Regulatory bodies

Techniques:

``` text
Interviews

Surveys

Workshops

Observation

Brainstorming

Prototyping
```

------------------------------------------------------------------------

# 4. Requirement Analysis

Purpose:

Understand and organize collected requirements.

Activities:

-   Remove conflicts
-   Check feasibility
-   Prioritize requirements
-   Identify dependencies

------------------------------------------------------------------------

# 5. Requirement Specification

Requirements are documented using:

## Software Requirement Specification (SRS)

SRS contains:

-   Functional requirements
-   Non-functional requirements
-   Constraints
-   Interfaces
-   Assumptions

------------------------------------------------------------------------

# 6. Functional Requirements

Define:

``` text
WHAT the system should do
```

Examples:

-   User login
-   Payment processing
-   Search functionality
-   Report generation

------------------------------------------------------------------------

# 7. Non Functional Requirements

Define:

``` text
HOW the system should behave
```

Examples:

-   Performance
-   Security
-   Scalability
-   Reliability
-   Availability
-   Maintainability
-   Usability

------------------------------------------------------------------------

# 8. Functional vs Non Functional Requirements

  Functional Requirements   Non Functional Requirements
  ------------------------- -----------------------------
  Define features           Define quality
  What system does          How system performs
  Login, payment            Security, speed

------------------------------------------------------------------------

# 9. Stakeholder Analysis

A stakeholder is anyone affected by or influencing the system.

Examples:

-   Customers
-   Users
-   Managers
-   Developers
-   Admins

Power Interest Matrix:

``` text
High Power + High Interest

        ↓

Manage Closely
```

------------------------------------------------------------------------

# 10. User Stories

Format:

``` text
As a <user>

I want <feature>

So that <benefit>
```

Example:

    As a customer,
    I want order tracking,
    so that I know delivery status.

------------------------------------------------------------------------

# 11. INVEST Criteria

A good User Story should be:

``` text
I → Independent

N → Negotiable

V → Valuable

E → Estimable

S → Small

T → Testable
```

------------------------------------------------------------------------

# 12. Acceptance Criteria

Defines conditions required for a feature to be accepted.

Example:

User Story:

"User wants password reset."

Acceptance Criteria:

``` text
✓ Reset email sent

✓ Link expires

✓ New password created

✓ Login successful
```

------------------------------------------------------------------------

# 13. Use Cases

A Use Case describes interaction between:

``` text
Actor

  ↓

System

  ↓

Goal
```

Components:

-   Actor
-   Goal
-   Preconditions
-   Main Flow
-   Alternate Flow
-   Postconditions

------------------------------------------------------------------------

# 14. UML Basics

UML is used to visualize software systems.

Main diagrams:

## Structural

-   Class Diagram
-   Component Diagram
-   Deployment Diagram

## Behavioral

-   Use Case Diagram
-   Sequence Diagram
-   Activity Diagram
-   State Diagram

------------------------------------------------------------------------

# 15. Requirement Traceability Matrix (RTM)

RTM maps:

``` text
Requirement

      ↓

Design

      ↓

Code

      ↓

Test Case
```

Purpose:

-   Ensure coverage
-   Track changes
-   Support testing

------------------------------------------------------------------------

# 16. Types of Traceability

## Forward Traceability

Requirement → Test Case

Purpose:

Ensure every requirement is tested.

------------------------------------------------------------------------

## Backward Traceability

Test Case → Requirement

Purpose:

Ensure every test has a valid requirement.

------------------------------------------------------------------------

# 17. Requirement Validation

Validation checks whether requirements are:

``` text
✓ Correct

✓ Complete

✓ Consistent

✓ Feasible

✓ Testable
```

------------------------------------------------------------------------

# 18. Verification vs Validation

  Verification                 Validation
  ---------------------------- ------------------------------------
  Are we building correctly?   Are we building the right product?
  Document focused             User focused
  Reviews                      User acceptance

------------------------------------------------------------------------

# 19. Requirement Engineering in SDLC

``` text
Planning

 ↓

Requirement Engineering

 ↓

Design

 ↓

Development

 ↓

Testing

 ↓

Deployment

 ↓

Maintenance
```

------------------------------------------------------------------------

# 20. Common Requirement Problems

## Ambiguous Requirements

Problem:

Different interpretations.

Solution:

Use clear language.

------------------------------------------------------------------------

## Missing Requirements

Problem:

Important features ignored.

Solution:

Perform proper elicitation.

------------------------------------------------------------------------

## Changing Requirements

Problem:

Business needs evolve.

Solution:

Use requirement management.

------------------------------------------------------------------------

# 21. Industry Example

## Banking System

Functional:

-   Account creation
-   Money transfer
-   Transaction history

Non Functional:

-   Encryption
-   High availability
-   Fast response

User Story:

    As a customer,
    I want secure money transfer,
    so that I can send payments safely.

Acceptance Criteria:

``` text
✓ Authentication required

✓ Transaction validated

✓ Confirmation generated
```

------------------------------------------------------------------------

# 22. Interview Quick Revision

## What is Requirement Engineering?

Process of managing software requirements.

------------------------------------------------------------------------

## What are requirement types?

-   Functional
-   Non Functional

------------------------------------------------------------------------

## What is SRS?

Document containing software requirements.

------------------------------------------------------------------------

## What is RTM?

A matrix connecting requirements with implementation and testing.

------------------------------------------------------------------------

## Why validate requirements?

To ensure correctness and avoid costly changes.

------------------------------------------------------------------------

# Complete Requirement Engineering Memory Map

``` text
                 REQUIREMENTS

                       |
        --------------------------------

        Elicitation
             |
        Analysis
             |
        Specification
             |
        Validation
             |
        Management


        Requirement Types

             |
     -------------------
     |                 |
 Functional       Non Functional


        Supporting Tools

             |
     -------------------------
     |          |            |
  Use Case    UML          RTM
```

------------------------------------------------------------------------

# Part 7 Summary

You now understand:

✓ Requirement Engineering\
✓ Requirement Elicitation\
✓ Stakeholder Analysis\
✓ Functional Requirements\
✓ Non Functional Requirements\
✓ Use Cases\
✓ User Stories\
✓ Acceptance Criteria\
✓ UML Basics\
✓ Requirement Traceability Matrix\
✓ Requirement Validation

Requirement Engineering ensures teams build the correct software by
understanding, documenting, validating, and managing stakeholder needs
before and during development.

------------------------------------------------------------------------

# Next Topic

## Part 8 --- Software Design Fundamentals

Upcoming lessons:

-   Introduction to Software Design
-   Design Principles
-   SOLID Principles
-   Architecture Basics
-   Design Patterns
-   High Level Design
-   Low Level Design
