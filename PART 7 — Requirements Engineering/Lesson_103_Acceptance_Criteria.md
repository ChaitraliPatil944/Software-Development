# Lesson 103 --- Acceptance Criteria

# Part 7 --- Requirements Engineering

> **Objective**
>
> Understand Acceptance Criteria, why they are important, how they
> define completion, their relationship with User Stories and Definition
> of Done, formats, examples, and industry practices.

------------------------------------------------------------------------

# Introduction

A requirement is not complete just because developers finish coding.

The team needs a clear way to decide:

-   Is the feature working correctly?
-   Does it satisfy user expectations?
-   Can it be accepted by stakeholders?

This is defined using **Acceptance Criteria**.

``` text
User Story

      ↓

Acceptance Criteria

      ↓

Development

      ↓

Testing

      ↓

Accepted Feature
```

------------------------------------------------------------------------

# What is Acceptance Criteria?

**Acceptance Criteria** are conditions that a software feature must
satisfy before it is accepted as complete.

They define:

-   Expected behavior
-   Required outcomes
-   Conditions for approval

------------------------------------------------------------------------

# Why Do We Need Acceptance Criteria?

Without acceptance criteria:

``` text
Unclear Requirement

        ↓

Different Interpretations

        ↓

Incorrect Implementation

        ↓

Rework
```

Acceptance Criteria help:

-   Clarify requirements
-   Guide development
-   Create test cases
-   Reduce misunderstandings
-   Define completion

------------------------------------------------------------------------

# Acceptance Criteria Example

## User Story

    As a customer,
    I want to reset my password,
    so that I can recover my account.

## Acceptance Criteria

    ✓ User can request password reset

    ✓ Reset email is sent

    ✓ Link expires after a defined time

    ✓ User can create a new password

    ✓ User can login with the new password

------------------------------------------------------------------------

# Characteristics of Good Acceptance Criteria

Good acceptance criteria should be:

## 1. Clear

Easy for everyone to understand.

------------------------------------------------------------------------

## 2. Specific

Avoid vague statements.

Bad:

"System should be fast."

Good:

"Search results should appear within 2 seconds."

------------------------------------------------------------------------

## 3. Testable

The condition should be verifiable.

Example:

"User receives confirmation email after registration."

------------------------------------------------------------------------

## 4. Complete

Include all important scenarios.

------------------------------------------------------------------------

## 5. Consistent

Should not conflict with other requirements.

------------------------------------------------------------------------

# Types of Acceptance Criteria

## 1. Scenario-Based Criteria

Describe user behavior.

Example:

"When a user enters valid credentials, access should be granted."

------------------------------------------------------------------------

## 2. Rule-Based Criteria

Define business rules.

Example:

"Password must contain at least 8 characters."

------------------------------------------------------------------------

# Given-When-Then Format

A popular format used in Agile and Behavior Driven Development (BDD).

Structure:

``` text
Given

Initial condition

When

Action occurs

Then

Expected result
```

------------------------------------------------------------------------

# Example

## Login Feature

``` text
Given the user has a registered account

When the user enters valid username and password

Then the user should access the dashboard
```

------------------------------------------------------------------------

# Multiple Scenario Example

## Online Shopping Checkout

Scenario 1:

``` text
Given product is available

When customer completes payment

Then order should be created
```

------------------------------------------------------------------------

Scenario 2:

``` text
Given payment fails

When customer retries payment

Then system should allow another attempt
```

------------------------------------------------------------------------

# Acceptance Criteria Workflow

``` text
Requirement

      ↓

User Story

      ↓

Acceptance Criteria

      ↓

Development

      ↓

Testing

      ↓

Approval
```

------------------------------------------------------------------------

# Acceptance Criteria vs Definition of Done

  Acceptance Criteria              Definition of Done
  -------------------------------- --------------------------
  Specific to a User Story         Applies to all work
  Defines feature behavior         Defines quality standard
  Created for individual stories   Team agreement
  Example: Payment works           Code reviewed and tested

------------------------------------------------------------------------

# Acceptance Criteria vs Functional Requirements

  Acceptance Criteria             Functional Requirements
  ------------------------------- -------------------------------
  Defines acceptance conditions   Defines system capabilities
  More detailed                   Higher-level requirement
  Used for testing a story        Used for system specification

------------------------------------------------------------------------

# Industry Example

## Banking Application

User Story:

    As a customer,
    I want to transfer money,
    so that I can send payments.

Acceptance Criteria:

    ✓ User authentication required

    ✓ Recipient account must exist

    ✓ Transaction amount must be valid

    ✓ Confirmation message displayed

    ✓ Transaction recorded

------------------------------------------------------------------------

# Role of Team Members

## Product Owner

Responsible for:

-   Defining expected business behavior
-   Clarifying acceptance conditions

------------------------------------------------------------------------

## Developers

Use criteria to:

-   Understand requirements
-   Build features correctly

------------------------------------------------------------------------

## Testers

Use criteria to:

-   Create test cases
-   Validate functionality

------------------------------------------------------------------------

# Common Mistakes

## Mistake 1

Writing unclear criteria.

Wrong:

"System should work properly."

Better:

"System should display confirmation after successful payment."

------------------------------------------------------------------------

## Mistake 2

Ignoring error scenarios.

Solution:

Include failure conditions.

------------------------------------------------------------------------

## Mistake 3

Creating criteria after development.

Solution:

Define them before implementation.

------------------------------------------------------------------------

# Best Practices

-   Write criteria before development starts
-   Use simple language
-   Include positive and negative cases
-   Make every condition testable
-   Review with stakeholders
-   Keep criteria focused

------------------------------------------------------------------------

# Interview Questions

1.  What is Acceptance Criteria?
2.  Why is Acceptance Criteria important?
3.  Difference between Acceptance Criteria and Definition of Done?
4.  Explain Given-When-Then format.
5.  Who creates Acceptance Criteria?
6.  How does Acceptance Criteria help testing?
7.  Give an example of Acceptance Criteria.

------------------------------------------------------------------------

# Cheat Sheet

``` text
Acceptance Criteria

User Story

      ↓

Conditions

      ↓

Expected Behavior

      ↓

Testing

      ↓

Acceptance
```

------------------------------------------------------------------------

# Summary

Acceptance Criteria define the conditions that must be satisfied for a
User Story to be considered complete. They improve communication between
stakeholders, developers, and testers by creating a shared understanding
of expected behavior. Well-written acceptance criteria make requirements
clear, testable, and easier to deliver successfully.
