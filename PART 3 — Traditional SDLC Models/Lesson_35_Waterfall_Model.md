# Lesson 35 — Waterfall Model

# Part 3 — Traditional SDLC Models

> **Objective**
>
> Understand the Waterfall Model in depth, including its history, workflow, phases, documentation, advantages, limitations, industry use cases, and interview concepts.

---

# Introduction

The **Waterfall Model** is the oldest and one of the most influential SDLC models.

It follows a **linear, sequential** approach where each phase must be completed before the next phase begins.

Like a waterfall, work flows in one direction.

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
      ↓
Maintenance
```

There is little or no movement back to previous phases.

---

# Why Was the Waterfall Model Created?

During the early years of software engineering, projects lacked structure.

Problems included:

- No planning
- Constant requirement changes
- Poor documentation
- Missed deadlines
- Cost overruns

The Waterfall Model introduced a disciplined process.

---

# History

- Popularized during the 1970s.
- Strongly associated with engineer **entity["people","Winston W. Royce","Software engineering pioneer"]**.
- Widely adopted for government, defense, banking, and aerospace projects where documentation and approvals are essential.

> Interestingly, Royce himself discussed limitations of a strictly sequential approach, but the model became famous anyway. Humans have a remarkable talent for simplifying nuanced advice into a flowchart. 📄

---

# Core Idea

Finish one phase completely before starting the next.

```text
Phase 1 ✔
     ↓
Phase 2 ✔
     ↓
Phase 3 ✔
     ↓
Phase 4 ✔
```

No overlapping work.

---

# Complete Workflow

```text
Business Need
      |
Requirements
      |
Design
      |
Implementation
      |
Testing
      |
Deployment
      |
Maintenance
```

---

# Waterfall Phases

## 1. Requirements

Activities:

- Requirement Gathering
- Requirement Analysis
- SRS Preparation

Output:

- Approved SRS

---

## 2. Design

Activities:

- HLD
- LLD
- Database Design
- API Design
- UI Design

Output:

- Design Documents

---

## 3. Development

Activities:

- Coding
- Unit Testing
- Build Generation

Output:

- Source Code

---

## 4. Testing

Activities:

- Functional Testing
- Integration Testing
- System Testing
- Bug Fix Verification

Output:

- Tested Software

---

## 5. Deployment

Activities:

- Production Release
- Smoke Testing
- Release Documentation

Output:

- Live Application

---

## 6. Maintenance

Activities:

- Bug Fixes
- Security Updates
- Feature Enhancements

Output:

- Updated Versions

---

# Documentation Flow

```text
BRD
  ↓
SRS
  ↓
HLD / LLD
  ↓
Source Code
  ↓
Test Reports
  ↓
Release Notes
```

Documentation is a major strength of the Waterfall Model.

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
Operations
```

---

# Advantages

- Simple and easy to understand
- Clear milestones
- Strong documentation
- Easy project tracking
- Well suited for fixed-scope projects
- Easier cost estimation

---

# Limitations

- Difficult to handle changing requirements
- Customer feedback arrives late
- Testing happens after development
- Higher cost of late changes
- Longer time before users see working software

---

# Best Use Cases

Ideal for:

- Government systems
- Banking core systems
- Defense projects
- Healthcare compliance systems
- Embedded systems with fixed requirements

Avoid when:

- Requirements change frequently
- Rapid releases are required
- Continuous customer feedback is expected

---

# Industry Example

## Government Tax Filing System

Requirements are defined by law.

Workflow:

```text
Legal Requirements
        ↓
SRS
        ↓
Design
        ↓
Development
        ↓
Testing
        ↓
Production
```

Frequent requirement changes are uncommon, making Waterfall suitable.

---

# Waterfall vs Agile (Quick Preview)

| Waterfall | Agile |
|-----------|--------|
| Sequential | Iterative |
| Fixed requirements | Changing requirements |
| Heavy documentation | Lightweight documentation |
| Late customer feedback | Continuous customer feedback |

A detailed comparison comes later in the handbook.

---

# Common Mistakes

❌ Starting coding before requirements are approved.

✔ Complete requirements first.

❌ Skipping documentation.

✔ Maintain complete documentation.

❌ Choosing Waterfall for rapidly changing projects.

✔ Select the SDLC model based on project characteristics.

---

# Interview Questions

1. What is the Waterfall Model?
2. Why is it called the Waterfall Model?
3. List the phases of the Waterfall Model.
4. What are the advantages of Waterfall?
5. What are its limitations?
6. When should Waterfall be used?
7. Why is documentation important in Waterfall?

---

# Cheat Sheet

```text
Waterfall

Requirements
      ↓
Design
      ↓
Development
      ↓
Testing
      ↓
Deployment
      ↓
Maintenance

Best For

✓ Stable Requirements
✓ Strong Documentation
✓ Compliance Projects

Weakness

✗ Poor flexibility
✗ Late feedback
```

---

# Summary

The Waterfall Model is a sequential SDLC model where each phase is completed before the next begins. Its emphasis on planning, documentation, and controlled execution makes it suitable for projects with stable requirements and strict regulatory needs. Although less flexible than modern iterative approaches, it remains widely used in industries where predictability and documentation are more important than rapid change.
