# Lesson 39 — Spiral Model

# Part 3 — Traditional SDLC Models

> **Objective**
>
> Understand the Spiral Model, its risk-driven approach, lifecycle, advantages, limitations, and where it is used in real-world software engineering.

---

# Introduction

Not every software project has stable requirements or low risk.

Examples:

- Banking platforms
- Space missions
- Defense systems
- Enterprise ERP
- AI platforms

These projects involve uncertainty, changing requirements, and significant financial risk.

The **Spiral Model** was designed to manage these risks throughout development.

---

# What is the Spiral Model?

The **Spiral Model** is an SDLC model that combines:

- Iterative development
- Risk analysis
- Prototyping
- Customer feedback

Development progresses through repeated cycles called **spirals**.

Each spiral produces a more complete version of the software.

---

# Why Was the Spiral Model Introduced?

Traditional models assumed risks could be handled with planning alone.

Large projects proved otherwise.

The Spiral Model introduces **risk assessment before major development activities**.

---

# Core Concept

```text
Plan
  ↓
Risk Analysis
  ↓
Engineering
  ↓
Customer Evaluation
  ↓
Repeat
```

Every cycle reduces uncertainty.

---

# Spiral Workflow

```text
           +----------------------+
           | Customer Evaluation  |
           +----------▲-----------+
                      |
+-----------+         |
| Planning  |---------+
+-----+-----+
      |
      v
+-----+-----+
| Risk      |
| Analysis  |
+-----+-----+
      |
      v
+-----+-----+
| Engineering|
| Design +   |
| Development|
+-----------+
      |
      +---------------------> Next Spiral
```

---

# Four Quadrants of Every Spiral

## 1. Planning

Activities:

- Define objectives
- Identify requirements
- Estimate resources

---

## 2. Risk Analysis

Identify:

- Technical risks
- Cost risks
- Schedule risks
- Security risks
- Business risks

Possible solutions are evaluated before coding.

---

## 3. Engineering

Activities:

- Design
- Development
- Testing
- Prototype refinement

---

## 4. Customer Evaluation

Customer reviews progress.

Feedback becomes input for the next spiral.

---

# Industry Example

## Online Banking Platform

### Spiral 1

- Login
- Authentication prototype
- Security risk assessment

### Spiral 2

- Account management
- Performance testing
- Compliance review

### Spiral 3

- Money transfer
- Fraud detection
- Customer feedback

The product grows while risks are continuously managed.

---

# Types of Risks

```text
Technical
Business
Schedule
Cost
Security
Operational
```

The Spiral Model addresses these throughout development.

---

# Advantages

- Excellent risk management
- Supports changing requirements
- Continuous customer feedback
- High-quality software
- Suitable for large projects
- Early prototypes

---

# Limitations

- Expensive
- Complex to manage
- Requires experienced teams
- Heavy documentation
- Not suitable for small projects

---

# Best Use Cases

Ideal for:

- Aerospace
- Defense
- Banking
- Healthcare
- Enterprise software
- AI & ML platforms

---

# Spiral vs Iterative

| Spiral | Iterative |
|--------|-----------|
| Risk-driven | Improvement-driven |
| Formal risk analysis | Minimal risk focus |
| Better for high-risk projects | Better for evolving products |

---

# Spiral vs Waterfall

| Waterfall | Spiral |
|-----------|---------|
| Sequential | Cyclic |
| Fixed planning | Continuous planning |
| Limited risk handling | Risk is central |

---

# Stakeholders

```text
Customer
    |
Business Analyst
    |
Project Manager
    |
Architect
    |
Developers
    |
QA
    |
Risk Management Team
```

---

# Deliverables

Each spiral produces:

- Risk Assessment Report
- Prototype / Working Software
- Updated Requirements
- Test Results
- Customer Feedback

---

# Common Mistakes

❌ Ignoring formal risk analysis.

✔ Evaluate risks in every cycle.

❌ Using Spiral for small, simple projects.

✔ Reserve it for complex, high-risk systems.

❌ Skipping customer evaluation.

✔ Validate every spiral before moving forward.

---

# Interview Questions

1. What is the Spiral Model?
2. Why was it introduced?
3. What are the four quadrants of the Spiral Model?
4. Why is it considered risk-driven?
5. Differentiate Spiral and Iterative Models.
6. Where is the Spiral Model commonly used?

---

# Cheat Sheet

```text
Planning
    ↓
Risk Analysis
    ↓
Engineering
    ↓
Customer Evaluation
    ↓
Repeat

Best For

✓ High Risk
✓ Large Projects
✓ Changing Requirements

Weakness

✗ Complex
✗ Expensive
```

---

# Summary

The Spiral Model is a risk-driven SDLC model that combines iterative development with continuous planning, engineering, customer evaluation, and formal risk analysis. By identifying and mitigating risks early in every development cycle, it is especially effective for large, complex, and mission-critical software projects where uncertainty and change are expected.
