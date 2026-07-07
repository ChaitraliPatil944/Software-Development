# Lesson 36 — V-Model (Verification and Validation Model)

# Part 3 — Traditional SDLC Models

> **Objective**
>
> Understand the V-Model, why it was introduced, how verification and validation work together, its workflow, advantages, limitations, and where it is used in industry.

---

# Introduction

The **V-Model** is an extension of the Waterfall Model.

Instead of keeping testing until the end, the V-Model plans testing alongside every development activity.

```text
Development        Testing

Requirements   ↔  Acceptance Testing
System Design  ↔  System Testing
Architecture   ↔  Integration Testing
Module Design  ↔  Unit Testing
         \      /
          Coding
```

The shape resembles the letter **V**, hence the name.

---

# Why Was the V-Model Created?

Waterfall had one major weakness:

- Testing happened only after development.

If design mistakes were discovered late, fixing them became expensive.

The V-Model introduced **early test planning**.

---

# What is Verification?

Verification asks:

> **"Are we building the product correctly?"**

It checks documents and designs before coding.

Activities:

- Requirement Reviews
- Design Reviews
- Walkthroughs
- Inspections

No software execution is required.

---

# What is Validation?

Validation asks:

> **"Are we building the right product?"**

It involves executing the software.

Activities:

- Unit Testing
- Integration Testing
- System Testing
- Acceptance Testing

---

# Complete V-Model Workflow

```text
Verification                     Validation

Business Requirements
        |                    Acceptance Testing
        |
System Requirements
        |                    System Testing
        |
High-Level Design
        |                    Integration Testing
        |
Low-Level Design
        |                    Unit Testing
         \                  /
              Coding
```

Every development phase has a matching testing phase.

---

# Development Phase Mapping

| Verification Phase | Validation Phase |
|--------------------|------------------|
| Business Requirements | Acceptance Testing |
| System Requirements | System Testing |
| High-Level Design | Integration Testing |
| Low-Level Design | Unit Testing |

---

# Activities

## Requirements

- Gather requirements
- Review requirements
- Prepare acceptance test plan

---

## System Design

- Overall architecture
- Plan system tests

---

## High-Level Design

- Module interactions
- Plan integration tests

---

## Low-Level Design

- Classes
- Functions
- Algorithms
- Prepare unit tests

---

## Coding

Implementation begins only after planning.

---

## Testing

Testing follows the planned validation strategy.

---

# Industry Example

## Medical Device Software

Requirements:

- Accurate patient readings
- Alarm system
- Regulatory compliance

Verification:

- Review requirements
- Review architecture

Validation:

- Unit testing
- Integration testing
- System testing
- Acceptance testing

Because patient safety is critical, defects must be prevented as early as possible.

---

# Advantages

- Early defect detection
- Better quality
- Strong documentation
- Easier traceability
- Clear milestones
- Testing planned from the beginning

---

# Limitations

- Difficult to accommodate changing requirements
- Documentation intensive
- Less suitable for Agile environments
- Higher planning effort

---

# Best Use Cases

Ideal for:

- Healthcare systems
- Banking
- Aerospace
- Automotive
- Defense
- Embedded systems

Where failures can have serious consequences.

---

# V-Model vs Waterfall

| Waterfall | V-Model |
|-----------|----------|
| Testing after development | Testing planned alongside development |
| Lower test planning | Strong test planning |
| Simpler | Higher quality focus |

---

# Stakeholders

```text
Customer
    |
Business Analyst
    |
Architect
    |
Developers
    |
QA Engineers
    |
Project Manager
```

QA participates much earlier than in Waterfall.

---

# Deliverables

- Reviewed Requirements
- Design Documents
- Test Plans
- Source Code
- Test Reports
- Release Recommendation

---

# Common Mistakes

❌ Writing test cases after coding.

✔ Prepare tests during design.

❌ Skipping requirement reviews.

✔ Detect defects before implementation.

❌ Using V-Model for rapidly changing products.

✔ Prefer stable requirements.

---

# Interview Questions

1. What is the V-Model?
2. Why was the V-Model introduced?
3. Explain verification and validation.
4. Which testing level corresponds to High-Level Design?
5. How is the V-Model different from Waterfall?
6. Where is the V-Model commonly used?

---

# Cheat Sheet

```text
Requirements      ↔ Acceptance Testing
System Design     ↔ System Testing
High-Level Design ↔ Integration Testing
Low-Level Design  ↔ Unit Testing
          \      /
             Coding

Best For

✓ Safety-Critical Systems
✓ Stable Requirements
✓ Strong Quality Assurance
```

---

# Summary

The V-Model extends the Waterfall approach by integrating verification and validation throughout the software lifecycle. Every development activity has a corresponding testing activity, enabling earlier defect detection, stronger traceability, and higher software quality. It is especially effective for projects with stable requirements where reliability and compliance are essential.
