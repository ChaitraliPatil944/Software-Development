# Lesson 194 --- Software Maintenance Interview Questions

# Part 12 --- Software Maintenance

> **Objective**
>
> Prepare for software maintenance interviews by understanding questions
> related to maintenance concepts, maintenance types, legacy systems,
> technical debt, refactoring, documentation, change management,
> versioning, release management, and real-world scenarios.

------------------------------------------------------------------------

# Section 1 --- Software Maintenance Fundamentals

## Q1. What is Software Maintenance?

**Answer:**

Software Maintenance is the process of modifying, updating, improving,
and managing software after deployment.

It includes:

-   Bug fixing
-   Feature enhancement
-   Performance improvement
-   Security updates
-   Environment adaptation

------------------------------------------------------------------------

## Q2. Why is software maintenance important?

Software maintenance helps:

-   Fix defects
-   Improve reliability
-   Adapt to changes
-   Enhance user experience
-   Extend software life

------------------------------------------------------------------------

## Q3. Is maintenance part of SDLC?

Yes.

Software maintenance is the final and longest phase of the Software
Development Life Cycle.

    Requirement

    ↓

    Design

    ↓

    Development

    ↓

    Testing

    ↓

    Deployment

    ↓

    Maintenance

------------------------------------------------------------------------

# Section 2 --- Types of Software Maintenance

## Q4. What are the four types of software maintenance?

The four types are:

1.  Corrective Maintenance
2.  Adaptive Maintenance
3.  Perfective Maintenance
4.  Preventive Maintenance

------------------------------------------------------------------------

## Q5. Explain Corrective Maintenance.

Corrective Maintenance fixes defects discovered after software
deployment.

Examples:

-   Bug fixes
-   Application crashes
-   Calculation errors

------------------------------------------------------------------------

## Q6. Explain Adaptive Maintenance.

Adaptive Maintenance modifies software to work in new environments.

Examples:

-   OS upgrades
-   Database migration
-   Cloud migration

------------------------------------------------------------------------

## Q7. Explain Perfective Maintenance.

Perfective Maintenance improves existing software features, performance,
and usability.

Examples:

-   UI improvements
-   Performance optimization
-   New features

------------------------------------------------------------------------

## Q8. Explain Preventive Maintenance.

Preventive Maintenance prevents future problems.

Examples:

-   Refactoring
-   Dependency updates
-   Security improvements

------------------------------------------------------------------------

# Section 3 --- Maintenance Comparison Questions

## Q9. Difference between Corrective and Preventive Maintenance?

  Corrective              Preventive
  ----------------------- ------------------------
  Fixes existing issues   Prevents future issues
  Reactive                Proactive
  After failure           Before failure

------------------------------------------------------------------------

## Q10. Difference between Adaptive and Perfective Maintenance?

  Adaptive                      Perfective
  ----------------------------- --------------------------
  Handles environment changes   Improves features
  Compatibility focused         User improvement focused

------------------------------------------------------------------------

# Section 4 --- Legacy Systems

## Q11. What is a Legacy System?

A legacy system is an old software system still used by an organization
despite outdated technology.

------------------------------------------------------------------------

## Q12. Why do organizations keep legacy systems?

Reasons:

-   Important business logic
-   High replacement cost
-   Migration risks
-   Business dependency

------------------------------------------------------------------------

## Q13. What are challenges of legacy systems?

Challenges:

-   Security risks
-   High maintenance cost
-   Poor documentation
-   Difficult integration
-   Limited scalability

------------------------------------------------------------------------

## Q14. What is legacy modernization?

Legacy modernization transforms old systems into modern maintainable
systems.

Strategies:

-   Rehosting
-   Replatforming
-   Refactoring
-   Reengineering
-   Replacement

------------------------------------------------------------------------

# Section 5 --- Technical Debt

## Q15. What is Technical Debt?

Technical debt is the future maintenance cost created by choosing quick
solutions instead of better long-term solutions.

------------------------------------------------------------------------

## Q16. Why does technical debt occur?

Reasons:

-   Tight deadlines
-   Poor design
-   Lack of testing
-   Outdated technologies

------------------------------------------------------------------------

## Q17. How can technical debt be reduced?

Methods:

-   Refactoring
-   Automated testing
-   Documentation
-   Dependency updates
-   Architecture improvements

------------------------------------------------------------------------

# Section 6 --- Refactoring

## Q18. What is Refactoring?

Refactoring improves the internal structure of code without changing its
external behavior.

------------------------------------------------------------------------

