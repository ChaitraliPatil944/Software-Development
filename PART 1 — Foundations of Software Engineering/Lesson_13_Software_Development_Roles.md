# Lesson 13 — Software Development Roles

# Part 1 — Foundations of Software Engineering

> **Objective**
>
> Understand the major roles in a software development team, their responsibilities, required skills, how they collaborate throughout the SDLC, and typical career paths.

---

# Introduction

Building modern software is a team effort.

A banking application, food delivery platform, or AI product cannot be built by one person alone.

Different specialists contribute at different stages of the Software Development Life Cycle (SDLC).

```text
Idea
 |
Business Analysis
 |
Design
 |
Development
 |
Testing
 |
Deployment
 |
Maintenance
```

Each stage involves different roles.

---

# Typical Software Team

```text
                    Customer
                        |
                 Product Owner
                        |
                Project Manager
                        |
                 Software Architect
                        |
 ---------------------------------------------------------
 |          |            |          |         |           |
Frontend  Backend    Database     QA      DevOps     UI/UX
Developer Developer Developer   Engineer  Engineer  Designer
```

---

# 1. Product Owner (PO)

## Purpose

Represents business needs and customer expectations.

## Responsibilities

- Defines product vision
- Prioritizes Product Backlog
- Accepts completed features
- Works closely with customers

## Skills

- Communication
- Business knowledge
- Prioritization
- Decision making

---

# 2. Business Analyst (BA)

## Purpose

Converts business ideas into technical requirements.

## Responsibilities

- Requirement gathering
- Requirement analysis
- Writing SRS
- User stories
- Process modeling

## Bridge

```text
Customer
    |
Business Analyst
    |
Development Team
```

---

# 3. Project Manager (PM)

## Purpose

Ensures the project is delivered on time, within budget, and with expected quality.

## Responsibilities

- Planning
- Scheduling
- Resource allocation
- Risk management
- Team coordination

Focus:

```text
Time
Cost
Scope
Quality
```

---

# 4. Software Architect

## Purpose

Designs the overall technical structure.

## Responsibilities

- High-Level Design
- Technology selection
- Scalability planning
- Security architecture
- Performance considerations

Analogy:

An architect designs the blueprint before construction begins.

---

# 5. Frontend Developer

Builds everything users interact with.

Examples:

- Login page
- Dashboard
- Buttons
- Forms
- Responsive layouts

Technologies:

- HTML
- CSS
- JavaScript
- React
- Angular
- Vue

---

# 6. Backend Developer

Develops business logic.

Responsibilities:

- APIs
- Authentication
- Payment processing
- Database interaction
- Business rules

Technologies:

- Java
- C#
- Python
- Node.js
- Go

---

# 7. Database Engineer / DBA

Responsible for data.

Tasks:

- Database design
- Query optimization
- Backups
- Security
- Performance tuning

---

# 8. UI/UX Designer

Creates intuitive user experiences.

Responsibilities:

- Wireframes
- Prototypes
- User research
- Accessibility
- Visual consistency

---

# 9. QA / Test Engineer

Ensures software quality.

Types of testing:

- Functional
- Regression
- Integration
- Performance
- Security
- Automation

Goal:

Deliver defect-free software.

---

# 10. DevOps Engineer

Connects development and operations.

Responsibilities:

- CI/CD pipelines
- Deployment automation
- Monitoring
- Infrastructure
- Cloud environments

Workflow:

```text
Code
 |
Build
 |
Test
 |
Deploy
 |
Monitor
```

---

# 11. Security Engineer

Protects applications and infrastructure.

Responsibilities:

- Vulnerability assessment
- Secure coding guidance
- Penetration testing
- Compliance

---

# 12. Site Reliability Engineer (SRE)

Focuses on system reliability after deployment.

Tasks:

- Monitoring
- Incident response
- Automation
- High availability

---

# Collaboration During SDLC

```text
Requirements
   |
BA + PO
   |
Design
   |
Architect + UI/UX
   |
Development
   |
Frontend + Backend + Database
   |
Testing
   |
QA
   |
Deployment
   |
DevOps
   |
Maintenance
   |
SRE + Developers
```

---

# Industry Example

Food Delivery Platform

- Product Owner: Prioritizes features
- BA: Documents requirements
- Architect: Designs system
- Frontend: Builds mobile/web UI
- Backend: Creates APIs
- DBA: Designs database
- QA: Tests ordering flow
- DevOps: Deploys updates
- SRE: Keeps production stable

---

# Career Progression

```text
Intern
   |
Junior Developer
   |
Software Engineer
   |
Senior Software Engineer
   |
Tech Lead
   |
Software Architect
```

Management path:

```text
Developer
   |
Team Lead
   |
Engineering Manager
   |
Director
   |
VP Engineering
   |
CTO
```

---

# Comparison

| Role | Primary Focus |
|------|---------------|
| Product Owner | Product vision |
| Business Analyst | Requirements |
| Project Manager | Planning |
| Architect | System design |
| Frontend Developer | User interface |
| Backend Developer | Business logic |
| DBA | Data |
| UI/UX Designer | User experience |
| QA Engineer | Quality |
| DevOps Engineer | Deployment |
| Security Engineer | Security |
| SRE | Reliability |

---

# Common Misconceptions

❌ Developers do everything.

✔ Large software projects require specialized roles.

❌ QA only tests.

✔ QA improves software quality throughout development.

❌ DevOps replaces developers.

✔ DevOps enables faster and more reliable delivery.

---

# Interview Questions

1. What is the role of a Software Architect?
2. Differentiate Product Owner and Project Manager.
3. What does a Business Analyst do?
4. Explain the responsibilities of a DevOps Engineer.
5. What is the difference between Frontend and Backend development?
6. Who is responsible for software quality?

---

# Cheat Sheet

```text
PO      → Product Vision
BA      → Requirements
PM      → Planning
Architect → Design
Frontend → UI
Backend  → Logic
DBA      → Data
QA       → Testing
DevOps   → Deployment
SRE      → Reliability
Security → Protection
```

---

# Summary

Modern software development relies on specialized roles working together across the SDLC. Each role contributes unique expertise, from understanding business needs to designing architecture, writing code, testing quality, deploying applications, and maintaining production systems. Successful software projects depend on collaboration, communication, and clearly defined responsibilities.
