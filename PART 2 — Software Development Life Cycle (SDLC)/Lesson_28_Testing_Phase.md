# Lesson 28 — Testing Phase

# Part 2 — Software Development Life Cycle (SDLC)

> **Objective**
>
> Understand the role of the Testing Phase in the SDLC, how QA teams verify software quality, and how testing ensures software is ready for deployment.

---

# Introduction

Writing code is only half the job.

Before software reaches users, teams must answer one question:

> **Does the software work correctly, safely, and reliably?**

The Testing Phase answers that question.

```text
Development
     |
Testing
     |
Reliable Software
```

---

# What is the Testing Phase?

The **Testing Phase** verifies and validates that the developed software meets the requirements defined in the SRS.

Its purpose is to identify defects before deployment.

---

# Why is Testing Important?

Without testing:

```text
Code
 |
Production
 |
Users Find Bugs
 |
Loss of Trust
```

With testing:

```text
Code
 |
QA Testing
 |
Bugs Fixed
 |
Stable Release
```

---

# Objectives

- Verify functionality
- Validate business requirements
- Find defects early
- Improve reliability
- Reduce production failures
- Ensure customer satisfaction

---

# Testing Workflow

```text
Development Complete
        |
Test Planning
        |
Test Case Design
        |
Execute Tests
        |
Bug Found?
   /        \
 Yes        No
 |           |
Report Bug  Ready for Release
 |
Developer Fix
 |
Retest
 |
Regression Testing
 |
Deployment
```

---

# Verification vs Validation

| Verification | Validation |
|--------------|------------|
| Are we building the product correctly? | Are we building the right product? |
| Reviews, inspections | Executing the software |
| Prevents defects | Detects defects |

---

# Levels of Testing

## Unit Testing

Tests individual functions or classes.

Performed mainly by developers.

---

## Integration Testing

Checks interaction between modules.

Example:

```text
Login
  |
Database
```

---

## System Testing

Tests the complete application as one system.

---

## User Acceptance Testing (UAT)

Performed by customers or business users to confirm the software satisfies business needs.

---

# Common Testing Types

- Functional Testing
- Regression Testing
- Smoke Testing
- Sanity Testing
- Performance Testing
- Security Testing
- Usability Testing
- Compatibility Testing

> Detailed testing concepts will be covered in the dedicated **Software Testing Handbook**.

---

# Defect Lifecycle

```text
Bug Found
    |
Reported
    |
Assigned
    |
Fixed
    |
Retested
    |
Closed
```

If the issue remains, it is reopened.

---

# Test Case

Example:

Requirement:

> User Login

Test Case:

- Enter valid username
- Enter valid password
- Click Login
- Expected Result: Dashboard opens

---

# Stakeholders

```text
QA Engineer
     |
Developer
     |
Business Analyst
     |
Product Owner
```

---

# Deliverables

- Test Plan
- Test Cases
- Bug Reports
- Test Summary Report
- Release Recommendation

---

# Industry Example

## Online Banking

QA verifies:

- Login
- Money Transfer
- Balance Inquiry
- Session Timeout
- Security
- Performance

Only after successful testing is the application approved for deployment.

---

# Common Challenges

- Changing requirements
- Tight deadlines
- Incomplete test data
- Environment differences
- Missed edge cases

---

# Best Practices

- Test early
- Automate repetitive tests where appropriate
- Maintain traceability between requirements and tests
- Re-test after bug fixes
- Document defects clearly

---

# Common Mistakes

❌ Assuming developers don't make mistakes.

✔ Every change should be tested.

❌ Skipping regression testing.

✔ Ensure existing features still work.

❌ Treating testing as the final step only.

✔ Quality should be considered throughout the SDLC.

---

# Inputs & Outputs

| Input | Output |
|-------|--------|
| Source Code | Bug Reports |
| SRS | Test Cases |
| Design Documents | Test Summary |
| Build | Release Recommendation |

---

# Interview Questions

1. What is the Testing Phase?
2. Why is testing important?
3. Differentiate verification and validation.
4. Name the levels of testing.
5. What is regression testing?
6. What is a test case?
7. What are the deliverables of testing?

---

# Cheat Sheet

```text
Development
     ↓
Testing
     ↓
Bug Fix
     ↓
Retest
     ↓
Regression
     ↓
Deployment

Outputs

✓ Test Plan
✓ Test Cases
✓ Bug Reports
✓ Test Summary
```

---

# Summary

The Testing Phase ensures that software satisfies both functional and quality requirements before release. Through structured planning, test execution, defect reporting, and regression testing, QA teams help deliver reliable software with fewer production issues. Testing is a critical quality gate in the SDLC, not merely a final checkpoint before deployment.
