# Lesson 24 — Non-Functional Requirements

# Part 2 — Software Development Life Cycle (SDLC)

> **Objective**
>
> Understand what Non-Functional Requirements (NFRs) are, why they are critical, how they differ from Functional Requirements, and how they influence the quality and success of software systems.

---

# Introduction

Imagine two food delivery applications.

Both allow users to:

- Register
- Search restaurants
- Place orders
- Make payments

Functionally, both do the same things.

But:

- One loads in **1 second**
- The other takes **15 seconds**
- One never crashes
- The other crashes during peak hours
- One protects customer data
- The other leaks passwords

Both satisfy the **functional requirements**, but only one satisfies the **non-functional requirements**.

---

# What are Non-Functional Requirements?

A **Non-Functional Requirement (NFR)** describes **how well a system should perform its functions**.

It defines the quality attributes, constraints, and performance expectations of the software.

Simply put:

```text
Functional Requirement
        ↓
What the system does

Non-Functional Requirement
        ↓
How well it does it
```

---

# Why are NFRs Important?

Ignoring NFRs can cause:

- Slow applications
- Security breaches
- Poor user experience
- Frequent downtime
- High maintenance costs

Good NFRs ensure software is ready for real-world use.

---

# Functional vs Non-Functional Requirements

| Functional Requirements | Non-Functional Requirements |
|--------------------------|-----------------------------|
| What the system does | How the system performs |
| User Login | Login within 2 seconds |
| Payment | Payment must be secure |
| Search | Search response < 1 second |
| Report Generation | Reports generated within 5 seconds |

---

# Characteristics of Good NFRs

A good NFR should be:

- Measurable
- Testable
- Specific
- Achievable
- Relevant
- Traceable

Bad:

> "The website should be fast."

Good:

> "The homepage shall load within 2 seconds for 95% of users."

---

# Types of Non-Functional Requirements

## 1. Performance

Measures system speed and resource usage.

Examples:

- Response time
- Throughput
- CPU usage
- Memory usage

```text
Request
   |
Server
   |
Response < 2 sec
```

---

## 2. Scalability

Ability to handle increasing workload.

```text
100 Users
   ↓
1,000 Users
   ↓
100,000 Users
   ↓
1 Million Users
```

---

## 3. Reliability

System performs consistently over time.

Example:

- Online banking should not crash during transactions.

---

## 4. Availability

Defines how often the system is operational.

Examples:

- 99.9%
- 99.99%
- 99.999%

Higher availability means less downtime.

---

## 5. Security

Protects:

- Data
- Privacy
- Transactions

Examples:

- Authentication
- Authorization
- Encryption
- Audit logs

---

## 6. Usability

Software should be easy to learn and use.

Example:

- Clear navigation
- Accessible interface
- Helpful error messages

---

## 7. Maintainability

Software should be easy to modify and support.

Examples:

- Easy bug fixes
- Easy feature additions
- Modular code

---

## 8. Portability

Software should work across multiple platforms.

Examples:

- Windows
- Linux
- macOS
- Cloud

---

## 9. Compatibility

Software should integrate smoothly with:

- Browsers
- APIs
- Operating systems
- External services

---

## 10. Compliance

Software must follow legal and industry regulations.

Examples:

- GDPR
- HIPAA
- PCI-DSS

---

# Industry Example

## Online Banking System

Functional Requirements:

- Login
- Transfer money
- View balance

Non-Functional Requirements:

- Login within 2 seconds
- 99.99% availability
- Multi-factor authentication
- AES-256 encrypted data
- Support 5 million users
- Complete transaction within 3 seconds

---

# Writing NFRs

Template:

```text
Requirement ID : NFR-001

Category :
Performance

Description :
The system shall respond to search requests
within 1 second for 95% of users.

Priority :
High
```

---

# Relationship with SDLC

```text
Requirement Gathering
        |
Functional Requirements
        |
Non-Functional Requirements
        |
SRS
        |
Design
        |
Development
        |
Testing
```

NFRs influence architecture, infrastructure, testing, and deployment.

---

# Common Mistakes

❌ Writing vague NFRs.

✔ Always include measurable values.

❌ Ignoring scalability.

✔ Estimate future growth.

❌ Thinking security can be added later.

✔ Consider security from the beginning.

---

# Best Practices

- Make every NFR measurable.
- Align NFRs with business goals.
- Review with stakeholders.
- Validate during testing.
- Document them in the SRS.

---

# Interview Questions

1. What are Non-Functional Requirements?
2. Differentiate Functional and Non-Functional Requirements.
3. Give examples of Performance requirements.
4. Why is scalability important?
5. Explain availability with examples.
6. Why should NFRs be measurable?

---

# Cheat Sheet

```text
Non-Functional Requirements

Answer:

"How well should the system work?"

Examples

✓ Performance
✓ Scalability
✓ Reliability
✓ Availability
✓ Security
✓ Usability
✓ Maintainability
✓ Portability
✓ Compatibility
✓ Compliance
```

---

# Summary

Non-Functional Requirements define the quality standards a software system must meet. They ensure that software is fast, secure, reliable, scalable, maintainable, and suitable for real-world environments. While Functional Requirements describe what the system should do, Non-Functional Requirements determine how effectively and efficiently it performs those functions throughout its lifecycle.
