# Lesson 26 — Design Phase

# Part 2 — Software Development Life Cycle (SDLC)

> **Objective**
>
> Understand the Design Phase of the SDLC, why it is essential, what activities are performed, what documents are produced, and how software architects transform requirements into a technical blueprint.

---

# Introduction

After requirements are finalized in the SRS, developers still cannot start coding immediately.

Why?

Because they know **what** to build, but not **how** to build it.

The **Design Phase** answers:

```text
Requirements
      |
 HOW should we build it?
      |
Software Design
```

---

# What is the Design Phase?

The **Design Phase** converts approved requirements into a technical blueprint that developers can implement.

It defines:

- Architecture
- Components
- Database
- APIs
- User Interface
- Security
- Technology stack

Think of it as the architect's blueprint before constructing a building.

---

# Why is the Design Phase Needed?

Without design:

```text
Requirements
      |
Developers Start Coding
      |
Different Approaches
      |
Inconsistent System
      |
Maintenance Problems
```

With design:

```text
Requirements
      |
Architecture
      |
Modules
      |
Database
      |
APIs
      |
Coding Begins
```

Everyone follows the same plan.

---

# Design Phase Workflow

```text
Approved SRS
      |
Requirement Analysis
      |
Architecture Design
      |
Database Design
      |
API Design
      |
UI/UX Design
      |
Detailed Design
      |
Development
```

---

# Major Activities

## 1. High-Level Design (HLD)

Describes the overall architecture.

Includes:

- Major modules
- System architecture
- Technology stack
- External integrations

Example:

```text
Browser
   |
Frontend
   |
Backend API
   |
Database
```

---

## 2. Low-Level Design (LLD)

Describes internal implementation details.

Includes:

- Classes
- Methods
- Data structures
- Algorithms
- Module interactions

---

## 3. Database Design

Designs data storage.

Activities:

- Tables
- Relationships
- Keys
- Constraints
- Indexes

Example:

```text
Users
  |
Orders
  |
Payments
```

---

## 4. API Design

Defines communication between systems.

Example:

```text
Client
   |
POST /login

GET /products

POST /orders
```

---

## 5. UI/UX Design

Creates user interaction.

Deliverables:

- Wireframes
- Mockups
- Prototypes

Goal:

Simple, intuitive interfaces.

---

## 6. Security Design

Plans:

- Authentication
- Authorization
- Encryption
- Audit logging

Security should be designed early, not added later.

---

# Design Deliverables

Typical outputs:

- High-Level Design (HLD)
- Low-Level Design (LLD)
- Architecture Diagram
- Database Schema
- API Specification
- Wireframes
- UML Diagrams

---

# Stakeholders

```text
Business Analyst
      |
Software Architect
      |
UI/UX Designer
      |
Senior Developers
      |
Database Engineer
```

The customer may review UI prototypes before development begins.

---

# Industry Example

## E-Commerce Platform

Architecture:

```text
Customer
    |
Web / Mobile App
    |
API Gateway
    |
-----------------------------
| Product Service
| Cart Service
| Order Service
| Payment Service
-----------------------------
        |
Database
```

Each service has a clearly defined responsibility.

---

# Benefits

- Clear architecture
- Faster development
- Better collaboration
- Easier maintenance
- Improved scalability
- Reduced defects

---

# Common Design Principles

- Simplicity (KISS)
- Modularity
- High Cohesion
- Low Coupling
- Reusability
- Scalability
- Security by Design

---

# Common Mistakes

❌ Skipping design to save time.

✔ Good design saves much more time later.

❌ Mixing business logic with UI.

✔ Separate responsibilities.

❌ Ignoring scalability.

✔ Design for future growth.

❌ Designing without considering security.

✔ Include security from the beginning.

---

# Inputs & Outputs

| Input | Output |
|-------|--------|
| Approved SRS | HLD |
| Functional Requirements | LLD |
| NFRs | Database Design |
| Constraints | API Design |
| Business Rules | Wireframes |

---

# Interview Questions

1. What is the Design Phase?
2. Why is software design important?
3. Differentiate HLD and LLD.
4. What are the deliverables of the Design Phase?
5. Why should security be considered during design?
6. What is API design?
7. What is database design?

---

# Cheat Sheet

```text
Approved SRS
      ↓
HLD
      ↓
LLD
      ↓
Database
      ↓
API
      ↓
UI/UX
      ↓
Development

Deliverables

✓ HLD
✓ LLD
✓ UML
✓ Database Schema
✓ API Spec
✓ Wireframes
```

---

# Summary

The Design Phase bridges the gap between business requirements and implementation. It transforms the SRS into a complete technical blueprint by defining architecture, modules, databases, APIs, user interfaces, and security. A well-designed system is easier to build, test, scale, and maintain, making this phase one of the most important stages in the Software Development Life Cycle.
