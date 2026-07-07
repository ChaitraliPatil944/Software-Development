# Lesson 30 — Maintenance Phase

# Part 2 — Software Development Life Cycle (SDLC)

> **Objective**
>
> Understand why the Maintenance Phase is the longest stage of the SDLC, the different types of maintenance, and how software continues to evolve after deployment.

---

# Introduction

Many people think software development ends after deployment.

In reality, deployment is often the beginning.

After users start using the software:

- Bugs are discovered
- New features are requested
- Security vulnerabilities appear
- Business rules change
- Operating systems evolve

The software must continuously adapt.

This ongoing work is called the **Maintenance Phase**.

---

# What is the Maintenance Phase?

The **Maintenance Phase** is the SDLC stage where software is monitored, supported, repaired, improved, and updated after it has been deployed to production.

```text
Deployment
     |
Users
     |
Feedback
     |
Maintenance
     |
Improved Software
```

---

# Why is Maintenance Important?

Without maintenance:

```text
Software Released
      |
Bugs Remain
      |
Security Issues
      |
Poor Performance
      |
Users Leave
```

With maintenance:

```text
Release
   |
Monitor
   |
Fix
   |
Improve
   |
Update
```

Software remains useful for years.

---

# Goals

- Fix production defects
- Improve performance
- Enhance security
- Add features
- Adapt to changing business needs
- Keep software compatible

---

# Maintenance Workflow

```text
Users
   |
Feedback / Incidents
   |
Analysis
   |
Bug Fix / Enhancement
   |
Testing
   |
Deployment
   |
Updated Version
```

---

# Types of Software Maintenance

## 1. Corrective Maintenance

Fixes defects discovered after release.

Examples:

- Login bug
- Payment failure
- Crash during checkout

---

## 2. Adaptive Maintenance

Keeps software compatible with changing environments.

Examples:

- New operating system
- Database upgrade
- Cloud migration
- API version changes

---

## 3. Perfective Maintenance

Improves existing functionality.

Examples:

- Faster search
- Better UI
- New dashboard
- Additional reports

---

## 4. Preventive Maintenance

Reduces future risks.

Examples:

- Refactoring
- Updating dependencies
- Improving documentation
- Code cleanup

---

# Visual Summary

```text
Maintenance

├── Corrective
├── Adaptive
├── Perfective
└── Preventive
```

---

# Industry Example

## Online Banking

Corrective:
- Fix failed transaction issue

Adaptive:
- Support latest mobile OS

Perfective:
- Add QR payments

Preventive:
- Upgrade encryption library

---

# Incident Management

Production issue:

```text
Issue Reported
      |
Priority Assigned
      |
Investigation
      |
Fix
      |
Testing
      |
Deployment
      |
Incident Closed
```

---

# Change Requests

Users request:

- New features
- UI improvements
- Business rule changes

These requests are analyzed before implementation.

---

# Versioning

Software evolves through releases.

```text
Version 1.0
      |
Version 1.1
      |
Version 1.2
      |
Version 2.0
```

Each release includes bug fixes or enhancements.

---

# Stakeholders

```text
Users
   |
Support Team
   |
Business Analyst
   |
Developers
   |
QA
   |
DevOps
   |
Product Owner
```

---

# Deliverables

- Bug Fixes
- Security Patches
- Feature Enhancements
- Updated Documentation
- New Software Versions
- Release Notes

---

# Best Practices

- Monitor production continuously
- Prioritize critical incidents
- Maintain documentation
- Automate repetitive maintenance tasks
- Review technical debt regularly

---

# Common Challenges

- Legacy code
- Poor documentation
- Technical debt
- Frequent requirement changes
- Tight maintenance windows

---

# Common Mistakes

❌ Ignoring customer feedback.

✔ Feedback drives product improvement.

❌ Delaying security updates.

✔ Patch vulnerabilities quickly.

❌ Making production fixes without testing.

✔ Test every maintenance change.

---

# Inputs & Outputs

| Input | Output |
|-------|--------|
| User Feedback | Bug Fixes |
| Incident Reports | Updated Releases |
| Change Requests | New Features |
| Monitoring Data | Performance Improvements |

---

# Interview Questions

1. What is the Maintenance Phase?
2. Why is maintenance considered the longest SDLC phase?
3. Explain the four types of software maintenance.
4. Differentiate corrective and preventive maintenance.
5. What is adaptive maintenance?
6. Why is production monitoring important?
7. What is a change request?

---

# Cheat Sheet

```text
Maintenance

Release
   ↓
Monitor
   ↓
Feedback
   ↓
Fix / Improve
   ↓
Test
   ↓
Deploy

Types

✓ Corrective
✓ Adaptive
✓ Perfective
✓ Preventive
```

---

# Summary

The Maintenance Phase keeps software valuable long after its initial release. Through corrective, adaptive, perfective, and preventive maintenance, engineering teams fix defects, improve performance, strengthen security, and deliver new capabilities. Continuous maintenance ensures software remains reliable, relevant, and aligned with changing business and user needs throughout its lifecycle.
