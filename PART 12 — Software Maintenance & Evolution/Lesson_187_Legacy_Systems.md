# Lesson 187 --- Legacy Systems

# Part 12 --- Software Maintenance

> **Objective**
>
> Understand legacy systems, why they exist, challenges of maintaining
> old software, legacy modernization approaches, migration strategies,
> examples, best practices, and their importance in software
> maintenance.

------------------------------------------------------------------------

# Introduction

Many organizations depend on software systems that were built years or
even decades ago.

These systems may still perform critical business functions.

Examples:

-   Banking systems
-   Government applications
-   Enterprise software

Such systems are called **Legacy Systems**.

``` text
Old Software

      ↓

Still Used

      ↓

Legacy System
```

------------------------------------------------------------------------

# What is a Legacy System?

A **Legacy System** is an old software system or technology that is
still being used by an organization, even though it may use outdated
technologies.

A legacy system can include:

-   Old applications
-   Old programming languages
-   Old databases
-   Outdated infrastructure

------------------------------------------------------------------------

# Why Do Legacy Systems Exist?

Legacy systems exist because:

-   They perform important business functions
-   Replacing them is expensive
-   Migration is risky
-   They contain valuable business logic
-   Users depend on them

------------------------------------------------------------------------

# Examples of Legacy Technologies

Examples:

## Programming Languages

-   COBOL
-   FORTRAN
-   Older Java versions

------------------------------------------------------------------------

## Databases

-   Older database systems
-   Mainframe databases

------------------------------------------------------------------------

## Applications

-   Banking transaction systems
-   Government record systems
-   Enterprise applications

------------------------------------------------------------------------

# Characteristics of Legacy Systems

## 1. Old Technology Stack

Uses outdated tools and platforms.

------------------------------------------------------------------------

## 2. Difficult Maintenance

Changes require significant effort.

------------------------------------------------------------------------

## 3. Poor Documentation

Original knowledge may be unavailable.

------------------------------------------------------------------------

## 4. High Business Dependency

Organizations cannot easily stop them.

------------------------------------------------------------------------

## 5. Limited Scalability

Modern requirements may exceed capabilities.

------------------------------------------------------------------------

# Challenges of Legacy Systems

## 1. Maintenance Difficulty

Understanding old code is challenging.

Example:

    Millions of Lines of Code

            ↓

    Hard to Modify

------------------------------------------------------------------------

## 2. Security Risks

Older systems may have:

-   Unsupported software
-   Missing security updates

------------------------------------------------------------------------

## 3. Lack of Skilled Developers

Experts in old technologies are difficult to find.

------------------------------------------------------------------------

## 4. Integration Problems

Legacy systems may not easily connect with modern applications.

------------------------------------------------------------------------

## 5. High Maintenance Cost

Keeping old systems running can become expensive.

------------------------------------------------------------------------

# Legacy System Maintenance

Maintenance activities include:

-   Bug fixing
-   Security updates
-   Performance improvements
-   Integration updates
-   Documentation improvement

------------------------------------------------------------------------

# Legacy Modernization

**Legacy Modernization** is the process of improving or transforming old
systems using modern technologies.

Goal:

    Old System

          ↓

    Modern System

          ↓

    Better Performance

------------------------------------------------------------------------

# Legacy Modernization Strategies

## 1. Rehosting (Lift and Shift)

Moving the application to new infrastructure without major changes.

Example:

    Old Server

          ↓

    Cloud Server

------------------------------------------------------------------------

## 2. Replatforming

Moving to a new platform with small modifications.

Example:

    Old Database

          ↓

    Cloud Database

------------------------------------------------------------------------

## 3. Refactoring

Improving internal code structure without changing functionality.

Example:

    Complex Code

          ↓

    Clean Code

------------------------------------------------------------------------

## 4. Reengineering

Redesigning the system using modern architecture.

Example:

    Monolithic Application

          ↓

    Modern Services

------------------------------------------------------------------------

## 5. Replacement

Completely replacing the old system.

Example:

    Legacy Application

          ↓

    New Software

------------------------------------------------------------------------

# Legacy Migration Process

``` text
Analyze Existing System

        ↓

Plan Migration

        ↓

Choose Strategy

        ↓

Develop Solution

        ↓

Test

        ↓

Deploy

        ↓

Monitor
```

------------------------------------------------------------------------

# Legacy System vs Modern System

  Legacy System         Modern System
  --------------------- ---------------------
  Old technology        New technology
  Difficult changes     Easier updates
  Limited scalability   High scalability
  Manual processes      Automated processes

------------------------------------------------------------------------

# Real-World Example

## Banking System

Old system:

    Mainframe Application

    COBOL Code

    Traditional Database

Modernization:

    Cloud Infrastructure

    Modern APIs

    Updated Database

Benefits:

-   Better scalability
-   Improved security
-   Easier integration

------------------------------------------------------------------------

# Best Practices for Managing Legacy Systems

## 1. Understand Existing System

Document:

-   Architecture
-   Dependencies
-   Business logic

------------------------------------------------------------------------

## 2. Do Incremental Modernization

Avoid replacing everything at once.

------------------------------------------------------------------------

## 3. Maintain Automated Testing

Protect existing functionality.

------------------------------------------------------------------------

## 4. Improve Documentation

Preserve system knowledge.

------------------------------------------------------------------------

## 5. Monitor Security

Apply required updates.

------------------------------------------------------------------------

# Tools Used in Legacy Modernization

Common tools:

-   Cloud migration tools
-   API gateways
-   Containerization tools
-   Code analysis tools
-   Database migration tools

------------------------------------------------------------------------

# Interview Questions

## 1. What is a legacy system?

A legacy system is an old software system still used by an organization
despite outdated technology.

------------------------------------------------------------------------

## 2. Why do organizations keep legacy systems?

Because they contain important business logic and replacing them is
expensive and risky.

------------------------------------------------------------------------

## 3. What are challenges of legacy systems?

Challenges include:

-   High maintenance cost
-   Security risks
-   Poor documentation
-   Integration problems

------------------------------------------------------------------------

## 4. What is legacy modernization?

Legacy modernization transforms old systems into modern, maintainable
systems.

------------------------------------------------------------------------

## 5. Explain migration strategies.

Common strategies:

-   Rehosting
-   Replatforming
-   Refactoring
-   Reengineering
-   Replacement

------------------------------------------------------------------------

# Cheat Sheet

``` text
Legacy System

Old Technology

      ↓

Maintenance Challenges

      ↓

Modernization

      ↓

Improved System
```

------------------------------------------------------------------------

# Summary

Legacy systems are old but important software systems that organizations
continue to use. Maintaining them requires careful planning because they
often contain valuable business logic but face challenges such as
security risks, high maintenance costs, and limited scalability.

Legacy modernization helps organizations transform outdated systems into
reliable, scalable, and maintainable modern solutions.
