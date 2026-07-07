# Lesson 29 — Deployment Phase

# Part 2 — Software Development Life Cycle (SDLC)

> **Objective**
>
> Understand how software is released to users, what happens during deployment, the environments involved, deployment strategies, and how organizations minimize risk during software releases.

---

# Introduction

Building and testing software is not the end of the SDLC.

The software must now reach real users safely.

This process is called the **Deployment Phase**.

```text
Development
      |
Testing
      |
Deployment
      |
Users
```

---

# What is Deployment?

Deployment is the process of moving tested software from a controlled environment into a live environment where end users can use it.

Deployment includes:

- Installing the application
- Configuring environments
- Connecting databases
- Verifying services
- Monitoring the release

---

# Why is Deployment Important?

Poor deployment can cause:

- Downtime
- Data loss
- Failed releases
- Customer complaints
- Revenue loss

A well-planned deployment reduces these risks.

---

# SDLC Deployment Workflow

```text
Development
      |
Testing
      |
Release Approval
      |
Deploy
      |
Smoke Test
      |
Monitoring
      |
Users
```

---

# Deployment Environments

```text
Developer Machine
        |
Development
        |
QA / Test
        |
Staging (Production-like)
        |
Production
```

## Development

Used by developers to build features.

## QA/Test

Used for functional and regression testing.

## Staging

A production-like environment for final validation.

## Production

The live environment used by customers.

---

# Activities During Deployment

- Prepare release package
- Backup databases
- Configure servers
- Deploy application
- Verify services
- Execute smoke tests
- Monitor logs
- Inform stakeholders

---

# Deployment Strategies

## 1. Recreate

```text
Old Version
    |
Stop
    |
Deploy New Version
```

Simple but causes downtime.

---

## 2. Rolling Deployment

```text
Server 1 → Update
Server 2 → Update
Server 3 → Update
```

Updates servers gradually.

---

## 3. Blue-Green Deployment

```text
Blue (Current)
        |
Switch Traffic
        |
Green (New)
```

Fast rollback with minimal downtime.

---

## 4. Canary Deployment

```text
5% Users
   |
25%
   |
50%
   |
100%
```

Release to a small group first, then expand if healthy.

---

# Rollback

If problems occur:

```text
New Release
     |
Issue Detected
     |
Rollback
     |
Previous Stable Version
```

Rollback minimizes customer impact.

---

# Smoke Testing

Performed immediately after deployment.

Purpose:

- Verify critical functionality
- Confirm application starts correctly
- Ensure deployment succeeded

---

# Monitoring

After deployment teams monitor:

- CPU
- Memory
- Errors
- Response time
- User traffic
- Logs

Monitoring helps detect production issues quickly.

---

# Stakeholders

```text
Developers
     |
QA
     |
DevOps
     |
Operations
     |
Product Owner
```

---

# Deliverables

- Live Application
- Deployment Report
- Release Notes
- Monitoring Dashboard
- Rollback Plan

---

# Industry Example

## E-Commerce Website

Release Day:

- Deploy new checkout feature
- Run smoke tests
- Monitor payment failures
- Watch server health
- Roll back immediately if major issues appear

---

# Best Practices

- Deploy during low-traffic periods
- Automate deployments where possible
- Always keep backups
- Maintain a rollback plan
- Validate in staging first
- Monitor continuously after release

---

# Common Mistakes

❌ Deploying without backups.

✔ Create backups before deployment.

❌ Deploying directly from developer machines.

✔ Use controlled release pipelines.

❌ Ignoring monitoring.

✔ Watch production metrics after every release.

---

# Inputs & Outputs

| Input | Output |
|-------|--------|
| Tested Build | Live Application |
| Release Candidate | Release Notes |
| Deployment Plan | Deployment Report |
| Configuration Files | Running Services |

---

# Interview Questions

1. What is the Deployment Phase?
2. Why is a staging environment important?
3. Explain Blue-Green Deployment.
4. What is Canary Deployment?
5. Why is rollback necessary?
6. What is smoke testing?
7. What happens after deployment?

---

# Cheat Sheet

```text
Testing
   ↓
Release Approval
   ↓
Deployment
   ↓
Smoke Test
   ↓
Monitoring
   ↓
Users

Strategies

✓ Recreate
✓ Rolling
✓ Blue-Green
✓ Canary

Outputs

✓ Live Application
✓ Release Notes
✓ Rollback Plan
```

---

# Summary

The Deployment Phase delivers tested software to end users in a controlled and reliable manner. By using deployment environments, release strategies, smoke testing, monitoring, and rollback plans, organizations minimize deployment risk and ensure stable software reaches production. Modern deployments are closely supported by DevOps practices, which will be explored in depth later in this handbook.
