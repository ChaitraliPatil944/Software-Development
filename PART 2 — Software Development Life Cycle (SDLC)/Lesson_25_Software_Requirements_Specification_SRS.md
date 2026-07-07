# Lesson 25 — Software Requirements Specification (SRS)

# Part 2 — Software Development Life Cycle (SDLC)

> **Objective**
>
> Understand what an SRS (Software Requirements Specification) document is, why it is one of the most important deliverables in SDLC, how it is structured, and how it guides the entire software development process.

---

# Introduction

Imagine a customer says:

> "Build me an online shopping application."

The development team asks:

- What features are required?
- Who are the users?
- What performance is expected?
- What security is needed?
- How will success be measured?

If these answers exist only in conversations, misunderstandings are inevitable.

The solution is a formal document called the **Software Requirements Specification (SRS).**

---

# What is an SRS?

A **Software Requirements Specification (SRS)** is a formal document that describes **what a software system should do** and **the constraints under which it must operate**.

It acts as the single source of truth for everyone involved in the project.

```text
Business Idea
      |
Requirement Gathering
      |
Requirement Analysis
      |
      SRS
      |
-------------------------------
| Architect
| Developers
| QA
| DevOps
| Customer
```

---

# Why is an SRS Important?

Without an SRS:

```text
Customer Says A
      |
Developer Understands B
      |
Software Becomes C
```

With an SRS:

```text
Customer
     |
Approved SRS
     |
Entire Team
     |
Same Understanding
```

Benefits:

- Clear communication
- Reduced ambiguity
- Better estimation
- Easier testing
- Better maintenance
- Contract between customer and development team

---

# Objectives of an SRS

- Clearly define requirements
- Reduce misunderstandings
- Support design and development
- Help testing teams create test cases
- Simplify maintenance
- Improve project estimation

---

# IEEE SRS Structure (Simplified)

```text
SRS
|
+-- 1. Introduction
+-- 2. Overall Description
+-- 3. Functional Requirements
+-- 4. Non-Functional Requirements
+-- 5. External Interfaces
+-- 6. Constraints
+-- 7. Assumptions
+-- 8. Appendices
```

---

# 1. Introduction

Contains:

- Purpose
- Scope
- Definitions
- References
- Document overview

Example:

Project:
Online Shopping System

Purpose:
Provide an e-commerce platform for customers.

---

# 2. Overall Description

Describes:

- Product perspective
- User classes
- Operating environment
- Assumptions
- Constraints

---

# 3. Functional Requirements

Examples:

FR-001 User Registration

FR-002 User Login

FR-003 Search Products

FR-004 Add to Cart

FR-005 Online Payment

Each requirement has:

- ID
- Description
- Priority
- Acceptance Criteria

---

# 4. Non-Functional Requirements

Examples:

- Homepage loads within 2 seconds
- 99.99% availability
- AES-256 encryption
- Support 100,000 concurrent users

---

# 5. External Interface Requirements

Examples:

User Interface

```text
User
 |
Web Browser
 |
Website
```

Software Interfaces

- Payment Gateway
- Email Service
- SMS API

Hardware Interfaces

- Barcode Scanner
- Printer
- Biometric Device

Communication Interfaces

- HTTPS
- REST APIs
- WebSockets

---

# 6. Constraints

Examples:

- Must use Java
- Must deploy on AWS
- Budget ₹20 lakh
- Completion in 6 months

Constraints limit design choices.

---

# 7. Assumptions

Examples:

- Internet connection available
- Users have smartphones
- Third-party payment gateway remains available

---

# Requirement Traceability

Every requirement should be traceable.

```text
Business Need
      |
Requirement
      |
Design
      |
Code
      |
Test Case
      |
Deployment
```

This helps verify nothing is missed.

---

# Sample Requirement

```text
Requirement ID : FR-010

Title :
Place Order

Description :
The customer shall be able to place an order
using items available in the shopping cart.

Priority :
High

Acceptance Criteria :
- Payment succeeds
- Order created
- Confirmation email sent
```

---

# Industry Example

## Hospital Management System

The SRS contains:

Functional Requirements

- Register Patient
- Book Appointment
- Generate Bill
- Manage Pharmacy

Non-Functional Requirements

- Response time < 3 seconds
- 99.95% availability
- Encrypted patient records

Constraints

- Follow healthcare regulations
- Deploy on hospital servers

---

# Who Uses the SRS?

```text
Customer
     |
Business Analyst
     |
Product Owner
     |
Architect
     |
Developers
     |
QA Engineers
     |
Project Manager
     |
DevOps
```

Almost every stakeholder refers to the SRS.

---

# Common Mistakes

❌ Writing vague requirements.

✔ Use measurable statements.

❌ Mixing business goals with technical design.

✔ Keep requirements separate from implementation.

❌ Missing acceptance criteria.

✔ Define how every requirement will be verified.

---

# Best Practices

- Use unique IDs
- Write simple language
- Avoid ambiguity
- Make requirements testable
- Review with stakeholders
- Maintain version history

---

# Interview Questions

1. What is an SRS?
2. Why is an SRS important?
3. What are the major sections of an SRS?
4. Who prepares an SRS?
5. Who uses an SRS?
6. What is requirement traceability?
7. Differentiate Functional and Non-Functional Requirements inside an SRS.

---

# Cheat Sheet

```text
SRS

Purpose
↓
Single Source of Truth

Contains

✓ Introduction
✓ Overall Description
✓ Functional Requirements
✓ Non-Functional Requirements
✓ Interfaces
✓ Constraints
✓ Assumptions

Used By

BA
PO
Architect
Developers
QA
DevOps
Customer
```

---

# Summary

The Software Requirements Specification (SRS) is the foundation of every successful software project. It converts stakeholder expectations into a structured, testable, and agreed-upon document that guides architecture, development, testing, deployment, and maintenance. A well-written SRS reduces misunderstandings, improves communication, and ensures every team member works toward the same product vision.
