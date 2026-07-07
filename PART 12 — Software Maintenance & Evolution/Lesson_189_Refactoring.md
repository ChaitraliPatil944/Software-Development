# Lesson 189 --- Refactoring

# Part 12 --- Software Maintenance

> **Objective**
>
> Understand refactoring, why it is needed, refactoring principles, code
> smells, common refactoring techniques, refactoring vs rewriting, the
> refactoring process, benefits, risks, best practices, and its role in
> improving software quality.

------------------------------------------------------------------------

# Introduction

Software systems continuously evolve.

As features are added, code can become:

-   Complex
-   Difficult to understand
-   Hard to modify
-   Difficult to test

Improving the internal structure of code without changing its external
behavior is called **Refactoring**.

``` text
Existing Code

      ↓

Improve Internal Structure

      ↓

Better Code

      ↓

Same Behavior
```

------------------------------------------------------------------------

# What is Refactoring?

**Refactoring** is the process of improving the design and structure of
existing code without changing what the software does.

Simple definition:

    Refactoring = Improving Code Quality Without Changing Functionality

------------------------------------------------------------------------

# Why is Refactoring Needed?

Over time, software accumulates problems:

-   Duplicate code
-   Complex logic
-   Poor design
-   Difficult maintenance
-   Technical debt

Without refactoring:

    Code Growth

          ↓

    Complexity Increase

          ↓

    Maintenance Difficulty

------------------------------------------------------------------------

# Goals of Refactoring

Refactoring improves:

-   Code readability
-   Maintainability
-   Performance
-   Testability
-   Software design

------------------------------------------------------------------------

# Refactoring Principles

## 1. Preserve Behavior

The software should work exactly as before.

Example:

Before:

    Calculate Price()

After:

    Improved Calculate Price()

Output remains the same.

------------------------------------------------------------------------

## 2. Small Changes

Refactoring should be performed gradually.

Example:

    Small Change

     ↓

    Test

     ↓

    Next Improvement

------------------------------------------------------------------------

## 3. Continuous Improvement

Refactoring should happen regularly, not only during problems.

------------------------------------------------------------------------

## 4. Use Automated Testing

Tests ensure that improvements do not break functionality.

------------------------------------------------------------------------

# What are Code Smells?

A **Code Smell** is a sign that code may have design problems.

It does not always mean a bug exists.

Examples:

-   Duplicate code
-   Large classes
-   Long methods
-   Complex conditions
-   Poor naming

------------------------------------------------------------------------

# Common Code Smells

## 1. Duplicate Code

Same logic appears multiple times.

Problem:

    Same Code

    Same Code

    Same Code

Solution:

Create reusable functions.

------------------------------------------------------------------------

## 2. Long Method

A method contains too many responsibilities.

Solution:

Split into smaller methods.

------------------------------------------------------------------------

## 3. Large Class

A class does too much.

Solution:

Separate responsibilities.

------------------------------------------------------------------------

## 4. Poor Naming

Unclear names reduce readability.

Example:

Bad:

    x1

Better:

    customerCount

------------------------------------------------------------------------

## 5. Complex Conditions

Too many nested conditions.

Solution:

Simplify logic.

------------------------------------------------------------------------

# Common Refactoring Techniques

## 1. Extract Method

Move part of a large method into a separate method.

Before:

    Large Function

After:

    Main Function

    +

    Helper Functions

------------------------------------------------------------------------

## 2. Rename Variables

Improve readability.

Example:

Before:

    a

After:

    totalAmount

------------------------------------------------------------------------

## 3. Remove Duplicate Code

Create reusable components.

------------------------------------------------------------------------

## 4. Extract Class

Split a large class into smaller classes.

------------------------------------------------------------------------

## 5. Simplify Conditional Logic

Make decision structures easier to understand.

------------------------------------------------------------------------

## 6. Replace Magic Numbers

Before:

    if(age > 18)

After:

    if(age > LEGAL_AGE)

------------------------------------------------------------------------

# Refactoring Process

