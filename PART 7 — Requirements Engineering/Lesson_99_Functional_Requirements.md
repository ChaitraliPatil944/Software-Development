# Lesson 99 — Functional Requirements

# Part 7 — Requirements Engineering

> **Objective**
>
> Understand Functional Requirements, their purpose, characteristics, structure, examples, and how they define what a software system should do.

---

# Introduction

Every software system exists to perform certain tasks.

Before development begins, teams must clearly define:

- What actions should the system perform?
- What features should users have?
- What operations should the software support?

These are captured as **Functional Requirements**.

```text
User Need

     ↓

Functional Requirement

     ↓

Software Feature

     ↓

Working System
```

---

# What are Functional Requirements?

**Functional Requirements** describe the specific behaviors, features, and operations that a software system must provide.

They define:

**What the system should do**

---

# Examples

## Banking Application

Functional Requirements:

- User can create an account
- User can transfer money
- User can view transaction history
- System generates account statements

---

## E-Commerce Application

Functional Requirements:

- User can search products
- User can add items to cart
- User can place orders
- User can make payments

---

# Why Do We Need Functional Requirements?

Without clear functional requirements:

```text
Unclear Features

        ↓

Wrong Implementation

        ↓

Customer Dissatisfaction

        ↓

Rework
```

Functional requirements help:

- Guide developers
- Create test cases
- Define project scope
- Validate customer expectations

---

# Characteristics of Good Functional Requirements

A good functional requirement should be:

## 1. Clear

Easy to understand.

Bad:

"The system should handle users."

Good:

"The system should allow users to create accounts using email and password."

---

## 2. Complete

Contains all necessary details.

---

## 3. Consistent

Should not conflict with other requirements.

---

## 4. Testable

Can be verified through testing.

Example:

Requirement:

"User can login."

Test:

Enter valid credentials and verify access.

---

## 5. Traceable

Can be tracked from requirement to implementation and testing.

---

# Functional Requirement Structure

A functional requirement usually contains:

```text
Requirement ID

Description

Input

Processing

Expected Output

Priority
```

---

# Example Functional Requirement

## Requirement ID

FR-001

## Description

User login functionality.

## Input

Username and password.

## Processing

System validates credentials.

## Output

User accesses dashboard.

---

# Types of Functional Requirements

## 1. User Management

Examples:

- Registration
- Login
- Password reset
- Profile update

---

## 2. Data Processing

Examples:

- Calculations
- Data storage
- Report generation

---

## 3. Transaction Handling

Examples:

- Payments
- Orders
- Transfers

---

## 4. System Interaction

Examples:

- API communication
- Notifications
- External integrations

---

# Functional Requirements in SDLC

```text
Requirement Phase

        ↓

Functional Requirements

        ↓

System Design

        ↓

Development

        ↓

Testing

        ↓

Deployment
```

---

# Functional Requirements and Testing

Functional requirements directly create test cases.

Example:

Requirement:

"User should be able to reset password."

Test Cases:

✓ Reset link generated

✓ Email sent successfully

✓ New password accepted

---

# Functional vs Non Functional Requirements

| Functional Requirements | Non Functional Requirements |
|---|---|
| What system does | How system performs |
| Features and operations | Quality attributes |
| User actions | Performance and security |
| Example: Login | Example: Response time |

---

# Industry Example

## Online Learning Platform

Functional Requirements:

Student:

- Register account
- Search courses
- Watch videos
- Take exams

Instructor:

- Upload courses
- Manage content

Admin:

- Manage users
- Generate reports

---

# Common Mistakes

## Mistake 1

Writing vague requirements.

Wrong:

"System should be user friendly."

Better:

"System should allow users to complete registration within three steps."

---

## Mistake 2

Mixing functional and non-functional requirements.

Wrong:

"System should load quickly."

This is performance-related.

---

## Mistake 3

Ignoring edge cases.

Example:

What happens if login credentials are incorrect?

---

# Best Practices

- Use simple language
- Assign unique IDs
- Include acceptance criteria
- Review with stakeholders
- Keep requirements testable
- Maintain traceability

---

# Interview Questions

1. What are Functional Requirements?
2. What do Functional Requirements describe?
3. Give examples of Functional Requirements.
4. Difference between Functional and Non Functional Requirements?
5. Why should Functional Requirements be testable?
6. How are Functional Requirements used in testing?
7. How do you write a good Functional Requirement?

---

# Cheat Sheet

```text
Functional Requirements

Define:

WHAT the system does


Examples:

Login
Payment
Search
Reports
Notifications
```

---

# Summary

Functional Requirements define the core behavior and features of a software system. They describe what users can do and what operations the system must perform. Clear, complete, and testable functional requirements provide a foundation for design, development, and testing while reducing misunderstandings between stakeholders and developers.
