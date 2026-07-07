# Lesson 20 — Requirement Gathering

# Part 2 — Software Development Life Cycle (SDLC)

> **Objective**
>
> Learn how software teams discover **what should be built**, who participates, which techniques are used, what documents are produced, and why Requirement Gathering is considered the most critical phase of the SDLC.

---

# Introduction

Imagine a customer says:

> "Build me an online shopping website."

Is that enough?

No.

Questions immediately arise:

- Who are the users?
- What products will be sold?
- Should it support online payments?
- Mobile app or website?
- Which countries?
- How many users?
- What security is required?

Before writing a single line of code, engineers must understand the problem completely.

This process is called **Requirement Gathering** (also called **Requirement Elicitation**).

---

# What is Requirement Gathering?

Requirement Gathering is the process of identifying, collecting, understanding, and documenting the needs and expectations of stakeholders.

Its goal is to answer:

```text
What should we build?
Why should we build it?
Who will use it?
```

---

# Why is Requirement Gathering Important?

A famous software engineering principle says:

> **A defect in requirements is the most expensive defect to fix later.**

```text
Wrong Requirement
        |
Design
        |
Development
        |
Testing
        |
Production

Fix Cost ↑↑↑
```

Finding mistakes early saves time, money, and effort.

---

# Real-Life Analogy

Imagine ordering a custom house.

If you only say:

> "Build me a house."

The architect has no idea about:

- Number of rooms
- Budget
- Parking
- Garden
- Floors
- Style

Software projects are no different.

---

# Stakeholders Involved

```text
Customer
     |
Business Analyst
     |
Product Owner
     |
Project Manager
     |
Architect
```

Sometimes developers, designers, and QA engineers also participate.

---

# Requirement Gathering Workflow

```text
Business Idea
      |
Identify Stakeholders
      |
Collect Requirements
      |
Clarify Requirements
      |
Document Requirements
      |
Review
      |
Customer Approval
```

Only after approval does the project move to Requirement Analysis.

---

# Types of Requirements Collected

## Business Requirements

High-level business goals.

Example:

- Increase online sales
- Reduce customer support calls

---

## User Requirements

What users expect.

Example:

- User can register.
- User can track orders.

---

## System Requirements

Technical capabilities.

Example:

- Database support
- Cloud deployment
- API integration

---

# Requirement Gathering Techniques

## 1. Interviews

One-to-one discussions with stakeholders.

Advantages:
- Detailed information
- Clarification possible

Best for:
- Small to medium projects

---

## 2. Questionnaires

Useful when many stakeholders are involved.

Advantages:
- Fast
- Cost-effective

Limitation:
- Less detailed responses

---

## 3. Workshops

Multiple stakeholders discuss requirements together.

Benefits:
- Faster decision-making
- Shared understanding

---

## 4. Brainstorming

Team generates ideas freely.

Useful for:
- New products
- Innovative solutions

---

## 5. Observation

Business Analyst observes current work.

Example:

Watching hospital staff register patients before designing a Hospital Management System.

---

## 6. Document Analysis

Study existing:

- Reports
- Forms
- Manuals
- Existing software

Useful when replacing legacy systems.

---

## 7. Prototyping

Create a simple model before development.

```text
Idea
  |
Prototype
  |
Customer Feedback
  |
Improved Requirements
```

Helps users visualize the final product.

---

# Industry Example

## Food Delivery Platform

Business Goal:

Allow customers to order food online.

Requirements gathered:

Customer:
- Browse restaurants
- Place order
- Online payment
- Live tracking

Restaurant:
- Accept orders
- Update menu
- View earnings

Delivery Partner:
- Accept deliveries
- Navigate to customer
- Update delivery status

Notice how different stakeholders have different requirements.

---

# Deliverables

Common outputs include:

- Meeting Notes
- Requirement List
- User Stories
- Use Cases
- BRD (Business Requirement Document)
- Initial Scope Document

These become inputs for Requirement Analysis.

---

# Common Problems

Poor Requirement Gathering causes:

- Wrong features
- Budget overruns
- Scope creep
- Frequent changes
- Customer dissatisfaction
- Project delays

---

# Best Practices

- Ask open-ended questions.
- Listen carefully.
- Confirm assumptions.
- Document everything.
- Review with stakeholders.
- Obtain formal approval.

---

# Common Mistakes

❌ Assuming requirements.

✔ Validate every requirement.

❌ Ignoring end users.

✔ Include real users whenever possible.

❌ Starting development immediately.

✔ Complete requirement gathering first.

---

# Interview Questions

1. What is Requirement Gathering?
2. Why is it important?
3. Name different requirement gathering techniques.
4. Differentiate Business, User, and System Requirements.
5. Why is prototyping useful?
6. Who participates in Requirement Gathering?

---

# Cheat Sheet

```text
Requirement Gathering

Identify Stakeholders
        ↓
Collect Information
        ↓
Clarify
        ↓
Document
        ↓
Review
        ↓
Approve

Techniques

✓ Interviews
✓ Questionnaires
✓ Workshops
✓ Brainstorming
✓ Observation
✓ Document Analysis
✓ Prototyping
```

---

# Summary

Requirement Gathering is the foundation of every successful software project. It transforms business ideas into clear, documented requirements by involving stakeholders, asking the right questions, and using structured elicitation techniques. Well-gathered requirements reduce project risk, improve communication, and ensure the development team builds the right product from the very beginning.
