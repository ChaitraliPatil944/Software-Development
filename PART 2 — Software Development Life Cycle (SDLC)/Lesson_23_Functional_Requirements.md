# Lesson 23 — Functional Requirements

# Part 2 — Software Development Life Cycle (SDLC)

> **Objective**
>
> Understand what Functional Requirements are, why they are essential, how to identify and document them, and how they guide software design, development, testing, and acceptance.

---

# Introduction

Imagine a customer says:

> "I need an online banking application."

This statement is too broad.

Engineers must identify **exactly what the software should do**.

Examples:

- User can register.
- User can log in.
- User can transfer money.
- User can view transaction history.
- User can download account statements.

These are **Functional Requirements**.

---

# What are Functional Requirements?

A **Functional Requirement (FR)** describes **what the system must do**.

It defines the features, services, and behaviors the software must provide to meet business and user needs.

Simply put:

```text
Functional Requirement

=
Expected Functionality
```

---

# Why are Functional Requirements Important?

Without clear functional requirements:

```text
Customer
    |
Vague Idea
    |
Developers Guess
    |
Wrong Software
```

With proper functional requirements:

```text
Business Need
      |
Functional Requirements
      |
Design
      |
Development
      |
Testing
      |
Correct Software
```

---

# Characteristics of Good Functional Requirements

A good functional requirement should be:

- Clear
- Complete
- Consistent
- Testable
- Measurable
- Traceable
- Unambiguous

Bad:

> "The website should be easy to use."

Good:

> "The user shall be able to register using email and password."

---

# Functional Requirement Lifecycle

```text
Business Need
      |
Requirement Gathering
      |
Requirement Analysis
      |
Functional Requirements
      |
SRS
      |
Design
      |
Development
      |
Testing
```

---

# Sources of Functional Requirements

Requirements can come from:

- Customers
- End Users
- Business Analysts
- Product Owner
- Existing Software
- Government Regulations

---

# Examples

## Example 1 — E-Commerce Website

Functional Requirements:

- User Registration
- Login
- Search Products
- Add to Cart
- Remove from Cart
- Online Payment
- Order Tracking
- Wishlist
- Product Reviews

---

## Example 2 — Hospital Management System

Functional Requirements:

- Register Patient
- Schedule Appointment
- Generate Bills
- Manage Pharmacy
- Generate Reports
- Store Medical Records

---

## Example 3 — Food Delivery Application

Functional Requirements:

Customer:

- Register
- Browse Restaurants
- Place Orders
- Make Payment
- Track Delivery

Restaurant:

- Accept Orders
- Update Menu
- Manage Inventory

Delivery Partner:

- Accept Delivery
- Update Delivery Status
- Navigate to Customer

---

# Functional Requirement Template

```text
Requirement ID : FR-001

Title :
User Login

Description :
The system shall allow registered users to log in
using email and password.

Priority :
High

Actor :
Customer

Acceptance Criteria :
Valid credentials provide access.
Invalid credentials display an error.
```

---

# User Stories

In Agile projects, functional requirements are often written as **User Stories**.

Example:

> As a customer,
> I want to search products,
> so that I can quickly find items to purchase.

---

# Use Cases

Functional requirements can also be represented as Use Cases.

```text
Customer
    |
Login
    |
Browse Products
    |
Add to Cart
    |
Checkout
```

---

# Acceptance Criteria

Every functional requirement should have acceptance criteria.

Example:

Requirement:

> User Login

Acceptance Criteria:

- Valid credentials allow login.
- Invalid password shows an error.
- Locked account cannot log in.

---

# Functional Requirements vs Non-Functional Requirements

| Functional | Non-Functional |
|------------|----------------|
| What system does | How well it performs |
| Login | Login within 2 seconds |
| Payment | Secure payment |
| Search | Search response < 1 sec |

---

# Industry Example

## Online Banking

Functional Requirements:

- Account Creation
- Login
- Balance Inquiry
- Fund Transfer
- Statement Download
- Bill Payments
- Beneficiary Management

QA engineers create test cases directly from these requirements.

---

# Stakeholders

```text
Customer
     |
Business Analyst
     |
Product Owner
     |
Developers
     |
QA Engineers
```

Everyone must agree before development begins.

---

# Common Mistakes

❌ Writing vague requirements.

✔ Use clear, measurable language.

❌ Combining multiple requirements into one.

✔ One requirement should describe one function.

❌ Forgetting acceptance criteria.

✔ Define how success will be verified.

---

# Best Practices

- Use simple language.
- Assign unique IDs.
- Keep one function per requirement.
- Make every requirement testable.
- Review with stakeholders.
- Maintain traceability.

---

# Interview Questions

1. What are Functional Requirements?
2. Give examples of Functional Requirements.
3. How are Functional and Non-Functional Requirements different?
4. What makes a good Functional Requirement?
5. What is a User Story?
6. Why are acceptance criteria important?

---

# Cheat Sheet

```text
Functional Requirement

Answers:

"What should the software do?"

Examples

✓ Login
✓ Register
✓ Search
✓ Payment
✓ Reports
✓ Notifications

Formats

✓ SRS
✓ User Stories
✓ Use Cases
```

---

# Summary

Functional Requirements define the features and behaviors a software system must provide. They form the foundation for software design, development, testing, and customer acceptance. Well-written functional requirements are clear, testable, traceable, and aligned with business goals, ensuring that the final product delivers the expected functionality.
