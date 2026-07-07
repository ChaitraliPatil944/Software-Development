# Lesson 31 — SDLC Models Overview

# Part 2 — Software Development Life Cycle (SDLC)

> **Objective**
>
> Understand the major SDLC models, how they organize software development, when each model should be used, and their advantages, disadvantages, and real-world applications.

---

# Introduction

The SDLC defines **what phases** software projects follow.

An **SDLC Model** defines **how those phases are executed**.

Think of the SDLC as a destination and an SDLC model as the route you choose.

```text
Same Destination
       |
---------------------------------------
| Waterfall | Agile | Spiral | V-Model |
---------------------------------------
```

---

# What is an SDLC Model?

An SDLC model is a structured approach that defines the sequence, interaction, and execution of SDLC phases.

Different projects require different models.

---

# Why Do We Need Different Models?

Not every project has the same requirements.

Examples:

- Government payroll system
- AI startup
- Banking software
- Hospital management system

Each has different:

- Risk
- Budget
- Timeline
- Requirement stability
- Team size

---

# Popular SDLC Models

```text
SDLC Models

├── Waterfall
├── V-Model
├── Iterative
├── Incremental
├── Prototype
├── RAD
├── Spiral
└── Agile
```

Each will be covered in detail later.

---

# 1. Waterfall Model

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

### Best For

- Stable requirements
- Government projects
- Compliance-heavy systems

### Advantages

- Simple
- Well documented
- Easy to manage

### Limitations

- Difficult to accommodate changes
- Testing occurs late

---

# 2. V-Model

```text
Requirements      Acceptance Testing
      \              /
       \            /
        Design    System Testing
          \      /
      Coding
```

Every development phase has a corresponding testing phase.

Best for safety-critical systems.

---

# 3. Iterative Model

Build a simple version first, then improve it repeatedly.

```text
Version 1
    ↓
Feedback
    ↓
Version 2
    ↓
Version 3
```

Suitable when requirements evolve.

---

# 4. Incremental Model

Develop the product in small functional increments.

```text
Release 1 → Login
Release 2 → Cart
Release 3 → Payment
Release 4 → Reports
```

Users receive value early.

---

# 5. Prototype Model

Create a quick prototype to validate requirements.

```text
Idea
  |
Prototype
  |
Customer Feedback
  |
Final Product
```

Useful when requirements are unclear.

---

# 6. RAD (Rapid Application Development)

Focuses on rapid delivery using reusable components and user feedback.

Advantages:

- Fast development
- Frequent customer involvement

Best for small to medium business applications.

---

# 7. Spiral Model

Combines development with continuous risk analysis.

```text
Plan
  ↓
Risk Analysis
  ↓
Develop
  ↓
Evaluate
  ↺ Repeat
```

Best for high-risk and complex projects.

---

# 8. Agile

Software is developed in short iterations called sprints.

```text
Plan
  ↓
Sprint
  ↓
Develop
  ↓
Test
  ↓
Review
  ↓
Repeat
```

Ideal for changing requirements and frequent releases.

---

# Comparison Table

| Model | Best For | Main Strength | Main Limitation |
|-------|----------|---------------|-----------------|
| Waterfall | Stable projects | Simple | Poor flexibility |
| V-Model | Critical systems | Strong testing | Expensive changes |
| Iterative | Evolving systems | Continuous improvement | Rework |
| Incremental | Large products | Early delivery | Integration effort |
| Prototype | Unclear requirements | Better understanding | Scope creep |
| RAD | Fast delivery | Speed | Less suitable for very large systems |
| Spiral | High-risk projects | Risk management | Complex & costly |
| Agile | Dynamic projects | Flexibility | Requires active collaboration |

---

# Choosing the Right Model

Consider:

- Requirement stability
- Project size
- Budget
- Risk
- Team experience
- Customer involvement
- Regulatory needs

---

# Industry Examples

| Project | Suitable Model |
|---------|----------------|
| Banking Core System | Waterfall / V-Model |
| Hospital System | V-Model |
| Startup SaaS Product | Agile |
| AI Product | Agile / Iterative |
| Government Portal | Waterfall |
| Research Prototype | Prototype / Spiral |

---

# Common Misconceptions

❌ Agile means no planning.

✔ Agile plans continuously.

❌ Waterfall is obsolete.

✔ It is still widely used where requirements are stable.

❌ One model fits every project.

✔ Model selection depends on project characteristics.

---

# Interview Questions

1. What is an SDLC model?
2. Why are different SDLC models needed?
3. Differentiate Waterfall and Agile.
4. When is the Spiral Model preferred?
5. What is the advantage of Incremental development?
6. Which model is suitable for unclear requirements?
7. Which model emphasizes risk analysis?

---

# Cheat Sheet

```text
Waterfall   → Stable Requirements
V-Model     → Testing Focus
Iterative   → Continuous Improvement
Incremental → Feature-by-Feature
Prototype   → Clarify Requirements
RAD         → Fast Development
Spiral      → Risk Management
Agile       → Frequent Delivery
```

---

# Summary

SDLC models provide different ways of executing the Software Development Life Cycle. Each model offers unique strengths and trade-offs based on project complexity, risk, customer involvement, and requirement stability. Choosing the appropriate model helps teams deliver software more efficiently while reducing project risks. The following chapters will explore each major model in detail, beginning with the Waterfall Model.
