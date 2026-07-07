# Lesson 27 — Development Phase

# Part 2 — Software Development Life Cycle (SDLC)

> **Objective**
>
> Understand how software is built during the Development Phase, the activities involved, industry workflows, coding standards, collaboration practices, and the deliverables produced before testing.

---

# Introduction

After the Design Phase is complete, the team finally starts writing code.

At this point, developers already have:

- Approved SRS
- High-Level Design (HLD)
- Low-Level Design (LLD)
- Database Design
- API Specifications
- UI Designs

The Development Phase transforms these documents into a working software product.

---

# What is the Development Phase?

The **Development Phase** is the SDLC stage where software engineers implement the approved design by writing, integrating, reviewing, and building source code.

```text
Design
   |
Coding
   |
Build
   |
Working Software
```

---

# Why is the Development Phase Important?

Good development practices ensure software is:

- Correct
- Maintainable
- Secure
- Scalable
- Easy to test

Poor coding practices create technical debt and increase future maintenance costs.

---

# Development Workflow

```text
Approved Design
        |
Task Assignment
        |
Coding
        |
Unit Testing
        |
Code Review
        |
Merge
        |
Build
        |
Testing Phase
```

---

# Activities in the Development Phase

## 1. Task Breakdown

Large features are divided into smaller development tasks.

Example:

```text
Shopping Cart
   |
------------------------
| Add Item
| Remove Item
| Update Quantity
| Checkout
```

---

## 2. Coding

Developers implement features according to design documents.

Example technologies:

- Java
- C#
- Python
- JavaScript
- Go
- C++

---

## 3. Version Control

Every change is tracked using Git.

```text
Repository
     |
Feature Branch
     |
Commit
     |
Pull Request
     |
Merge
```

Benefits:

- Collaboration
- History
- Rollback
- Parallel development

---

## 4. Unit Testing

Developers verify individual functions or modules.

```text
Function
    |
Unit Test
    |
Pass
```

Testing early reduces bugs later.

---

## 5. Code Review

Another developer reviews the code.

Checklist:

- Readability
- Correctness
- Security
- Performance
- Coding standards

Code reviews improve quality and spread knowledge.

---

## 6. Build Process

Source code is compiled or packaged.

```text
Source Code
      |
Build Tool
      |
Executable / Package
```

Examples:

- Maven
- Gradle
- npm
- MSBuild

---

## 7. Integration

Modules are combined into one application.

```text
Login
   |
Cart
   |
Payment
   |
Orders
```

Integration verifies that components work together.

---

# Coding Standards

Professional teams follow standards such as:

- Meaningful variable names
- Consistent formatting
- Small functions
- Proper comments
- Error handling
- Logging

Good code is written for humans first and computers second.

---

# Industry Workflow

```text
Sprint Planning
      |
Developer Picks Task
      |
Create Branch
      |
Code
      |
Unit Test
      |
Commit
      |
Pull Request
      |
Code Review
      |
Merge
      |
Build
      |
QA Testing
```

---

# Collaboration

Typical participants:

```text
Product Owner
      |
Scrum Master
      |
Developers
      |
QA Engineers
      |
DevOps Engineers
```

Developers collaborate continuously throughout implementation.

---

# Deliverables

Outputs include:

- Source Code
- Unit Tests
- Build Artifacts
- Technical Documentation
- Updated Repository
- Release Candidate

---

# Industry Example

## Food Delivery Platform

Frontend Team:

- Login Screen
- Restaurant List
- Cart
- Checkout

Backend Team:

- Authentication API
- Payment API
- Order API
- Notification Service

Database Team:

- Tables
- Indexes
- Stored Procedures

All work is integrated before testing.

---

# Common Challenges

- Merge conflicts
- Misunderstood requirements
- Poor code quality
- Tight deadlines
- Technical debt
- Dependency issues

---

# Best Practices

- Commit frequently
- Write clean code
- Follow coding standards
- Review code
- Write unit tests
- Keep branches small
- Document important decisions

---

# Common Mistakes

❌ Coding without understanding requirements.

✔ Read the SRS and design first.

❌ Large commits after several days.

✔ Make small, meaningful commits.

❌ Skipping code reviews.

✔ Review every significant change.

❌ Ignoring unit testing.

✔ Test before merging.

---

# Inputs & Outputs

| Input | Output |
|-------|--------|
| SRS | Source Code |
| HLD | Unit Tests |
| LLD | Build Artifacts |
| Database Design | Updated Repository |
| API Design | Release Candidate |

---

# Interview Questions

1. What happens during the Development Phase?
2. Why is version control important?
3. What is code review?
4. Why should developers write unit tests?
5. What are coding standards?
6. What are the outputs of the Development Phase?
7. Why are small commits recommended?

---

# Cheat Sheet

```text
Development Phase

Design
   ↓
Coding
   ↓
Unit Testing
   ↓
Code Review
   ↓
Commit
   ↓
Merge
   ↓
Build
   ↓
Testing

Outputs

✓ Source Code
✓ Unit Tests
✓ Build
✓ Repository
```

---

# Summary

The Development Phase transforms software designs into working applications through coding, version control, unit testing, code reviews, integration, and build processes. By following disciplined engineering practices and collaborating effectively, development teams produce reliable, maintainable software that is ready for comprehensive testing and deployment.
