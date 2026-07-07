# Lesson 186 --- Preventive Maintenance

# Part 12 --- Software Maintenance

> **Objective**
>
> Understand Preventive Maintenance, why prevention is important, code
> improvement activities, dependency updates, security improvements,
> preventive maintenance process, challenges, best practices, and its
> role in long-term software reliability.

------------------------------------------------------------------------

# Introduction

Software problems are not always fixed after they occur.

Good engineering teams prevent problems before they appear.

Preventive Maintenance focuses on improving software internally to
reduce future risks.

``` text
Current Software

      ↓

Identify Future Risks

      ↓

Improve System

      ↓

Prevent Problems
```

------------------------------------------------------------------------

# What is Preventive Maintenance?

**Preventive Maintenance** is the process of modifying software to
prevent future failures, improve maintainability, and reduce long-term
maintenance effort.

Simple definition:

    Preventive Maintenance = Prevent Future Problems

------------------------------------------------------------------------

# Why is Preventive Maintenance Needed?

Software quality decreases over time because of:

-   Increasing complexity
-   Outdated dependencies
-   Poor code structure
-   Security vulnerabilities
-   Lack of documentation

Without preventive maintenance:

    Software Growth

          ↓

    Complexity Increase

          ↓

    Future Failures

------------------------------------------------------------------------

# Examples of Preventive Maintenance

## Example 1 --- Code Refactoring

Before:

    Complex Unreadable Code

After:

    Clean Modular Code

------------------------------------------------------------------------

## Example 2 --- Dependency Updates

Old:

    Library Version 1.0

Updated:

    Library Version 2.0

Benefits:

-   Security fixes
-   Better performance
-   Compatibility

------------------------------------------------------------------------

## Example 3 --- Security Improvements

Activities:

-   Security patches
-   Vulnerability fixes
-   Access control improvements

------------------------------------------------------------------------

## Example 4 --- Documentation Updates

Maintaining:

-   Architecture documents
-   API documentation
-   User guides

------------------------------------------------------------------------

# Preventive Maintenance Process

``` text
Identify Future Risks

        ↓

Analyze System

        ↓

Plan Improvements

        ↓

Modify Software

        ↓

Test Changes

        ↓

Deploy Update

        ↓

Monitor
```

------------------------------------------------------------------------

# Step 1 --- Identify Risks

Sources:

-   Code reviews
-   Security scans
-   Performance analysis
-   Technical debt analysis

Example:

    Outdated Dependency Found

------------------------------------------------------------------------

# Step 2 --- Analyze Impact

Teams evaluate:

-   Affected components
-   Required effort
-   Possible risks

------------------------------------------------------------------------

# Step 3 --- Implement Improvements

Changes may include:

-   Refactoring code
-   Updating libraries
-   Improving architecture
-   Removing unused components

------------------------------------------------------------------------

# Step 4 --- Testing

Testing ensures improvements do not break existing features.

Includes:

-   Unit testing
-   Integration testing
-   Regression testing

------------------------------------------------------------------------

# Areas of Preventive Maintenance

## 1. Code Quality Improvement

Activities:

-   Remove duplicate code
-   Improve structure
-   Follow coding standards

------------------------------------------------------------------------

## 2. Security Enhancement

Activities:

-   Apply patches
-   Fix vulnerabilities
-   Improve authentication

------------------------------------------------------------------------

## 3. Dependency Management

Activities:

-   Update libraries
-   Remove outdated packages
-   Check compatibility

------------------------------------------------------------------------

## 4. Architecture Improvement

Activities:

-   Improve design
-   Reduce complexity
-   Increase scalability

------------------------------------------------------------------------

## 5. Documentation Improvement

Activities:

-   Update technical documents
-   Maintain system knowledge

------------------------------------------------------------------------

# Preventive Maintenance vs Corrective Maintenance

  Preventive               Corrective
  ------------------------ -----------------------
  Prevents future issues   Fixes existing issues
  Proactive approach       Reactive approach
  Done before failure      Done after failure

------------------------------------------------------------------------

# Preventive Maintenance vs Perfective Maintenance

  Preventive                   Perfective
  ---------------------------- -------------------------
  Focuses on future problems   Focuses on improvements
  Reduces risks                Enhances features

------------------------------------------------------------------------

# Challenges in Preventive Maintenance

## 1. Business Priority

Preventive work may not provide immediate visible benefits.

------------------------------------------------------------------------

## 2. Resource Allocation

Teams must dedicate time for improvement.

------------------------------------------------------------------------

## 3. Risk of Changes

Internal improvements can introduce bugs.

------------------------------------------------------------------------

## 4. Measuring Benefits

Preventing failures is difficult to measure.

------------------------------------------------------------------------

# Best Practices

## 1. Perform Regular Code Reviews

Find problems early.

------------------------------------------------------------------------

## 2. Keep Dependencies Updated

Reduce security risks.

------------------------------------------------------------------------

## 3. Automate Testing

Ensure safe changes.

------------------------------------------------------------------------

## 4. Monitor System Health

Identify warning signs.

------------------------------------------------------------------------

## 5. Maintain Technical Documentation

Preserve system knowledge.

------------------------------------------------------------------------

# Preventive Maintenance in SDLC

``` text
Development

      ↓

Deployment

      ↓

Monitoring

      ↓

Risk Identification

      ↓

Preventive Maintenance

      ↓

Reliable Software
```

------------------------------------------------------------------------

# Real-World Example

## Banking Application

Problem prediction:

    Database Performance May Decrease

Preventive actions:

    Optimize Queries

    Update Database Version

    Improve Indexing

    Monitor Performance

Result:

    Reduced Future Failures

------------------------------------------------------------------------

# Tools Used

Common tools:

-   SonarQube
-   Git
-   Static analysis tools
-   Security scanners
-   Dependency management tools

------------------------------------------------------------------------

# Interview Questions

## 1. What is Preventive Maintenance?

Preventive Maintenance modifies software to prevent future problems and
improve reliability.

------------------------------------------------------------------------

## 2. Why is preventive maintenance important?

It reduces future failures, improves maintainability, and extends
software life.

------------------------------------------------------------------------

## 3. Give examples of preventive maintenance.

Examples:

-   Refactoring code
-   Updating dependencies
-   Security improvements
-   Documentation updates

------------------------------------------------------------------------

## 4. Difference between preventive and corrective maintenance?

Preventive avoids future problems.

Corrective fixes existing problems.

------------------------------------------------------------------------

## 5. How does preventive maintenance improve software quality?

It reduces complexity, improves security, and makes future changes
easier.

------------------------------------------------------------------------

# Cheat Sheet

``` text
Preventive Maintenance

Find Risks

    ↓

Improve System

    ↓

Reduce Future Failures

    ↓

Reliable Software
```

------------------------------------------------------------------------

# Summary

Preventive Maintenance focuses on preventing future software problems
through code improvement, dependency updates, security enhancements, and
better documentation. It helps organizations reduce maintenance costs,
improve reliability, and extend the life of software systems.

Strong software teams do not only fix problems; they continuously
improve systems before problems occur.