## Q19. Why is refactoring important?

Benefits:

-   Better readability
-   Easier maintenance
-   Reduced technical debt
-   Improved code quality

------------------------------------------------------------------------

## Q20. Difference between refactoring and rewriting?

  Refactoring              Rewriting
  ------------------------ ---------------------
  Improves existing code   Creates new system
  Lower risk               Higher risk
  Keeps behavior           May change behavior

------------------------------------------------------------------------

## Q21. What are code smells?

Code smells are indicators of poor code design.

Examples:

-   Duplicate code
-   Long methods
-   Large classes
-   Complex logic

------------------------------------------------------------------------

# Section 7 --- Documentation

## Q22. Why is software documentation important?

Documentation helps:

-   Knowledge sharing
-   Maintenance
-   Troubleshooting
-   Team collaboration

------------------------------------------------------------------------

## Q23. Types of software documentation?

Examples:

-   Technical documentation
-   User documentation
-   API documentation
-   Process documentation

------------------------------------------------------------------------

## Q24. Why should documentation be maintained?

Because software changes continuously and outdated documentation becomes
unreliable.

------------------------------------------------------------------------

# Section 8 --- Change Management

## Q25. What is Change Management?

Change Management controls software modifications through planning,
approval, implementation, and tracking.

------------------------------------------------------------------------

## Q26. Explain Change Management process.

    Request

    ↓

    Impact Analysis

    ↓

    Approval

    ↓

    Implementation

    ↓

    Testing

    ↓

    Deployment

------------------------------------------------------------------------

## Q27. What is Change Control Board (CCB)?

CCB is a group responsible for reviewing and approving important
changes.

------------------------------------------------------------------------

# Section 9 --- Versioning

## Q28. What is Software Versioning?

Software versioning assigns identifiers to different software releases.

------------------------------------------------------------------------

## Q29. Explain Semantic Versioning.

Format:

    MAJOR.MINOR.PATCH

Example:

    2.5.1

------------------------------------------------------------------------

## Q30. Difference between major, minor, and patch versions?

Major:

-   Breaking changes

Minor:

-   New features

Patch:

-   Bug fixes

------------------------------------------------------------------------

# Section 10 --- Release Management

## Q31. What is Release Management?

Release Management plans, coordinates, tests, and delivers software
releases.

------------------------------------------------------------------------

## Q32. Explain release lifecycle.

    Planning

    ↓

    Development

    ↓

    Testing

    ↓

    Approval

    ↓

    Deployment

    ↓

    Monitoring

------------------------------------------------------------------------

## Q33. What are release strategies?

Examples:

-   Rolling release
-   Blue-Green deployment
-   Canary release
-   Big Bang release

------------------------------------------------------------------------

## Q34. What is rollback?

Rollback restores the previous stable version after a failed release.

------------------------------------------------------------------------

# Section 11 --- Scenario-Based Questions

## Q35. A production bug is found. What will you do?

Answer:

1.  Create incident
2.  Analyze logs
3.  Identify root cause
4.  Fix issue
5.  Test solution
6.  Deploy update
7.  Perform RCA

------------------------------------------------------------------------

## Q36. Users request a new feature. Which maintenance type is used?

Answer:

Perfective Maintenance.

------------------------------------------------------------------------

## Q37. Database version changes. Which maintenance type is required?

Answer:

Adaptive Maintenance.

------------------------------------------------------------------------

## Q38. Code quality is poor. What activity should be performed?

Answer:

Refactoring and Preventive Maintenance.

------------------------------------------------------------------------

# Quick Revision Table

  Topic                Key Point
  -------------------- ------------------------------------
  Maintenance          Improves software after deployment
  Corrective           Fixes bugs
  Adaptive             Handles environment changes
  Perfective           Improves features
  Preventive           Prevents future issues
  Legacy System        Old but important software
  Technical Debt       Future cost of shortcuts
  Refactoring          Improves code structure
  Documentation        Preserves knowledge
  Change Management    Controls modifications
  Versioning           Tracks releases
  Release Management   Controls software delivery

------------------------------------------------------------------------

# Interview Tips

For maintenance questions:

1.  Define the concept
2.  Explain why it is needed
3.  Give an example
4.  Mention best practices

------------------------------------------------------------------------

# Summary

Software maintenance interviews focus on understanding how software
evolves after deployment. Candidates should understand maintenance
types, system modernization, code quality improvement, change control,
and release processes.

A good software engineer does not only build systems; they maintain and
improve them throughout their lifecycle.
