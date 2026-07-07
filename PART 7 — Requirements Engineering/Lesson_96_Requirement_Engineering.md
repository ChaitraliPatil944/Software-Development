# Lesson 96 — Requirement Engineering

# Part 7 — Requirements Engineering

> **Objective**
>
> Understand Requirement Engineering, why it is important in software projects, its activities, process, techniques, and role in building successful software systems.

---

# Introduction

Every software project starts with a problem that needs to be solved.

Before writing code, teams must understand:

- What should the software do?
- Who will use it?
- What problems should it solve?
- What constraints exist?

This process is called **Requirement Engineering**.

```text
Business Problem

        ↓

Requirements Understanding

        ↓

Software Design

        ↓

Development

        ↓

Testing

        ↓

Final Product
```

---

# What is Requirement Engineering?

**Requirement Engineering (RE)** is the systematic process of identifying, analyzing, documenting, validating, and managing software requirements.

It acts as a bridge between:

```text
Customers / Business

        ↓

Requirement Engineering

        ↓

Software Development Team
```

---

# Why Do We Need Requirement Engineering?

Without proper requirements:

```text
Unclear Requirements

        ↓

Wrong Development

        ↓

More Changes

        ↓

Higher Cost

        ↓

Project Failure
```

Good requirements help:

- Reduce misunderstandings
- Control project scope
- Improve software quality
- Reduce development cost
- Increase customer satisfaction

---

# Real-Life Example

## Food Delivery Application

Customer says:

"I want an app for ordering food."

This is not enough.

Requirement Engineering identifies:

Users:

- Customers
- Restaurants
- Delivery Partners
- Admin

Features:

- Registration
- Restaurant search
- Order placement
- Payment
- Tracking

Constraints:

- Security
- Performance
- Availability

---

# Requirement Engineering Process

```text
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

---

# 1. Requirement Elicitation

## Meaning

Collecting requirements from stakeholders.

Sources:

- Customers
- Users
- Business teams
- Domain experts

Techniques:

- Interviews
- Surveys
- Observation
- Workshops
- Brainstorming

Example:

Interviewing customers to understand banking needs.

---

# 2. Requirement Analysis

Collected requirements are analyzed.

Activities:

- Remove conflicts
- Check feasibility
- Prioritize requirements
- Identify dependencies

Example:

Requirement:

"System should process unlimited users instantly."

Analysis:

Check whether infrastructure supports this.

---

# 3. Requirement Specification

Requirements are documented clearly.

Common document:

**Software Requirement Specification (SRS)**

Contains:

- Functional requirements
- Non-functional requirements
- Constraints
- Assumptions

---

# 4. Requirement Validation

Ensures requirements are:

- Correct
- Complete
- Consistent
- Realistic
- Testable

Example:

Requirement:

"System should be fast."

Problem:

Not measurable.

Better:

"System should respond within 2 seconds."

---

# 5. Requirement Management

Requirements change during projects.

Management includes:

- Tracking changes
- Version control
- Impact analysis

---

# Types of Requirements

```text
Requirements

      |
      |
---------------------
|                   |
Functional       Non Functional
```

---

# Functional Requirements

Describe:

**What the system should do**

Examples:

- User login
- Payment processing
- Report generation

---

# Non Functional Requirements

Describe:

**How the system should perform**

Examples:

- Performance
- Security
- Reliability
- Scalability

---

# Requirement Engineering Activities

| Activity | Purpose |
|---|---|
| Elicitation | Gather requirements |
| Analysis | Understand requirements |
| Specification | Document requirements |
| Validation | Verify correctness |
| Management | Control changes |

---

# Requirement Engineering in SDLC

```text
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
```

---

# Industry Example

## Banking Software

Requirement Engineering identifies:

Functional:

- Account creation
- Money transfer
- Transaction history

Non Functional:

- Encryption
- High availability
- Fast response time

Validation ensures requirements meet banking standards.

---

# Common Problems Without Requirement Engineering

❌ Wrong features developed

❌ Increased development cost

❌ Frequent requirement changes

❌ Customer dissatisfaction

❌ Project delays

---

# Best Practices

- Involve stakeholders early
- Document clearly
- Avoid ambiguity
- Prioritize requirements
- Validate regularly
- Manage changes carefully

---

# Interview Questions

1. What is Requirement Engineering?
2. Why is Requirement Engineering important?
3. Explain Requirement Engineering phases.
4. Difference between functional and non-functional requirements?
5. What is requirement elicitation?
6. What is SRS?
7. Why do requirements change?

---

# Cheat Sheet

```text
Requirement Engineering

Elicit
  ↓
Analyze
  ↓
Specify
  ↓
Validate
  ↓
Manage
```

---

# Summary

Requirement Engineering is the foundation of software development. It ensures that teams understand customer needs before building software. Through elicitation, analysis, specification, validation, and management, Requirement Engineering reduces risks, improves communication, and helps deliver software that solves the correct problem.
