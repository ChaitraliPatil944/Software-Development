# Lesson 54 — Agile Team Structure

# Part 4 — Agile Software Development

> **Objective**
>
> Understand the structure of an Agile team, the responsibilities of every role, how cross-functional teams collaborate, and how work flows inside modern software companies.

---

# Introduction

Agile is built around **people**, not departments.

Instead of teams working one after another, Agile encourages everyone to collaborate continuously.

```text
Business
    │
Product Owner
    │
────────────────────────────────
 Scrum Master
 Developers
 QA Engineers
 UI/UX Designers
 DevOps
 Business Analyst
────────────────────────────────
    │
Working Software
```

---

# What is an Agile Team?

An **Agile Team** is a small, cross-functional, self-organizing group responsible for delivering working software during every sprint.

Characteristics:

- Cross-functional
- Self-organizing
- Collaborative
- Customer-focused
- Continuous improvement

---

# Team Structure

```text
                 Stakeholders
                      │
               Product Owner
                      │
              Scrum Master
                      │
 ┌────────────────────────────────────┐
 │ Developers │ QA │ UI/UX │ DevOps │
 │ Business Analyst │ Security │      │
 └────────────────────────────────────┘
                      │
              Working Product
```

---

# Product Owner (PO)

## Purpose

Represents the customer and maximizes business value.

### Responsibilities

- Define product vision
- Maintain Product Backlog
- Prioritize features
- Accept completed work
- Clarify business requirements

### Industry Example

For an e-commerce application, the Product Owner decides:

- Should Wishlist be built before Coupons?
- Which feature delivers the highest business value?

---

# Scrum Master

## Purpose

Helps the team follow Agile practices.

The Scrum Master is **not** the team's manager.

### Responsibilities

- Facilitate Scrum ceremonies
- Remove blockers
- Coach Agile practices
- Protect the team from distractions
- Improve team productivity

Example:

If developers cannot access a testing server, the Scrum Master coordinates with infrastructure teams to resolve the issue.

---

# Developers

Developers create the software.

Responsibilities:

- Design
- Coding
- Unit Testing
- Code Reviews
- Bug Fixes
- Collaboration

Modern Agile developers are expected to understand the complete feature rather than only isolated tasks.

---

# QA Engineers

QA ensures software quality.

Activities:

- Test Planning
- Functional Testing
- Regression Testing
- Automation
- Defect Reporting

QA works throughout the sprint instead of only after development.

---

# UI/UX Designers

Responsibilities:

- User Research
- Wireframes
- Mockups
- Prototypes
- Design Systems

Goal:

Create intuitive user experiences.

---

# DevOps Engineer

Responsibilities:

- CI/CD Pipelines
- Infrastructure
- Cloud Deployment
- Monitoring
- Automation
- Release Management

Later handbook sections will explore DevOps in depth.

---

# Business Analyst (BA)

Responsibilities:

- Gather requirements
- Analyze business processes
- Write User Stories
- Clarify requirements
- Support Product Owner

---

# Security Engineer (Optional)

In many organizations:

- Threat Modeling
- Secure Code Reviews
- Vulnerability Assessment
- Compliance

---

# Stakeholders

Stakeholders include:

- Customers
- Sponsors
- Business Leaders
- End Users
- Regulatory Teams

They provide feedback during Sprint Reviews.

---

# Cross-Functional Teams

Traditional:

```text
Business
   ↓
Developers
   ↓
QA
   ↓
Operations
```

Agile:

```text
Business
    ↕
Product Owner
    ↕
Developers ↔ QA ↔ DevOps ↔ UX
```

Everyone collaborates throughout the sprint.

---

# Self-Organizing Teams

Managers define goals.

Teams decide:

- Task distribution
- Technical implementation
- Daily collaboration

This increases ownership and accountability.

---

# Communication Flow

```text
Customer
    │
Product Owner
    │
Scrum Master
    │
Developers ↔ QA ↔ DevOps ↔ UX
    │
Working Software
```

---

# Industry Example

## Food Delivery Platform

Product Owner:

- Prioritizes "Live Order Tracking"

Developers:

- Build APIs and UI

QA:

- Tests order tracking

DevOps:

- Deploys new release

Customers review the feature during the Sprint Review.

---

# Advantages of Agile Teams

- Faster decisions
- Better communication
- Higher quality
- Reduced handoff delays
- Continuous collaboration
- Shared ownership

---

# Common Misconceptions

❌ Scrum Master manages developers.

✔ Scrum Master coaches and facilitates.

❌ QA only tests after coding.

✔ QA participates throughout the sprint.

❌ Developers work alone.

✔ Agile development is collaborative.

---

# Interview Questions

1. What is an Agile team?
2. What is the role of the Product Owner?
3. What does a Scrum Master do?
4. How are Agile teams different from traditional teams?
5. What is a cross-functional team?
6. What is a self-organizing team?
7. Why is QA involved throughout the sprint?

---

# Cheat Sheet

```text
Product Owner
   │
Business Value

Scrum Master
   │
Agile Process

Developers
   │
Software

QA
   │
Quality

DevOps
   │
Deployment

UI/UX
   │
User Experience

Business Analyst
   │
Requirements
```

---

# Summary

An Agile team is a cross-functional, self-organizing group that collaborates throughout every sprint to deliver valuable software. Each role contributes specialized expertise while sharing responsibility for the product's success. Strong communication, continuous feedback, and collective ownership are the foundations of effective Agile teams.
