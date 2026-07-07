# Lesson 102 --- User Stories

# Part 7 --- Requirements Engineering

> **Objective**
>
> Understand User Stories as a requirement technique, why they are used,
> their structure, characteristics, relationship with Agile development,
> and how they convert user needs into actionable software requirements.

------------------------------------------------------------------------

# Introduction

Software is created to solve user problems.

Instead of only describing technical features, modern teams describe
requirements from the user's perspective.

This is done using **User Stories**.

``` text
User Need

    ↓

User Story

    ↓

Development Task

    ↓

Software Feature
```

------------------------------------------------------------------------

# What is a User Story?

A **User Story** is a short description of a software requirement
written from the perspective of the user.

It explains:

-   Who needs something
-   What they need
-   Why they need it

------------------------------------------------------------------------

# Standard User Story Format

``` text
As a <user>

I want <feature>

So that <benefit>
```

------------------------------------------------------------------------

# Example

## Online Shopping System

    As a customer,
    I want to track my order,
    so that I know when my package will arrive.

User:

Customer

Feature:

Order Tracking

Benefit:

Know delivery status

------------------------------------------------------------------------

# Why Do We Need User Stories?

Traditional Requirement:

"Implement order tracking module."

Problem:

-   Focuses on implementation
-   Does not explain user value

User Story:

"As a customer, I want order tracking so that I can monitor delivery."

Benefits:

-   User-focused requirements
-   Better communication
-   Easier prioritization
-   Improved collaboration

------------------------------------------------------------------------

# Components of User Story

## 1. User / Actor

Who requires the feature?

Examples:

-   Customer
-   Admin
-   Student
-   Employee

------------------------------------------------------------------------

## 2. Feature / Action

What does the user want?

Examples:

-   Login
-   Search
-   Upload documents
-   Make payment

------------------------------------------------------------------------

## 3. Benefit / Goal

Why does the user need it?

Examples:

-   Save time
-   Improve security
-   Complete tasks easily

------------------------------------------------------------------------

# User Story Hierarchy

Large requirements are divided into smaller parts.

``` text
Epic

 ↓

Feature

 ↓

User Story

 ↓

Task
```

------------------------------------------------------------------------

# Example

## Banking Application

Epic:

Mobile Banking

Feature:

Money Transfer

User Story:

    As a customer,
    I want to transfer money,
    so that I can send payments easily.

Tasks:

-   Create transfer API
-   Design transfer screen
-   Add security validation
-   Test transactions

------------------------------------------------------------------------

# INVEST Criteria

A good User Story should follow INVEST.

``` text
I → Independent

N → Negotiable

V → Valuable

E → Estimable

S → Small

T → Testable
```

------------------------------------------------------------------------

# Independent

A story should be completed without depending heavily on another story.

Example:

Separate login and payment features.

------------------------------------------------------------------------

# Negotiable

A story describes the requirement, not the exact implementation.

Example:

Need:

"Secure login"

Solution:

Discussed by the team.

------------------------------------------------------------------------

# Valuable

Every story should provide value to users or business.

------------------------------------------------------------------------

# Estimable

The team should understand enough to estimate effort.

------------------------------------------------------------------------

# Small

Large stories should be divided.

Example:

Large:

"Build complete banking system"

Small:

-   Account creation
-   Balance check
-   Transfer money

------------------------------------------------------------------------

# Testable

A story must have clear validation criteria.

Example:

Login:

-   Valid credentials allow access
-   Invalid credentials show error

------------------------------------------------------------------------

# User Story and Acceptance Criteria

User Story:

    As a customer,
    I want password reset,
    so that I can recover my account.

Acceptance Criteria:

    ✓ Reset email is sent

    ✓ Link expires after defined time

    ✓ User can create a new password

------------------------------------------------------------------------

# User Story Lifecycle

``` text
User Requirement

        ↓

User Story Creation

        ↓

Product Backlog

        ↓

Estimation

        ↓

Sprint Selection

        ↓

Development

        ↓

Testing

        ↓

Completed Feature
```

------------------------------------------------------------------------

# User Stories in Requirement Engineering

User Stories help during:

-   Requirement gathering
-   Requirement documentation
-   Prioritization
-   Development planning
-   Testing

------------------------------------------------------------------------

# User Story vs Use Case

  User Story          Use Case
  ------------------- ------------------------------
  Short requirement   Detailed interaction
  User-focused        System behavior focused
  Common in Agile     Common in analysis/design
  Simple format       Includes flows and scenarios

------------------------------------------------------------------------

# User Story vs Functional Requirement

  User Story             Functional Requirement
  ---------------------- -----------------------------
  Describes user need    Describes system capability
  Business perspective   System perspective
  Used for planning      Used for specification

------------------------------------------------------------------------

# Industry Example

## Online Learning Platform

User Stories:

Student:

    As a student,
    I want to search courses,
    so that I can find relevant learning material.

Instructor:

    As an instructor,
    I want to upload videos,
    so that students can access lessons.

Admin:

    As an admin,
    I want to manage users,
    so that platform access remains controlled.

------------------------------------------------------------------------

# Common Mistakes

## Mistake 1

Writing technical tasks as stories.

Wrong:

"Create database table."

Better:

"As an admin, I want to manage users."

------------------------------------------------------------------------

## Mistake 2

Creating very large stories.

Solution:

Break into smaller valuable stories.

------------------------------------------------------------------------

## Mistake 3

Missing acceptance criteria.

Solution:

Define completion clearly.

------------------------------------------------------------------------

# Best Practices

-   Write from user perspective
-   Focus on business value
-   Keep stories small
-   Add acceptance criteria
-   Review with stakeholders
-   Update when requirements change

------------------------------------------------------------------------

# Interview Questions

1.  What is a User Story?
2.  Why are User Stories used?
3.  Explain User Story format.
4.  What is INVEST criteria?
5.  Difference between User Story and Use Case?
6.  What is acceptance criteria?
7.  Who creates User Stories?

------------------------------------------------------------------------

# Cheat Sheet

``` text
User Story

Who?
 ↓
Needs What?
 ↓
Why?

As a User
I want Feature
So that Benefit
```

------------------------------------------------------------------------

# Summary

User Stories provide a simple and effective way to capture software
requirements from the user's perspective. They help teams understand
customer needs, prioritize development work, and create valuable
software features. Combined with acceptance criteria and INVEST
principles, User Stories become clear, testable, and actionable
requirements.
