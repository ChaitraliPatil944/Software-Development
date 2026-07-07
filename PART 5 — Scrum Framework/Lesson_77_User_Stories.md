# Lesson 77 — User Stories

# Part 5 — Scrum Framework

> **Objective**
>
> Understand User Stories in depth, why Agile uses them, their structure, INVEST criteria, acceptance criteria, examples, and how teams convert customer needs into development work.

---

# Introduction

Software is built for users.

Instead of starting with technical features, Agile starts by understanding:

- Who needs something?
- What do they need?
- Why does it matter?

This is represented using **User Stories**.

```text
User Need
    ↓
User Story
    ↓
Development Work
    ↓
Product Value
```

---

# What is a User Story?

A **User Story** is a short description of a software requirement written from the perspective of the user.

It explains:

- Who needs something
- What they need
- Why they need it

---

# User Story Format

The standard format is:

```text
As a <user>,
I want <feature>,
so that <benefit>.
```

---

# Example

Feature:

Online Payment

User Story:

```
As a customer,
I want to pay online,
so that I can complete my order quickly.
```

---

# Why Do We Need User Stories?

Traditional Requirement:

```
Implement payment API.
```

Problem:

It explains the technical task, not the user value.

User Story:

```
As a customer,
I want secure payments,
so that I can purchase products safely.
```

Benefits:

- Focuses on user needs
- Improves communication
- Helps prioritization

---

# Components of User Story

## 1. User

Who needs the feature?

Examples:

- Customer
- Admin
- Employee
- Doctor

---

## 2. Action

What does the user want?

Examples:

- Search products
- Upload documents
- Reset password

---

## 3. Benefit

Why does the user need it?

Examples:

- Save time
- Improve security
- Complete tasks faster

---

# User Story Example

## Food Delivery Application

```
As a customer,
I want to track my order,
so that I know when it will arrive.
```

User:

Customer

Action:

Track order

Benefit:

Know delivery status

---

# INVEST Criteria

A good User Story follows INVEST.

```text
I → Independent
N → Negotiable
V → Valuable
E → Estimable
S → Small
T → Testable
```

---

# I — Independent

A story should not depend heavily on another story.

Bad:

"Complete payment after login system."

Better:

Separate login and payment stories.

---

# N — Negotiable

A User Story describes the need, not the exact solution.

Example:

Need:

"Customer needs secure login."

Solution can be discussed.

---

# V — Valuable

Every story should provide user or business value.

---

# E — Estimable

The team should understand enough to estimate effort.

---

# S — Small

Large stories should be broken down.

Example:

Large:

"Build E-Commerce Platform"

Small:

- User Registration
- Product Search
- Cart
- Payment

---

# T — Testable

A story must have clear validation.

Example:

Login Story:

✓ User enters valid credentials  
✓ User accesses dashboard

---

# Acceptance Criteria

Acceptance Criteria define when a User Story is complete.

Example:

User Story:

"As a user, I want password reset."

Acceptance Criteria:

```
✓ User receives reset email
✓ Link expires after time limit
✓ New password can be created
```

---

# User Story Workflow

```text
Customer Need

      ↓

User Story Creation

      ↓

Backlog

      ↓

Estimation

      ↓

Sprint Selection

      ↓

Development

      ↓

Testing

      ↓

Done
```

---

# Epic vs Feature vs User Story vs Task

| Level | Example |
|---|---|
| Epic | Online Shopping |
| Feature | Payment System |
| User Story | Customer pays online |
| Task | Create payment API |

---

# Industry Example

## Banking Application

Epic:

Mobile Banking

Feature:

Fund Transfer

User Story:

```
As a customer,
I want to transfer money,
so that I can send payments easily.
```

Tasks:

- Create transfer API
- Build UI
- Add security checks
- Test transactions

---

# Common Mistakes

## Mistake 1

Writing technical tasks as stories.

Wrong:

"Create database table."

Better:

"As an admin, I want to manage users."

---

## Mistake 2

Making stories too large.

Solution:

Split into smaller stories.

---

## Mistake 3

Missing acceptance criteria.

Solution:

Define completion clearly.

---

# Interview Questions

1. What is a User Story?
2. Why does Agile use User Stories?
3. Explain User Story format.
4. What is INVEST criteria?
5. Difference between Epic and User Story?
6. What are Acceptance Criteria?
7. Who writes User Stories?

---

# Cheat Sheet

```text
User Story

Who?
 ↓
What?
 ↓
Why?

As a User
I want Feature
So that Benefit
```

---

# Summary

User Stories help Agile teams understand software requirements from the user's perspective. They shift the focus from technical tasks to customer value. By following the INVEST criteria and defining clear acceptance criteria, teams create better backlog items that are easier to estimate, develop, and test.
