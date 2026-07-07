# Lesson 37 — Incremental Model

# Part 3 — Traditional SDLC Models

> **Objective**
>
> Understand the Incremental Model, how software is delivered in multiple releases, when it should be used, its workflow, advantages, limitations, and industry applications.

---

# Introduction

Imagine building an e-commerce application.

Instead of waiting one year to release everything, the team delivers:

```text
Release 1 → User Login
Release 2 → Product Catalog
Release 3 → Shopping Cart
Release 4 → Payments
Release 5 → Order Tracking
```

Each release adds new functionality.

This approach is called the **Incremental Model**.

---

# What is the Incremental Model?

The Incremental Model divides a software project into multiple smaller parts called **increments**.

Each increment goes through its own mini-SDLC:

```text
Requirements
     ↓
Design
     ↓
Development
     ↓
Testing
     ↓
Deployment
```

At the end of every increment, users receive a working version.

---

# Why Was the Incremental Model Introduced?

Traditional models delayed software delivery until the end.

Organizations wanted to:

- Deliver value earlier
- Gather user feedback sooner
- Reduce project risk
- Handle large projects more effectively

---

# Complete Workflow

```text
Overall Requirements
        |
-------------------------------
| Increment 1
|  SDLC
-------------------------------
        |
Working Software v1
        |
-------------------------------
| Increment 2
|  SDLC
-------------------------------
        |
Working Software v2
        |
-------------------------------
| Increment 3
|  SDLC
-------------------------------
        |
Final Product
```

---

# Characteristics

- Feature-by-feature delivery
- Multiple releases
- Continuous integration
- Early customer feedback
- Progressive improvement

---

# Industry Example

## Food Delivery Platform

### Increment 1

- Registration
- Login

### Increment 2

- Browse Restaurants
- Search Food

### Increment 3

- Cart
- Checkout

### Increment 4

- Online Payments

### Increment 5

- Live Order Tracking

Users can already use the application after the first release.

---

# Activities in Each Increment

1. Requirement selection
2. Design
3. Development
4. Testing
5. Deployment
6. Customer feedback

Then the cycle repeats.

---

# Advantages

- Early working software
- Lower project risk
- Easier testing
- Faster customer feedback
- Better resource utilization
- Easier project management

---

# Limitations

- Requires good planning
- Integration becomes more complex
- Architecture must support growth
- Scope changes must be controlled

---

# Best Use Cases

Ideal for:

- Web applications
- Mobile applications
- SaaS products
- Enterprise software
- E-commerce platforms

---

# Incremental vs Waterfall

| Waterfall | Incremental |
|-----------|-------------|
| One final release | Multiple releases |
| Feedback comes late | Feedback after each increment |
| Entire system built together | Features built gradually |

---

# Stakeholders

```text
Customer
    |
Product Owner
    |
Business Analyst
    |
Developers
    |
QA
    |
DevOps
```

Customers review every release.

---

# Deliverables

Each increment produces:

- Working Software
- Source Code
- Test Reports
- Release Notes
- Customer Feedback

---

# Common Mistakes

❌ Ignoring architecture.

✔ Design for future increments.

❌ Delivering unrelated features.

✔ Prioritize business value.

❌ Poor integration planning.

✔ Integrate continuously.

---

# Interview Questions

1. What is the Incremental Model?
2. Why is it better than a single large release?
3. How does it differ from Waterfall?
4. What are its advantages?
5. Where is it commonly used?
6. What challenges exist with multiple increments?

---

# Cheat Sheet

```text
Overall Requirements
        ↓
Increment 1
        ↓
Release
        ↓
Increment 2
        ↓
Release
        ↓
Increment 3
        ↓
Final Product

Best For

✓ Large Applications
✓ Early Delivery
✓ Continuous Feedback
```

---

# Summary

The Incremental Model develops software in multiple planned releases instead of delivering everything at once. Each increment follows the complete SDLC and adds valuable functionality to the product. This model enables earlier delivery, faster feedback, lower risk, and continuous improvement, making it a popular choice for modern business applications.