``` text
Identify Code Problem

        ↓

Create Tests

        ↓

Apply Small Change

        ↓

Run Tests

        ↓

Review Code

        ↓

Deploy
```

------------------------------------------------------------------------

# Refactoring vs Rewriting

  Refactoring              Rewriting
  ------------------------ --------------------------
  Improves existing code   Creates new system
  Keeps functionality      May change functionality
  Lower risk               Higher risk
  Incremental              Large effort

------------------------------------------------------------------------

# Benefits of Refactoring

## 1. Better Readability

Developers understand code faster.

------------------------------------------------------------------------

## 2. Easier Maintenance

Future changes require less effort.

------------------------------------------------------------------------

## 3. Reduced Technical Debt

Improves code quality.

------------------------------------------------------------------------

## 4. Better Testing

Cleaner code is easier to test.

------------------------------------------------------------------------

## 5. Improved Development Speed

Future features can be added faster.

------------------------------------------------------------------------

# Risks of Refactoring

## 1. Introducing Bugs

Changes may affect existing behavior.

------------------------------------------------------------------------

## 2. Time Requirement

Refactoring requires developer effort.

------------------------------------------------------------------------

## 3. Poor Planning

Large uncontrolled changes create problems.

------------------------------------------------------------------------

# Refactoring and Technical Debt

Technical debt increases when code quality decreases.

Refactoring reduces debt.

``` text
Technical Debt

      ↓

Refactoring

      ↓

Cleaner Code

      ↓

Lower Maintenance Cost
```

------------------------------------------------------------------------

# Refactoring in Agile

Agile teams use:

-   Refactoring tasks
-   Code reviews
-   Continuous improvement
-   Technical debt management

------------------------------------------------------------------------

# Refactoring in DevOps

DevOps supports refactoring through:

-   Automated testing
-   CI pipelines
-   Code quality tools
-   Continuous delivery

------------------------------------------------------------------------

# Refactoring Tools

Common tools:

-   IntelliJ IDEA
-   Visual Studio Code extensions
-   Eclipse refactoring tools
-   SonarQube
-   SonarLint

------------------------------------------------------------------------

# Real-World Example

## Banking Application

Problem:

    Transaction Module

    5000 Lines of Code

Issues:

-   Difficult maintenance
-   Slow changes

Refactoring:

    Split Module

    Improve Structure

    Add Tests

Result:

    Cleaner Code

    Faster Development

    Lower Risk

------------------------------------------------------------------------

# Best Practices

## 1. Refactor Regularly

Do not wait until code becomes unmanageable.

------------------------------------------------------------------------

## 2. Write Tests Before Refactoring

Tests protect existing behavior.

------------------------------------------------------------------------

## 3. Make Small Changes

Avoid large risky modifications.

------------------------------------------------------------------------

## 4. Review Changes

Use code reviews.

------------------------------------------------------------------------

## 5. Follow Coding Standards

Maintain consistency.

------------------------------------------------------------------------

# Interview Questions

## 1. What is refactoring?

Refactoring improves the internal structure of code without changing its
external behavior.

------------------------------------------------------------------------

## 2. Why is refactoring important?

It improves maintainability, readability, and reduces technical debt.

------------------------------------------------------------------------

## 3. What are code smells?

Code smells are indicators of poor code design.

------------------------------------------------------------------------

## 4. Difference between refactoring and rewriting?

Refactoring improves existing code.

Rewriting creates a new implementation.

------------------------------------------------------------------------

## 5. What are common refactoring techniques?

Examples:

-   Extract Method
-   Rename Variables
-   Remove Duplicate Code
-   Extract Class

------------------------------------------------------------------------

# Cheat Sheet

``` text
Refactoring

Identify Problems

        ↓

Improve Code Structure

        ↓

Run Tests

        ↓

Better Maintainable Software
```

------------------------------------------------------------------------

# Summary

Refactoring is a software maintenance activity that improves code
quality without changing functionality. It reduces technical debt,
improves maintainability, and helps software remain flexible as it
grows.

Good developers do not only write code; they continuously improve the
code they maintain.
