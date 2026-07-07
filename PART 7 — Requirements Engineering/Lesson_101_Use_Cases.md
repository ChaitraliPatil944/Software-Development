# Lesson 101 — Use Cases

# Part 7 — Requirements Engineering

> **Objective**
>
> Understand Use Cases, their purpose, components, actors, system boundaries, Use Case diagrams, flows, and how they help teams capture functional requirements.

---

# Introduction

Before building software, teams need to understand how users interact with the system.

Use Cases describe:

- Who uses the system?
- What actions can they perform?
- How does the system respond?

```text
User

  ↓

Use Case

  ↓

System Behavior
```

---

# What is a Use Case?

A **Use Case** describes a sequence of interactions between an actor and a system to achieve a specific goal.

It represents:

**How a user achieves something using the system**

---

# Real-Life Example

## ATM System

User Goal:

Withdraw money.

Use Case:

"Withdraw Cash"

Actor:

Customer

System:

ATM Machine

Flow:

```text
Customer inserts card

        ↓

System verifies PIN

        ↓

Customer enters amount

        ↓

System provides cash
```

---

# Why Do We Need Use Cases?

Without Use Cases:

```text
Requirements

      ↓

Unclear User Interaction

      ↓

Wrong Features
```

Use Cases help:

- Understand user goals
- Define system behavior
- Identify missing requirements
- Create test scenarios
- Improve communication

---

# Components of a Use Case

A Use Case contains:

```text
Use Case Name

Actor

Goal

Preconditions

Main Flow

Alternate Flow

Postconditions
```

---

# 1. Actor

An actor is anyone or anything interacting with the system.

Actors can be:

## Human Actors

Examples:

- Customer
- Admin
- Employee

---

## External Systems

Examples:

- Payment Gateway
- Email Service
- Authentication System

---

# 2. Goal

The objective the actor wants to achieve.

Example:

Actor:

Customer

Goal:

Purchase product

---

# 3. Preconditions

Conditions that must exist before the Use Case starts.

Example:

Login Use Case:

Precondition:

User account exists.

---

# 4. Main Flow

The normal successful interaction.

Example:

Login:

```text
1. User enters username

2. User enters password

3. System validates credentials

4. User gets access
```

---

# 5. Alternate Flow

Different paths or exceptions.

Example:

Login:

```text
Wrong Password

        ↓

System Shows Error

        ↓

User Tries Again
```

---

# 6. Postconditions

The final result after completion.

Example:

Login:

User is authenticated.

---

# Use Case Diagram

A Use Case Diagram shows:

- Actors
- System functions
- Relationships

Example:

```text
          Customer

             |
             |
        -------------
        |           |
     Login       Payment
        |           |
        -------------
             |
          Banking System
```

---

# Elements of Use Case Diagram

## Actor

Represented as external user/entity.

Example:

Customer

---

## Use Case

Represents system functionality.

Example:

Login

---

## System Boundary

Defines what belongs inside the system.

Example:

```text
-------------------------
|   Banking System       |
|                       |
|  Login                |
|  Transfer Money       |
|  Balance Check        |
|                       |
-------------------------

Customer
```

---

# Relationships in Use Cases

## Association

Shows interaction between actor and use case.

Example:

Customer → Login

---

## Include Relationship

One use case always uses another.

Example:

```text
Checkout

   includes

Payment
```

---

## Extend Relationship

Optional behavior added under certain conditions.

Example:

```text
Login

   extends

Two Factor Authentication
```

---

# Use Case Example

## Online Shopping System

Actor:

Customer

Use Case:

Place Order

Preconditions:

- User logged in
- Product available

Main Flow:

```text
Search Product

        ↓

Add to Cart

        ↓

Make Payment

        ↓

Order Confirmed
```

Alternate Flow:

Payment Failure

        ↓

Retry Payment

Postcondition:

Order created.

---

# Use Case vs User Story

| Use Case | User Story |
|---|---|
| Detailed interaction | Short requirement |
| Describes system behavior | Describes user need |
| Used in analysis/design | Used in Agile backlog |
| Includes flows | Simple format |

---

# Use Case vs Functional Requirement

| Use Case | Functional Requirement |
|---|---|
| Describes interaction | Describes system capability |
| Actor-focused | System-focused |
| Scenario based | Feature based |

---

# Industry Example

## Banking Application

Actors:

- Customer
- Bank Employee
- Admin

Use Cases:

Customer:

- Login
- Transfer Money
- View Balance

Employee:

- Approve Requests

Admin:

- Manage Users

---

# Common Mistakes

## Mistake 1

Writing technical details instead of user goals.

Wrong:

"Database updates transaction table."

Better:

"Customer transfers money."

---

## Mistake 2

Ignoring alternate flows.

Solution:

Consider errors and exceptions.

---

## Mistake 3

Missing actors.

Solution:

Identify everyone interacting with the system.

---

# Best Practices

- Focus on user goals
- Define clear actors
- Include alternate scenarios
- Keep system boundary clear
- Review with stakeholders
- Link use cases with testing

---

# Interview Questions

1. What is a Use Case?
2. Why are Use Cases used?
3. What are actors?
4. Explain Use Case Diagram.
5. Difference between Use Case and User Story?
6. What is include relationship?
7. What is extend relationship?

---

# Cheat Sheet

```text
Use Case

Actor
  ↓
Goal
  ↓
Interaction
  ↓
System Response
  ↓
Result
```

---

# Summary

Use Cases provide a structured way to describe how users interact with software systems. They capture actors, goals, workflows, and system responses, helping developers, testers, and stakeholders understand functional requirements clearly before implementation begins.
