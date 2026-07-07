# Lesson 124 --- Sequence Diagrams

# Part 8 --- Software Design

> **Objective**
>
> Understand Sequence Diagrams, their purpose in software design,
> objects, lifelines, messages, interaction flow, communication types,
> and how they help model system behavior.

------------------------------------------------------------------------

# Introduction

Software systems contain multiple components that communicate with each
other.

Before implementation, developers need to understand:

-   Which objects interact?
-   In what order do interactions happen?
-   How does data flow between components?

Sequence Diagrams represent these interactions visually.

``` text
User Request

      ↓

Object Interaction

      ↓

System Response
```

------------------------------------------------------------------------

# What is a Sequence Diagram?

A **Sequence Diagram** is a UML behavioral diagram that shows how
objects communicate with each other over time.

It represents:

-   Objects
-   Messages
-   Order of interactions
-   Time sequence

------------------------------------------------------------------------

# Why Do We Need Sequence Diagrams?

Without interaction modeling:

``` text
Multiple Components

        ↓

Unclear Communication

        ↓

Design Errors
```

Sequence diagrams help:

-   Understand system behavior
-   Design APIs
-   Identify object responsibilities
-   Document workflows
-   Improve communication

------------------------------------------------------------------------

# Sequence Diagram Structure

Main components:

``` text
Sequence Diagram

        |
-------------------
|        |        |
Objects Lifelines Messages
```

------------------------------------------------------------------------

# 1. Objects

Objects represent system components involved in interaction.

Examples:

-   User
-   Controller
-   Service
-   Database

Representation:

    User

    LoginController

    Database

------------------------------------------------------------------------

# 2. Lifeline

A lifeline represents the existence of an object during interaction.

Example:

    User

     |

     |

     |

The vertical line shows time progression.

------------------------------------------------------------------------

# 3. Messages

Messages represent communication between objects.

Example:

    User

      -------->

    Controller

Types:

-   Request
-   Response
-   Method call

------------------------------------------------------------------------

# Sequence Diagram Notation

Basic structure:

    Object A          Object B

       |                 |
       |---- Request --->|
       |                 |
       |<--- Response ---|
       |                 |

Time moves from top to bottom.

------------------------------------------------------------------------

# Example 1 --- Login System

Sequence:

``` text
User

 |

 | Enter Credentials

 ↓

Login Controller

 |

 | Validate User

 ↓

Database

 |

 | User Found

 ↓

Login Controller

 |

 | Success Response

 ↓

User
```

------------------------------------------------------------------------

# Example 2 --- Online Payment

``` text
Customer

    |

    | Payment Request

    ↓

Order Service

    |

    | Process Payment

    ↓

Payment Gateway

    |

    | Confirmation

    ↓

Order Service

    |

    | Order Completed

    ↓

Customer
```

------------------------------------------------------------------------

# Types of Messages

## 1. Synchronous Message

Sender waits for response.

Example:

    Application

          |

          | Request

          ↓

    Database

------------------------------------------------------------------------

## 2. Asynchronous Message

Sender does not wait.

Example:

    Order Service

          |

          | Send Notification

          ↓

    Email Service

------------------------------------------------------------------------

# Activation Bar

Shows when an object is performing an operation.

Example:

    Controller

        |

       [====]

        |

     Database

------------------------------------------------------------------------

# Sequence Diagram in API Design

Example:

REST API:

    Client

     ↓

    Controller

     ↓

    Service

     ↓

    Repository

     ↓

    Database

Shows:

-   Request flow
-   Processing logic
-   Response path

------------------------------------------------------------------------

# Sequence Diagram Example: Banking Transfer

Objects:

    Customer

    Bank App

    Transaction Service

    Database

Flow:

    Customer

     ↓

    Transfer Request

     ↓

    Transaction Service

     ↓

    Check Balance

     ↓

    Database

     ↓

    Update Transaction

     ↓

    Confirmation

------------------------------------------------------------------------

# Sequence Diagram vs Activity Diagram

  Sequence Diagram           Activity Diagram
  -------------------------- -----------------------
  Shows object interaction   Shows workflow
  Time-based                 Process-based
  Focuses on communication   Focuses on activities

------------------------------------------------------------------------

# Sequence Diagram vs Flowchart

  Sequence Diagram       Flowchart
  ---------------------- --------------------------
  Object communication   Process logic
  UML diagram            Algorithm representation
  Shows interactions     Shows steps

------------------------------------------------------------------------

# Benefits of Sequence Diagrams

-   Clarifies object communication
-   Helps API design
-   Identifies missing interactions
-   Improves system understanding
-   Supports debugging

------------------------------------------------------------------------

# Limitations

-   Large systems create complex diagrams
-   Requires updating when design changes
-   Not ideal for every scenario

------------------------------------------------------------------------

# Common Mistakes

## Mistake 1

Adding too many details.

Solution:

Focus on important interactions.

------------------------------------------------------------------------

## Mistake 2

Wrong object responsibility.

Solution:

Assign clear responsibilities.

------------------------------------------------------------------------

## Mistake 3

Ignoring alternate flows.

Solution:

Include error scenarios.

------------------------------------------------------------------------

# Best Practices

-   Identify important objects first
-   Keep interactions clear
-   Use meaningful names
-   Model main and alternate flows
-   Update diagrams with design changes

------------------------------------------------------------------------

# Industry Example

## E-Commerce Order Processing

Sequence:

    Customer

     ↓

    Shopping Cart

     ↓

    Order Service

     ↓

    Payment Service

     ↓

    Inventory Service

     ↓

    Confirmation Service

------------------------------------------------------------------------

# Interview Questions

1.  What is a Sequence Diagram?
2.  Why are sequence diagrams used?
3.  What are lifelines?
4.  Explain messages in sequence diagrams.
5.  Difference between synchronous and asynchronous messages?
6.  Difference between sequence and activity diagrams?
7.  How are sequence diagrams useful in API design?

------------------------------------------------------------------------

# Cheat Sheet

``` text
Sequence Diagram

Objects

   ↓

Messages

   ↓

Interaction Order

   ↓

System Behavior
```

------------------------------------------------------------------------

# Summary

Sequence Diagrams are UML behavioral diagrams that represent how objects
communicate over time. They help developers understand workflows, design
APIs, assign responsibilities, and visualize interactions before
implementation. They are especially useful when designing complex
systems with multiple interacting components.
