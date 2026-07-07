# Lesson 108 --- Requirement Engineering Practice

# Part 7 --- Requirements Engineering

> **Objective**
>
> Practice Requirement Engineering concepts through practical exercises
> including requirement identification, functional and non-functional
> requirement writing, user stories, use cases, acceptance criteria, and
> Requirement Traceability Matrix creation.

------------------------------------------------------------------------

# Introduction

Understanding requirements requires practice.

A requirement engineer should be able to:

-   Identify stakeholder needs
-   Convert problems into requirements
-   Write clear requirements
-   Validate requirements
-   Connect requirements with testing

``` text
Business Problem

        ↓

Requirements

        ↓

Design

        ↓

Development

        ↓

Testing
```

------------------------------------------------------------------------

# Section 1 --- Identify Requirements Practice

## Scenario

Build an Online Food Delivery Application.

Identify:

-   Stakeholders
-   Functional Requirements
-   Non Functional Requirements

------------------------------------------------------------------------

# Stakeholders

Possible stakeholders:

``` text
Customer

Restaurant Owner

Delivery Partner

Admin

Payment Provider
```

------------------------------------------------------------------------

# Functional Requirements

Examples:

    FR-001

    User should be able to register an account.


    FR-002

    Customer should be able to search restaurants.


    FR-003

    Customer should be able to place orders.


    FR-004

    Customer should be able to make payments.


    FR-005

    Delivery partner should update delivery status.

------------------------------------------------------------------------

# Non Functional Requirements

Examples:

    NFR-001

    Application should respond within 2 seconds.


    NFR-002

    User data should be encrypted.


    NFR-003

    System should support thousands of users.


    NFR-004

    Application should be available 99.9% of the time.

------------------------------------------------------------------------

# Section 2 --- Write User Stories Practice

## Scenario

Create User Stories for an E-Commerce System.

------------------------------------------------------------------------

## User Registration

    As a customer,

    I want to create an account,

    so that I can purchase products.

------------------------------------------------------------------------

## Product Search

    As a customer,

    I want to search products,

    so that I can find items easily.

------------------------------------------------------------------------

## Order Tracking

    As a customer,

    I want to track my order,

    so that I know delivery status.

------------------------------------------------------------------------

# Section 3 --- Acceptance Criteria Practice

## User Story

    As a customer,

    I want to reset my password,

    so that I can recover my account.

------------------------------------------------------------------------

## Acceptance Criteria

    ✓ User can request password reset

    ✓ System sends reset email

    ✓ Reset link has expiry time

    ✓ User can create a new password

    ✓ User can login with updated password

------------------------------------------------------------------------

# Section 4 --- Use Case Practice

## Scenario

ATM Withdrawal System

------------------------------------------------------------------------

# Use Case

Name:

Withdraw Cash

------------------------------------------------------------------------

Actor:

Customer

------------------------------------------------------------------------

Precondition:

Customer has a valid bank card.

------------------------------------------------------------------------

Main Flow:

``` text
Insert Card

      ↓

Enter PIN

      ↓

Enter Amount

      ↓

System Checks Balance

      ↓

Cash Dispensed
```

------------------------------------------------------------------------

Alternate Flow:

``` text
Invalid PIN

      ↓

Display Error Message
```

------------------------------------------------------------------------

Postcondition:

Transaction completed.

------------------------------------------------------------------------

# Section 5 --- Requirement Validation Practice

Check the requirement:

"System should be fast."

------------------------------------------------------------------------

## Problem

The requirement is unclear.

Questions:

-   How fast?
-   Under what conditions?
-   How will it be tested?

------------------------------------------------------------------------

## Improved Requirement

"System should display search results within 2 seconds."

------------------------------------------------------------------------

# Section 6 --- RTM Practice

Create Requirement Traceability Matrix.

## Example

  Requirement ID   Requirement      Test Case   Status
  ---------------- ---------------- ----------- ---------
  FR-001           User Login       TC-001      Passed
  FR-002           Product Search   TC-002      Passed
  FR-003           Payment          TC-003      Pending

------------------------------------------------------------------------

# Section 7 --- Requirement Analysis Scenario

## Situation

A customer says:

"I need a better shopping application."

------------------------------------------------------------------------

## Analysis

This is not a complete requirement.

Questions:

-   Better in what way?
-   Faster search?
-   More products?
-   Easier payment?
-   Better interface?

------------------------------------------------------------------------

## Converted Requirements

Functional:

-   Product search
-   Shopping cart
-   Online payment

Non Functional:

-   Fast response
-   Secure transactions
-   High availability

------------------------------------------------------------------------

# Section 8 --- Stakeholder Conflict Practice

## Scenario

Customer:

"Make login simple."

Security Team:

"Add multiple authentication steps."

------------------------------------------------------------------------

## Solution

Analyze:

-   User experience
-   Security risks
-   Business requirements

Possible solution:

Implement simple login with optional multi-factor authentication.

------------------------------------------------------------------------

# Section 9 --- Complete Requirement Engineering Simulation

## Project

Online Learning Platform

------------------------------------------------------------------------

# Stakeholders

``` text
Students

Teachers

Admin

Payment Provider
```

------------------------------------------------------------------------

# Functional Requirements

``` text
Student Registration

Course Search

Video Learning

Online Tests

Certificate Generation
```

------------------------------------------------------------------------

# Non Functional Requirements

``` text
Secure Login

Fast Video Loading

High Availability

Scalable Infrastructure
```

------------------------------------------------------------------------

# User Story

    As a student,

    I want to take online tests,

    so that I can evaluate my learning.

------------------------------------------------------------------------

# Acceptance Criteria

    ✓ Student can start test

    ✓ Questions are displayed

    ✓ Answers are saved

    ✓ Score is generated

------------------------------------------------------------------------

# Practice Questions

1.  Identify requirements for a banking application.
2.  Write five functional requirements for a hospital system.
3.  Write three non-functional requirements for an e-commerce website.
4.  Create user stories for a mobile application.
5.  Create acceptance criteria for login functionality.
6.  Create RTM for a small software system.
7.  Identify stakeholders for a railway booking system.

------------------------------------------------------------------------

# Self Evaluation

You should be able to:

✓ Identify stakeholders\
✓ Write functional requirements\
✓ Write non-functional requirements\
✓ Create user stories\
✓ Write acceptance criteria\
✓ Create use cases\
✓ Validate requirements\
✓ Build RTM

------------------------------------------------------------------------

# Summary

Requirement Engineering practice develops the ability to convert
real-world problems into clear software requirements. Through exercises
involving user stories, use cases, acceptance criteria, validation, and
traceability, engineers learn how professional software teams analyze
and manage requirements.
