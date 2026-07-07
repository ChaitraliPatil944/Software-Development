# Lesson 126 --- State Diagrams

# Part 8 --- Software Design

> **Objective**
>
> Understand State Diagrams, state machine concepts, states,
> transitions, events, actions, notation, and how they represent the
> lifecycle of objects in software systems.

------------------------------------------------------------------------

# Introduction

Many software objects change their behavior based on their current
condition.

Examples:

-   Order status
-   User account status
-   Payment status
-   Device status

State Diagrams help represent these changes.

``` text
Object

 ↓

Different States

 ↓

State Changes

 ↓

System Behavior
```

------------------------------------------------------------------------

# What is a State Diagram?

A **State Diagram** is a UML behavioral diagram that shows different
states of an object and how it transitions from one state to another
based on events.

It represents:

-   States
-   Events
-   Transitions
-   Actions

------------------------------------------------------------------------

# Why Do We Need State Diagrams?

Without state modeling:

``` text
Object Behavior

        ↓

Unexpected State Changes

        ↓

System Errors
```

State diagrams help:

-   Understand object lifecycle
-   Model event-driven systems
-   Define valid transitions
-   Prevent invalid operations
-   Improve system design

------------------------------------------------------------------------

# State Machine Concept

A state machine consists of:

``` text
State

  +

Event

  +

Transition

  +

Action
```

------------------------------------------------------------------------

# 1. State

A state represents a condition or situation of an object.

Examples:

Order:

    Created

    Paid

    Shipped

    Delivered

------------------------------------------------------------------------

# 2. Event

An event causes a state change.

Example:

    Payment Completed

            ↓

    Order moves from

    Created → Paid

------------------------------------------------------------------------

# 3. Transition

A transition represents movement between states.

Example:

    Pending

       |

    Payment Received

       ↓

    Completed

------------------------------------------------------------------------

# 4. Action

An action is performed during a transition.

Example:

    Payment Successful

            ↓

    Send Confirmation Email

------------------------------------------------------------------------

# State Diagram Notation

## Initial State

Represents starting point.

Symbol:

    ●

------------------------------------------------------------------------

## State

Represents condition.

Example:

    +-----------+
    | Processing|
    +-----------+

------------------------------------------------------------------------

## Transition

Arrow between states.

Example:

    State A

      ----->

    State B

------------------------------------------------------------------------

## Final State

Represents completion.

Symbol:

    ◎

------------------------------------------------------------------------

# Basic State Diagram Example

## Order Management System

``` text
        ●

        ↓

     Created

        |

 Order Confirmed

        ↓

      Paid

        |

 Shipped

        ↓

    Delivered

        ↓

        ◎
```

------------------------------------------------------------------------

# Example: Online Payment System

States:

    Initiated

        ↓

    Processing

        ↓

    Successful

Failure path:

    Processing

        ↓

    Failed

Diagram:

``` text
        ●

        ↓

   Initiated

        ↓

  Processing

     /      \

Success    Failed

   ↓          ↓

Completed   Retry
```

------------------------------------------------------------------------

# Example: User Account Lifecycle

``` text
New User

   ↓

Active

   ↓

Suspended

   ↓

Deleted
```

Events:

-   Registration
-   Account violation
-   Deletion request

------------------------------------------------------------------------

# State Diagram vs Activity Diagram

  State Diagram       Activity Diagram
  ------------------- --------------------
  Object lifecycle    Process workflow
  Focuses on states   Focuses on actions
  Event driven        Flow driven

------------------------------------------------------------------------

# State Diagram vs Sequence Diagram

  State Diagram         Sequence Diagram
  --------------------- ------------------------------
  Shows object states   Shows object communication
  Focuses on changes    Focuses on interaction order

------------------------------------------------------------------------

# State Diagrams in Software Design

Used for:

-   Workflow systems
-   Embedded systems
-   User accounts
-   Payment systems
-   Order management
-   Device control systems

------------------------------------------------------------------------

# Industry Example

## Banking Transaction

States:

``` text
Initiated

    ↓

Processing

    ↓

Approved

    ↓

Completed
```

Failure:

``` text
Processing

    ↓

Rejected
```

------------------------------------------------------------------------

# Benefits of State Diagrams

-   Clarifies object behavior
-   Identifies invalid states
-   Improves system reliability
-   Helps event-driven design
-   Simplifies complex workflows

------------------------------------------------------------------------

# Limitations

-   Can become complex for large systems
-   Not useful for simple objects
-   Requires proper state identification

------------------------------------------------------------------------

# Common Mistakes

## Mistake 1

Creating too many states.

Solution:

Include only meaningful states.

------------------------------------------------------------------------

## Mistake 2

Missing transition conditions.

Solution:

Define events clearly.

------------------------------------------------------------------------

## Mistake 3

Ignoring invalid transitions.

Solution:

Identify all possible scenarios.

------------------------------------------------------------------------

# Best Practices

-   Identify important object lifecycle
-   Define clear states
-   Document transition events
-   Avoid unnecessary complexity
-   Validate with business rules

------------------------------------------------------------------------

# Interview Questions

1.  What is a State Diagram?
2.  Why are state diagrams used?
3.  Explain state, event, and transition.
4.  Difference between state and activity diagrams?
5.  What is a state machine?
6.  Give a real-world example of a state diagram.
7.  How do state diagrams improve software design?

------------------------------------------------------------------------

# Cheat Sheet

``` text
State Diagram

Initial State

      ↓

State

      ↓

Event

      ↓

Transition

      ↓

Final State
```

------------------------------------------------------------------------

# Summary

State Diagrams model the lifecycle and behavior changes of objects in a
software system. By representing states, events, and transitions, they
help developers design reliable event-driven systems and prevent invalid
object behavior.
