# Lesson 5 — Characteristics of Good Software

# Part 1 — Foundations of Software Engineering

> **Objective**
>
> Learn what makes software "good", why quality attributes matter, and how companies evaluate software beyond simply checking whether it works.

---

# Introduction

Writing software that runs is **not enough**.

Imagine buying a car.

It should:
- Start every time
- Be safe
- Be fuel efficient
- Be easy to maintain
- Last for years

Software is no different.

A program that merely produces the correct output once is **not necessarily good software**.

---

# What is Good Software?

Good software satisfies user requirements while being:

- Reliable
- Efficient
- Secure
- Maintainable
- Scalable
- Usable

These qualities determine whether software succeeds in the real world.

---

# Why Do These Characteristics Matter?

Consider an online banking application.

```
Customer
    |
Transfer Money
    |
Software Crashes
    |
Money Lost
```

Even if the code is "correct", poor reliability destroys trust.

Quality attributes reduce business risk.

---

# Core Characteristics

## 1. Correctness

The software should do exactly what users expect.

Example:

```
2 + 2

Expected = 4
Actual   = 4
```

If requirements are met consistently, the software is correct.

---

## 2. Reliability

The software should work consistently without unexpected failures.

Example:
- ATM machine
- Air traffic control
- Hospital software

```
Request
   |
Process
   |
Correct Response
   |
Repeat Thousands of Times
```

---

## 3. Maintainability

Software should be easy to modify.

Example:

An e-commerce website needs a new payment method.

Poor software:

```
Change One File
     |
20 Bugs
```

Good software:

```
Well-Designed Modules
        |
Small Change
        |
System Still Stable
```

---

## 4. Scalability

Software should handle increasing users and data.

Example:

```
100 Users
   |
1,000 Users
   |
100,000 Users
   |
1 Million Users
```

The system should continue performing well.

---

## 5. Performance (Efficiency)

Performance measures how efficiently software uses resources.

Resources include:

- CPU
- Memory
- Disk
- Network

Example:

```
Slow Search = 8 sec

Fast Search = 0.2 sec
```

---

## 6. Security

Software must protect:

- Data
- Users
- Privacy

Security includes:

- Authentication
- Authorization
- Encryption
- Secure communication

---

## 7. Usability

Software should be easy to learn and use.

Example:

Compare:

```
Simple Interface

Login
Search
Checkout
```

vs

```
50 Buttons
Confusing Menu
Hidden Features
```

Users prefer simplicity.

---

## 8. Availability

Software should remain accessible whenever users need it.

Example:

Cloud services often target:

```
99.9%

99.99%

99.999% Availability
```

Higher availability means less downtime.

---

## 9. Portability

Software should run on different platforms.

Example:

```
Windows

Linux

macOS

Cloud
```

without major changes.

---

## 10. Reusability

Reusable modules reduce development time.

Example:

```
Login Module

     |

Website A

Website B

Website C
```

Write once, reuse many times.

---

## 11. Flexibility

Software should adapt to future requirements without major redesign.

Example:

Adding:

- Dark mode
- New payment gateway
- New language

should not require rebuilding the entire system.

---

## ASCII Overview

```
                Good Software
                     |
 -------------------------------------------------
 |      |        |       |       |        |      |
Correct Reliable Secure Efficient Maintainable Usable
                     |
                 Scalable
```

---

# Real-Life Example

## Food Delivery App

Good software should:

✔ Correctly place orders

✔ Stay online during lunch hours

✔ Protect payment information

✔ Support millions of users

✔ Allow new restaurants to be added easily

✔ Be simple for customers to use

---

# Industry Example

Large technology companies evaluate software continuously.

Before releasing a feature, engineers check:

- Does it work?
- Is it secure?
- Is it fast?
- Can it scale?
- Is it maintainable?
- Is it user-friendly?

Quality is not tested only at the end. It is considered throughout development.

---

# Comparative Study

| Poor Software | Good Software |
|---------------|---------------|
| Frequent crashes | Stable |
| Slow | Fast |
| Difficult to update | Easy to maintain |
| Insecure | Secure |
| Confusing UI | User-friendly |
| Cannot handle growth | Scalable |

---

# Common Misconceptions

❌ If software works once, it is good.

✔ Good software continues to work reliably over time.

❌ Fast software is always good.

✔ Fast but insecure software is still poor quality.

❌ More features mean better software.

✔ Useful, maintainable features matter more than feature count.

---

# Interview Questions

1. What are the characteristics of good software?
2. Differentiate reliability and availability.
3. What is maintainability?
4. Why is scalability important?
5. Explain portability with an example.
6. What is software usability?

---

# Cheat Sheet

```
Good Software

✓ Correct
✓ Reliable
✓ Efficient
✓ Secure
✓ Maintainable
✓ Scalable
✓ Usable
✓ Portable
✓ Flexible
✓ Available
✓ Reusable
```

---

# Summary

Good software is more than functional code. It must consistently satisfy user needs while remaining reliable, secure, maintainable, scalable, and easy to use. These quality characteristics help software survive real-world usage, changing requirements, and long-term maintenance, making them essential goals of Software Engineering.
