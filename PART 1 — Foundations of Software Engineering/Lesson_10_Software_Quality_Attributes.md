# Lesson 10 — Software Quality Attributes

# Part 1 — Foundations of Software Engineering

> **Objective**
>
> Learn the quality attributes used to evaluate software in professional environments and understand why software that "works" is not always considered high-quality software.

---

# Introduction

Imagine buying two cars.

Both can drive from Pune to Mumbai.

But one is:

- Safer
- Faster
- More fuel efficient
- Easier to maintain
- More comfortable

Which is the better car?

The second one.

Software is evaluated the same way.

Correct functionality is only **one** aspect of quality.

---

# What are Software Quality Attributes?

Software Quality Attributes are measurable characteristics that describe **how well** software performs its intended job.

They answer questions such as:

- Is it secure?
- Is it reliable?
- Is it easy to maintain?
- Can it handle growth?
- Is it user-friendly?

---

# ISO/IEC 25010 Quality Model

A widely used international quality model defines the following major attributes:

```text
              Software Quality
                     |
 ------------------------------------------------------------
 |       |        |        |        |        |       |       |
Functional Reliability Performance Security Usability Maintainability Portability Compatibility
```

---

# 1. Functional Suitability

The software should provide the correct features and produce correct results.

Example:

```
UPI Transfer
     |
Money Sent to Correct Account
```

Questions:
- Does it meet business requirements?
- Does every feature work correctly?

---

# 2. Reliability

Reliability measures whether software performs consistently over time.

Example:

```
1000 Requests
      |
999 Successful
      |
High Reliability
```

Characteristics:
- Stability
- Fault tolerance
- Recoverability

Industry examples:
- Banking
- Healthcare
- Aviation

---

# 3. Performance Efficiency

Measures how efficiently software uses resources.

Resources:

- CPU
- Memory
- Disk
- Network

Example:

```
Search Time

0.2 sec ✓

8 sec ✗
```

---

# 4. Usability

Users should learn and operate the software easily.

Good usability includes:

- Simple navigation
- Clear messages
- Consistent design
- Accessibility

Example:

```
Login
Search
Checkout

(Simple)
```

---

# 5. Security

Protects:

- Users
- Data
- Privacy
- Business information

Security involves:

- Authentication
- Authorization
- Encryption
- Secure communication

Example:

```
Username
Password
   |
Verification
   |
Access Granted
```

---

# 6. Compatibility

Software should work correctly with other systems.

Examples:

- Payment gateway integration
- Browser compatibility
- API communication

```
Application
    |
-----------------------
| Browser
| Database
| Payment Gateway
| Email Service
```

---

# 7. Maintainability

Software should be easy to:

- Read
- Modify
- Test
- Improve

Good maintainability reduces long-term cost.

---

# 8. Portability

Software should run across different environments with minimal changes.

Example:

```
Windows

Linux

macOS

Cloud
```

---

# Additional Important Attributes

## Scalability

Ability to support increasing users and workloads.

```
100 Users
    |
10,000 Users
    |
1 Million Users
```

---

## Availability

Measures how often the software remains operational.

Examples:

- 99.9%
- 99.99%
- 99.999%

Higher availability means less downtime.

---

## Reusability

Reusable modules save development time.

```
Authentication Module

      |

Project A
Project B
Project C
```

---

## Testability

Software should be easy to verify through automated and manual tests.

Well-designed modules are easier to test independently.

---

# Real-Life Example

Food Delivery App

Quality checklist:

✓ Correct order placement

✓ Fast search

✓ Secure payments

✓ Easy navigation

✓ Available during peak hours

✓ Handles festival traffic

✓ Easy to update

---

# Industry Example

Before releasing a feature, companies typically evaluate:

```
Feature
   |
----------------------------------------
| Functional
| Reliable
| Secure
| Fast
| Maintainable
| Compatible
| Portable
```

Only after satisfying quality standards is the feature released.

---

# Comparative Study

| Attribute | Question It Answers |
|-----------|---------------------|
| Functional Suitability | Does it work correctly? |
| Reliability | Does it work consistently? |
| Performance | Is it fast and efficient? |
| Security | Is data protected? |
| Usability | Is it easy to use? |
| Compatibility | Does it work with other systems? |
| Maintainability | Is it easy to modify? |
| Portability | Can it run elsewhere? |
| Scalability | Can it grow? |
| Availability | Is it always accessible? |

---

# Common Misconceptions

❌ Software with many features is high quality.

✔ Quality depends on how well the software performs and evolves.

❌ Fast software is automatically good.

✔ Fast but insecure software is still poor quality.

❌ Testing alone creates quality.

✔ Quality is designed into the software from the beginning.

---

# Interview Questions

1. What are software quality attributes?
2. Explain ISO/IEC 25010.
3. Differentiate reliability and availability.
4. What is maintainability?
5. Why is compatibility important?
6. Explain portability with an example.
7. Differentiate functionality and performance.

---

# Cheat Sheet

```text
Quality Attributes

✓ Functional Suitability
✓ Reliability
✓ Performance Efficiency
✓ Security
✓ Usability
✓ Compatibility
✓ Maintainability
✓ Portability
✓ Scalability
✓ Availability
✓ Reusability
✓ Testability
```

---

# Summary

Software Quality Attributes define how well software satisfies user expectations beyond basic functionality. Professional software is evaluated for reliability, performance, security, usability, maintainability, compatibility, portability, and scalability. These attributes guide engineers in building systems that remain valuable, dependable, and easy to evolve throughout their lifecycle.
