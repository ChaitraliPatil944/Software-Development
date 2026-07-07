# Lesson 43 — Component-Based Model

# Part 3 — Traditional SDLC Models

> **Objective**
>
> Understand the Component-Based Development (CBD) Model, how reusable software components reduce development time and cost, and where this model is used in modern software engineering.

---

# Introduction

Imagine building a computer.

Do manufacturers create every chip, RAM module, and SSD from scratch?

No.

They assemble reliable, pre-built components.

Modern software follows the same idea.

Instead of developing every feature from scratch, teams reuse existing components wherever possible.

---

# What is the Component-Based Model?

The **Component-Based Development (CBD) Model** is an SDLC model where software is built by integrating reusable, independent software components.

```text
Existing Components
        |
Selection
        |
Integration
        |
Testing
        |
Final Software
```

---

# Why Was CBD Introduced?

Large software projects repeatedly implemented the same features:

- Authentication
- Payment gateways
- Logging
- Email
- Reporting

Reusing proven components saves time and improves reliability.

---

# Core Principles

- Reusability
- Modularity
- Loose Coupling
- High Cohesion
- Standard Interfaces

---

# CBD Workflow

```text
Requirements
      |
Identify Components
      |
Select / Build Components
      |
Integrate
      |
Test
      |
Deploy
```

---

# Major Activities

## 1. Requirement Analysis

Determine which features are needed.

---

## 2. Component Identification

Identify components that can be reused.

Examples:

- Login module
- Notification service
- PDF generator

---

## 3. Component Evaluation

Check:

- Compatibility
- Performance
- Security
- Licensing
- Maintainability

---

## 4. Component Adaptation

Configure or customize components if needed.

---

## 5. Integration

Combine components into one application.

```text
UI
 |
API
 |
-----------------------
| Login Component
| Payment Component
| Reporting Component
-----------------------
 |
Database
```

---

## 6. Testing

Verify:

- Individual components
- Component interaction
- Entire system

---

# Types of Components

- UI Components
- Business Logic Components
- Database Components
- API Components
- Third-Party Libraries
- Cloud Services

---

# Industry Example

## E-Commerce Platform

Instead of building everything:

- Authentication → Existing Identity Provider
- Payments → Payment Gateway
- Email → Email Service
- Search → Search Engine
- File Storage → Cloud Storage

Developers focus on business-specific logic.

---

# Advantages

- Faster development
- Lower cost
- Better reliability
- Reduced maintenance
- Easier scalability
- Proven functionality

---

# Limitations

- Integration complexity
- Dependency on third-party vendors
- Licensing issues
- Compatibility problems
- Less control over external components

---

# Best Use Cases

Suitable for:

- Enterprise applications
- Web platforms
- SaaS products
- Cloud-native systems
- Microservices

---

# CBD vs Waterfall

| Waterfall | CBD |
|-----------|-----|
| Build everything | Reuse components |
| Longer development | Faster development |
| More custom code | Less custom code |

---

# CBD vs RAD

| CBD | RAD |
|-----|-----|
| Focus on reuse | Focus on speed |
| Reusable architecture | Rapid prototyping |

---

# Stakeholders

```text
Business Analyst
      |
Architect
      |
Developers
      |
QA
      |
DevOps
```

---

# Deliverables

- Component Catalog
- Integration Design
- Source Code
- Test Reports
- Deployment Package

---

# Best Practices

- Reuse trusted components
- Review licenses
- Validate security
- Maintain interface documentation
- Keep components loosely coupled

---

# Common Mistakes

❌ Reusing outdated libraries.

✔ Keep dependencies updated.

❌ Ignoring compatibility.

✔ Test integrations thoroughly.

❌ Selecting components based only on popularity.

✔ Evaluate quality, support, and security.

---

# Interview Questions

1. What is the Component-Based Model?
2. Why is software component reuse important?
3. What are the advantages of CBD?
4. What challenges exist when integrating components?
5. Give examples of reusable software components.
6. Where is CBD commonly used?

---

# Cheat Sheet

```text
Requirements
      ↓
Identify Components
      ↓
Evaluate
      ↓
Integrate
      ↓
Test
      ↓
Deploy

Best For

✓ Enterprise Apps
✓ Cloud Systems
✓ Reusable Architecture

Weakness

✗ Integration Complexity
✗ Third-Party Dependencies
```

---

# Summary

The Component-Based Development Model builds software by assembling reusable, well-tested components instead of creating every feature from scratch. This approach reduces development time, lowers costs, improves reliability, and allows teams to focus on unique business functionality while relying on proven reusable modules for common capabilities.
