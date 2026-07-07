# Lesson 105 --- Requirement Traceability Matrix (RTM)

# Part 7 --- Requirements Engineering

> **Objective**
>
> Understand Requirement Traceability Matrix (RTM), why traceability is
> important, how requirements are mapped with design, development, and
> testing, and how RTM helps maintain software quality.

------------------------------------------------------------------------

# Introduction

Software projects contain many requirements.

Teams need to ensure:

-   Every requirement is implemented
-   Every requirement is tested
-   No requirement is forgotten

This is achieved using a **Requirement Traceability Matrix**.

``` text
Requirement

      ↓

Design

      ↓

Development

      ↓

Testing

      ↓

Final Product
```

------------------------------------------------------------------------

# What is Requirement Traceability Matrix?

A **Requirement Traceability Matrix (RTM)** is a document that maps
software requirements with their related artifacts such as:

-   Design components
-   Code modules
-   Test cases
-   Test results

It provides complete traceability throughout the software development
lifecycle.

------------------------------------------------------------------------

# Why Do We Need RTM?

Without RTM:

``` text
Requirement

      ↓

Development

      ↓

Unknown Test Coverage
```

Problems:

-   Missing features
-   Untested requirements
-   Difficult impact analysis
-   Poor quality control

With RTM:

``` text
Requirement

      ↓

Implementation

      ↓

Testing

      ↓

Validation
```

------------------------------------------------------------------------

# Purpose of RTM

RTM helps to:

-   Track requirement implementation
-   Ensure complete test coverage
-   Identify missing requirements
-   Manage changes
-   Support audits
-   Improve software quality

------------------------------------------------------------------------

# RTM Structure

A typical RTM contains:

  Requirement ID   Requirement   Design Module   Test Case ID   Status
  ---------------- ------------- --------------- -------------- --------

------------------------------------------------------------------------

# RTM Example

## Banking Application

  Requirement ID   Requirement           Test Case   Status
  ---------------- --------------------- ----------- ---------
  FR-001           User Login            TC-001      Passed
  FR-002           Money Transfer        TC-002      Passed
  FR-003           Transaction History   TC-003      Pending

------------------------------------------------------------------------

# Types of Traceability

There are mainly two types:

``` text
Traceability

      |
      |
-----------------
|               |
Forward       Backward
```

------------------------------------------------------------------------

# 1. Forward Traceability

Tracks:

Requirement → Test Cases

Purpose:

Ensure every requirement is tested.

Example:

``` text
Requirement:

User Login

        ↓

Test Case:

Verify Login Functionality
```

------------------------------------------------------------------------

# 2. Backward Traceability

Tracks:

Test Case → Requirement

Purpose:

Ensure every test has a valid requirement.

Example:

``` text
Test Case:

Password Reset Test

        ↓

Requirement:

Password Recovery Feature
```

------------------------------------------------------------------------

# Bidirectional Traceability

The best practice is maintaining both directions.

``` text
Requirement

      ↕

Test Case
```

Benefits:

-   Complete coverage
-   Better impact analysis
-   Easier maintenance

------------------------------------------------------------------------

# RTM in SDLC

``` text
Requirement Phase

        ↓

Create RTM

        ↓

Design

        ↓

Development

        ↓

Testing

        ↓

Update RTM

        ↓

Release
```

------------------------------------------------------------------------

# RTM and Testing

Testers use RTM to verify:

-   Every requirement has test cases
-   Test cases match requirements
-   Testing is complete

Example:

Requirement:

"User can reset password."

Test Cases:

✓ Reset email generated

✓ Password changed successfully

✓ Invalid link rejected

------------------------------------------------------------------------

# RTM and Change Management

Requirements change frequently.

Example:

New requirement:

"Add two-factor authentication."

RTM helps identify:

Affected:

-   Design
-   Code
-   Test cases

------------------------------------------------------------------------

# Industry Example

## E-Commerce System

Requirements:

FR-001:

User Registration

Mapped:

Design:

User Module

Code:

Authentication Service

Testing:

TC-001 Registration Test

------------------------------------------------------------------------

FR-002:

Payment Processing

Mapped:

Design:

Payment Module

Code:

Payment API

Testing:

TC-002 Payment Test

------------------------------------------------------------------------

# Benefits of RTM

-   Better requirement coverage
-   Easier testing
-   Reduced risk
-   Improved documentation
-   Faster debugging
-   Better change management

------------------------------------------------------------------------

# Common Mistakes

## Mistake 1

Creating RTM only at the end.

Solution:

Maintain it throughout the project.

------------------------------------------------------------------------

## Mistake 2

Not updating RTM after requirement changes.

Solution:

Keep traceability current.

------------------------------------------------------------------------

## Mistake 3

Mapping only functional requirements.

Solution:

Include important non-functional requirements also.

------------------------------------------------------------------------

# RTM vs Test Case Document

  RTM                          Test Case Document
  ---------------------------- --------------------------
  Maps requirements to tests   Describes test execution
  Ensures coverage             Defines testing steps
  Traceability purpose         Testing purpose

------------------------------------------------------------------------

# Interview Questions

1.  What is Requirement Traceability Matrix?
2.  Why is RTM important?
3.  What are types of traceability?
4.  Difference between forward and backward traceability?
5.  How does RTM help testing?
6.  When should RTM be created?
7.  What information does RTM contain?

------------------------------------------------------------------------

# Cheat Sheet

``` text
RTM

Requirement

     ↓

Design

     ↓

Code

     ↓

Test Case

     ↓

Validation
```

------------------------------------------------------------------------

# Summary

Requirement Traceability Matrix connects requirements with design,
implementation, and testing activities. It ensures that every
requirement is properly implemented and verified. RTM improves quality,
supports change management, and provides confidence that the final
software system meets stakeholder expectations.
