# Lesson 100 — Non Functional Requirements

# Part 7 — Requirements Engineering

> **Objective**
>
> Understand Non Functional Requirements, why they are important, different quality attributes, examples, documentation, and how they influence software architecture and system quality.

---

# Introduction

Functional Requirements define:

**What the system does**

But software quality depends on:

- How fast it works
- How secure it is
- How reliable it is
- How easily it can be maintained

These qualities are defined by **Non Functional Requirements**.

```text
Functional Requirements

        ↓

System Features


Non Functional Requirements

        ↓

System Quality
```

---

# What are Non Functional Requirements?

**Non Functional Requirements (NFRs)** describe the quality attributes, constraints, and performance expectations of a software system.

They define:

**How the system should behave**

---

# Examples

## Banking Application

Functional:

"User can transfer money."

Non Functional:

- Transaction should complete within 2 seconds
- Data should be encrypted
- System should be available 99.9% of the time

---

## E-Commerce Application

Functional:

"User can search products."

Non Functional:

- Search results should appear quickly
- System should support millions of users
- User data should be protected

---

# Why Do We Need Non Functional Requirements?

Without NFRs:

```text
Features Work

      ↓

Poor User Experience

      ↓

Performance Problems

      ↓

System Failure
```

NFRs help:

- Improve user experience
- Define system quality
- Guide architecture decisions
- Reduce technical risks
- Ensure reliability

---

# Types of Non Functional Requirements

```text
Non Functional Requirements

        |
        |
-------------------------------
|       |       |       |
Performance Security Reliability Scalability
```

---

# 1. Performance Requirements

Define how fast the system responds.

Examples:

- Response time
- Processing speed
- Throughput

Example:

"System should display search results within 2 seconds."

---

# Performance Metrics

## Response Time

Time taken to complete a request.

Example:

API response:

< 500 milliseconds

---

## Throughput

Number of operations processed in a given time.

Example:

"System should handle 10,000 transactions per minute."

---

# 2. Security Requirements

Define protection against threats.

Examples:

- Authentication
- Authorization
- Encryption
- Data protection

Example:

"Passwords must be stored using encryption."

---

# 3. Scalability Requirements

Define the ability to handle growth.

Example:

A shopping website should support:

```text
10,000 Users

        ↓

1 Million Users
```

without major redesign.

---

# 4. Reliability Requirements

Define whether the system works consistently.

Examples:

- Error handling
- Fault tolerance
- Data recovery

Example:

"System should recover automatically after failure."

---

# 5. Availability Requirements

Define how often the system is accessible.

Example:

"Application should have 99.9% uptime."

---

# 6. Maintainability Requirements

Define how easily software can be modified.

Examples:

- Clean code
- Documentation
- Modular architecture

---

# 7. Usability Requirements

Define ease of use.

Examples:

- Simple interface
- Easy navigation
- Accessibility support

---

# 8. Portability Requirements

Define ability to run in different environments.

Example:

Application should support:

- Windows
- Linux
- Cloud environments

---

# Non Functional Requirement Structure

A good NFR contains:

```text
Requirement ID

Quality Attribute

Description

Measurement Criteria

Priority
```

---

# Example

## Requirement ID

NFR-001

## Type

Performance

## Description

The system should respond quickly.

## Measurement

Response time should be less than 2 seconds.

---

# Non Functional Requirements in SDLC

```text
Requirements

      ↓

Architecture Design

      ↓

Development

      ↓

Testing

      ↓

Deployment
```

NFRs strongly influence architecture decisions.

---

# Impact on Software Design

Example:

Requirement:

"System should support millions of users."

Possible design decisions:

- Load balancing
- Cloud infrastructure
- Database optimization
- Caching

---

# Functional vs Non Functional Requirements

| Functional Requirements | Non Functional Requirements |
|---|---|
| What system does | How system performs |
| Features | Quality attributes |
| User operations | System constraints |
| Login, Payment | Security, Speed |

---

# Industry Example

## Online Banking System

Functional Requirements:

- Account creation
- Money transfer
- Transaction history

Non Functional Requirements:

Performance:

Transactions complete within seconds.

Security:

Multi-factor authentication.

Availability:

24/7 service.

Scalability:

Support millions of customers.

---

# Common Mistakes

## Mistake 1

Writing vague requirements.

Wrong:

"System should be fast."

Better:

"System should respond within 2 seconds."

---

## Mistake 2

Ignoring NFRs until testing.

Solution:

Define them during requirement phase.

---

## Mistake 3

Treating security as optional.

Solution:

Security is a core requirement.

---

# Best Practices

- Make requirements measurable
- Define acceptance criteria
- Prioritize important qualities
- Involve architects early
- Test quality attributes
- Review with stakeholders

---

# Interview Questions

1. What are Non Functional Requirements?
2. Difference between Functional and Non Functional Requirements?
3. Give examples of NFRs.
4. Explain performance requirements.
5. What is scalability?
6. Why are security requirements important?
7. How do NFRs influence system design?

---

# Cheat Sheet

```text
Non Functional Requirements

Define:

HOW the system behaves


Examples:

Performance
Security
Scalability
Reliability
Availability
Maintainability
Usability
```

---

# Summary

Non Functional Requirements define the quality and constraints of a software system. They ensure that software is not only functional but also secure, reliable, scalable, maintainable, and easy to use. Strong NFRs guide architecture decisions and help organizations build systems that perform effectively in real-world environments.
