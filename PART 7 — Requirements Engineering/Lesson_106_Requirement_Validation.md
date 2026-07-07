# Lesson 106 --- Requirement Validation

# Part 7 --- Requirements Engineering

> **Objective**
>
> Understand Requirement Validation, why requirements must be checked
> before development, validation activities, validation criteria,
> techniques, and the difference between verification and validation.

------------------------------------------------------------------------

# Introduction

A requirement document may contain mistakes:

-   Missing information
-   Incorrect assumptions
-   Conflicting requirements
-   Unrealistic expectations

Before software development begins, requirements must be reviewed and
confirmed.

This process is called **Requirement Validation**.

``` text
Requirement Document

        ↓

Validation

        ↓

Approved Requirements

        ↓

Development
```

------------------------------------------------------------------------

# What is Requirement Validation?

**Requirement Validation** is the process of checking whether documented
requirements are correct, complete, consistent, realistic, and suitable
for development.

It answers:

-   Are we building the right system?
-   Do requirements match stakeholder needs?
-   Can these requirements actually be implemented?

------------------------------------------------------------------------

# Why Do We Need Requirement Validation?

Without validation:

``` text
Incorrect Requirements

        ↓

Wrong Design

        ↓

Wrong Development

        ↓

Project Problems
```

Validation helps:

-   Reduce errors early
-   Avoid costly changes
-   Improve requirement quality
-   Confirm stakeholder expectations

------------------------------------------------------------------------

# Requirement Validation Process

``` text
Review Requirements

        ↓

Identify Issues

        ↓

Discuss With Stakeholders

        ↓

Correct Requirements

        ↓

Approve Final Version
```

------------------------------------------------------------------------

# Requirement Validation Criteria

A good requirement should satisfy:

``` text
Requirement Quality

        |
-----------------------
|    |    |    |      |
Correct Complete Consistent Feasible Testable
```

------------------------------------------------------------------------

# 1. Correctness

Requirements should represent actual stakeholder needs.

Example:

Wrong:

"System should generate reports automatically."

Question:

Which reports?

Who needs them?

------------------------------------------------------------------------

# 2. Completeness

All necessary information should be included.

Example:

Login requirement should include:

-   Username
-   Password
-   Error handling
-   Security rules

------------------------------------------------------------------------

# 3. Consistency

Requirements should not conflict with each other.

Example:

Requirement 1:

"Password must contain 8 characters."

Requirement 2:

"Password must contain minimum 12 characters."

Conflict must be resolved.

------------------------------------------------------------------------

# 4. Feasibility

Requirements should be technically and financially possible.

Example:

"System should support unlimited users with zero cost."

Needs analysis.

------------------------------------------------------------------------

# 5. Testability

Requirements should be measurable.

Bad:

"System should be fast."

Good:

"System should respond within 2 seconds."

------------------------------------------------------------------------

# Requirement Validation Techniques

## 1. Requirement Reviews

Stakeholders and team members review requirements.

Participants:

-   Business analysts
-   Developers
-   Testers
-   Customers

------------------------------------------------------------------------

## 2. Prototyping

Creating an early model to verify understanding.

Example:

Creating UI mockups before development.

------------------------------------------------------------------------

## 3. Test Case Generation

If requirements cannot create test cases, they may be unclear.

------------------------------------------------------------------------

## 4. Stakeholder Feedback

Stakeholders confirm whether requirements match expectations.

------------------------------------------------------------------------

# Requirement Validation Example

## Online Banking System

Requirement:

"Customer can transfer money."

Validation Questions:

Can customer transfer money?

✓ Correct

Is amount limit defined?

✓ Complete

Does security requirement exist?

✓ Consistent

Can it be tested?

✓ Testable

------------------------------------------------------------------------

# Requirement Verification vs Validation

  -----------------------------------------------------------------------
  Verification                        Validation
  ----------------------------------- -----------------------------------
  Are we building the product         Are we building the right product?
  correctly?                          

  Checks documents and specifications Checks stakeholder needs

  Process-focused                     User-focused

  Example: Requirement review         Example: Customer approval
  -----------------------------------------------------------------------

------------------------------------------------------------------------

# Requirement Validation in SDLC

``` text
Requirement Engineering

        ↓

Validation

        ↓

Design

        ↓

Development

        ↓

Testing
```

------------------------------------------------------------------------

# Industry Example

## Healthcare Application

Requirement:

"Patients should book appointments online."

Validation:

Correct:

Patients need appointment booking.

Complete:

Includes:

-   Doctor selection
-   Date selection
-   Confirmation

Consistent:

Matches hospital workflow.

Testable:

Appointment can be created and verified.

------------------------------------------------------------------------

# Common Validation Problems

## 1. Ambiguous Requirements

Problem:

Different people interpret differently.

Solution:

Use clear language.

------------------------------------------------------------------------

## 2. Missing Requirements

Problem:

Important functionality forgotten.

Solution:

Perform stakeholder reviews.

------------------------------------------------------------------------

## 3. Changing Requirements

Problem:

Business needs evolve.

Solution:

Maintain requirement management process.

------------------------------------------------------------------------

# Best Practices

-   Review requirements early
-   Involve stakeholders
-   Use prototypes
-   Make requirements measurable
-   Maintain documentation
-   Link requirements with testing

------------------------------------------------------------------------

# Interview Questions

1.  What is Requirement Validation?
2.  Why is requirement validation important?
3.  Explain validation criteria.
4.  Difference between verification and validation?
5.  What techniques are used for requirement validation?
6.  How do you check if a requirement is testable?
7.  Who participates in requirement validation?

------------------------------------------------------------------------

# Cheat Sheet

``` text
Requirement Validation

Check:

✓ Correct
✓ Complete
✓ Consistent
✓ Feasible
✓ Testable

        ↓

Approved Requirements
```

------------------------------------------------------------------------

# Summary

Requirement Validation ensures that software requirements are accurate,
complete, realistic, and aligned with stakeholder expectations. By
reviewing requirements before development, teams reduce risks, prevent
misunderstandings, and build software that solves the correct problem.
