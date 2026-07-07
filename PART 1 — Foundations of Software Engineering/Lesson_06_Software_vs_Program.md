# Lesson 6 — Software vs Program

# Part 1 — Foundations of Software Engineering

> **Objective**
>
> Understand the difference between a **program** and **software**, why the terms are not interchangeable, and how this distinction is viewed in academia and the software industry.

---

# Introduction

Many beginners use the words **program** and **software** as if they mean the same thing.

They are closely related, but they are **not identical**.

Think of it this way:

- A **program** is one component.
- **Software** is the complete product delivered to users.

---

# What is a Program?

A **program** is a set of instructions written in a programming language that tells a computer how to perform a specific task.

Examples:

- Calculator program
- Sorting program
- Temperature converter
- Login validation script

Simple view:

```text
Input
  |
Program
  |
Output
```

A program mainly focuses on solving one problem.

---

# What is Software?

**Software** is a complete system consisting of:

- Programs
- Documentation
- Configuration files
- Databases
- Libraries
- User interface
- Installation files
- User manuals
- Maintenance support

```text
                 Software
                     |
 ------------------------------------------------
 |        |        |       |        |            |
Programs  Database Docs  Config   UI      Libraries
```

Without these supporting components, users often cannot install, operate, or maintain the product effectively.

---

# Real-Life Analogy

Imagine a car.

### Program

A single engine.

### Software

The complete car.

```text
Car
 |
 +-- Engine
 +-- Wheels
 +-- Steering
 +-- Brakes
 +-- Dashboard
 +-- Electronics
```

The engine is essential, but it is **not the entire car**.

Similarly:

```text
Software
 |
 +-- Programs
 +-- Documentation
 +-- Database
 +-- Configuration
 +-- UI
```

---

# Example 1: Calculator

### Program

A Python script:

```python
print(10 + 20)
```

It performs one calculation.

### Software

A calculator application includes:

- GUI
- Calculation logic
- History
- Settings
- Installer
- Documentation

---

# Example 2: Banking System

A banking application contains:

```text
Internet Banking
        |
---------------------------------------
|        |        |         |          |
Login  Transfer  Cards   Database  Reports
```

Each module contains many programs.

Together they form **software**.

---

# Industry Example

Consider an online shopping platform.

Programs include:

- Login service
- Payment service
- Inventory service
- Recommendation engine
- Notification service

Software additionally includes:

- API documentation
- Deployment scripts
- Databases
- Monitoring
- Configuration
- User manuals

The customer receives the **software**, not individual programs.

---

# Key Differences

| Program | Software |
|---------|----------|
| Collection of instructions | Complete product |
| Solves a specific task | Solves business problems |
| Smaller | Larger |
| Can be written by one developer | Usually built by teams |
| Minimal documentation | Extensive documentation |
| Limited scope | Entire lifecycle |

---

# Relationship

```text
Program
    |
Many Programs
    |
Application
    |
Software Product
```

Not every program becomes software.

Every software product contains one or more programs.

---

# Why the Difference Matters

Suppose a customer asks for:

> "Build an inventory management system."

If developers only deliver source code, the customer still lacks:

- Installation guide
- Database
- Configuration
- User interface
- Documentation
- Updates

Engineering delivers the **complete solution**, not just code.

---

# Common Misconceptions

❌ Every program is software.

✔ Every software product contains programs, but software is much more than code.

❌ Software only means source code.

✔ Software also includes documentation, data, configuration, deployment, and maintenance.

---

# Interview Questions

1. Differentiate between a program and software.
2. Can software exist without programs?
3. Can a single program be called software?
4. Why does software include documentation?
5. Give a real-world example of software and identify its programs.

---

# Cheat Sheet

```text
Program
 |
Specific Task
 |
Source Code

Software
 |
Programs
+ Documentation
+ Database
+ UI
+ Configurations
+ Libraries
+ Support
```

---

# Summary

A **program** is a set of instructions designed to perform a particular task, while **software** is a complete, usable product that combines multiple programs with documentation, configuration, interfaces, data, and maintenance support. Understanding this distinction is fundamental to Software Engineering because engineers build software products, not isolated programs.
