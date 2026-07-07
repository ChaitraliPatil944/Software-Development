# Lesson 21 — Requirement Analysis

# Part 2 — Software Development Life Cycle (SDLC)

> **Objective**
>
> Learn how gathered requirements are analyzed, validated, prioritized, and refined before software design begins.

---

# Introduction

Requirement Gathering answers:

> **What does the customer want?**

Requirement Analysis answers:

> **Can these requirements be built correctly, completely, and realistically?**

Requirement Analysis converts raw ideas into precise, implementable requirements.

---

# Why Requirement Analysis is Needed

After gathering requirements, they are often:

- Incomplete
- Ambiguous
- Conflicting
- Unrealistic
- Duplicate

Example:

Customer says:

> "The application should be fast."

Questions:

- Fast for how many users?
- Response time?
- Which operations?

Requirement Analysis removes uncertainty.

---

# Requirement Gathering vs Requirement Analysis

| Requirement Gathering | Requirement Analysis |
|------------------------|----------------------|
| Collect requirements | Examine requirements |
| Listen to stakeholders | Validate requirements |
| Record information | Remove ambiguity |
| Focus on business needs | Focus on implementation |

---

# Workflow

```text
Business Idea
      |
Requirement Gathering
      |
Requirement Analysis
      |
Approved Requirements
      |
Software Design
```

---

# Activities in Requirement Analysis

## 1. Understand Requirements

Business Analysts and stakeholders review every requirement carefully.

Questions include:

- Is it clear?
- Is it necessary?
- Is it achievable?

---

## 2. Remove Ambiguity

Bad:

> "System should load quickly."

Good:

> "Dashboard shall load within 2 seconds for 95% of users."

---

## 3. Resolve Conflicts

Example:

Marketing:

> Allow guest checkout.

Security Team:

> Every purchase requires authentication.

The team discusses trade-offs and reaches agreement.

---

## 4. Prioritize Requirements

Not every feature has equal importance.

Example:

```text
Must Have
Should Have
Could Have
Won't Have (Current Release)
```

This is commonly called **MoSCoW Prioritization**.

---

## 5. Check Feasibility

Questions:

- Is it technically possible?
- Can it fit the budget?
- Can it be completed on time?

---

## 6. Validate Requirements

Requirements should be:

- Correct
- Complete
- Consistent
- Testable
- Traceable

---

# Characteristics of a Good Requirement

A good requirement is:

✓ Clear

✓ Complete

✓ Consistent

✓ Unambiguous

✓ Feasible

✓ Testable

✓ Measurable

✓ Traceable

---

# Stakeholders Involved

```text
Customer
    |
Business Analyst
    |
Product Owner
    |
Architect
    |
Development Team
```

Sometimes QA engineers also participate to ensure requirements are testable.

---

# Industry Example

## Online Banking System

Collected Requirement:

> Users should transfer money instantly.

After Analysis:

- Maximum transfer amount?
- Daily transfer limit?
- Internet required?
- Authentication?
- Timeout?
- Audit logs?

Only after answering these questions is the requirement considered complete.

---

# Inputs & Outputs

| Input | Output |
|-------|--------|
| Raw Requirements | Refined Requirements |
| Meeting Notes | Requirement Specifications |
| User Feedback | Approved Requirement List |

---

# Requirement Analysis Process

```text
Collected Requirements
        |
Review
        |
Clarify
        |
Resolve Conflicts
        |
Prioritize
        |
Validate
        |
Approve
```

---

# Benefits

- Reduces misunderstanding
- Prevents scope creep
- Improves estimation
- Better architecture
- Easier testing
- Higher customer satisfaction

---

# Common Problems

Without Requirement Analysis:

- Developers interpret requirements differently.
- Features conflict.
- Deadlines increase.
- Budget grows.
- More bugs appear.

---

# Best Practices

- Ask "why" repeatedly.
- Convert vague statements into measurable requirements.
- Review requirements with stakeholders.
- Record assumptions.
- Obtain formal approval.

---

# Common Mistakes

❌ Accepting vague requirements.

✔ Make every requirement measurable.

❌ Ignoring conflicts.

✔ Resolve conflicts before design.

❌ Prioritizing everything as "High".

✔ Prioritize based on business value.

---

# Interview Questions

1. What is Requirement Analysis?
2. How is it different from Requirement Gathering?
3. What makes a good requirement?
4. Explain MoSCoW prioritization.
5. Why should requirements be testable?
6. What happens if ambiguous requirements are ignored?

---

# Cheat Sheet

```text
Requirement Analysis

Gathered Requirements
        ↓
Review
        ↓
Clarify
        ↓
Resolve Conflicts
        ↓
Prioritize
        ↓
Validate
        ↓
Approve

Goal:
Clear + Complete + Testable + Feasible
```

---

# Summary

Requirement Analysis transforms collected stakeholder needs into clear, validated, and implementable requirements. By removing ambiguity, resolving conflicts, checking feasibility, and prioritizing features, this phase provides a strong foundation for design, development, testing, and successful project delivery.
