# Lesson 32 — SDLC Interview Questions

# Part 2 — Software Development Life Cycle (SDLC)

> **Objective**
>
> Revise the complete SDLC through interview-oriented questions, model answers, scenarios, and quick revision notes.

---

# Section 1 — Fundamental Questions

## Q1. What is SDLC?

**Answer**

The Software Development Life Cycle (SDLC) is a structured process used to plan, design, develop, test, deploy, and maintain software.

---

## Q2. Why is SDLC important?

It helps:

- Deliver quality software
- Reduce project risk
- Improve planning
- Control cost and schedule
- Improve communication
- Simplify maintenance

---

## Q3. List the phases of SDLC.

```text
Requirements
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
```

---

## Q4. Which SDLC phase is the most important?

There is no single correct answer.

A strong interview response:

> Every phase is important, but Requirement Gathering and Requirement Analysis have the greatest influence because mistakes made there become expensive to fix later.

---

## Q5. What are the major deliverables of each phase?

| Phase | Deliverable |
|--------|-------------|
| Requirements | BRD, User Stories |
| Analysis | Validated Requirements |
| SRS | Software Requirements Specification |
| Design | HLD, LLD, UML, API Design |
| Development | Source Code |
| Testing | Test Cases, Bug Reports |
| Deployment | Live Application |
| Maintenance | Updates & Patches |

---

# Section 2 — Requirement Engineering

## Q6. What is Requirement Gathering?

Collecting business and user needs from stakeholders.

---

## Q7. Name requirement gathering techniques.

- Interviews
- Questionnaires
- Workshops
- Brainstorming
- Observation
- Document Analysis
- Prototyping

---

## Q8. Requirement Gathering vs Requirement Analysis

| Gathering | Analysis |
|-----------|----------|
| Collect requirements | Validate & refine requirements |
| Focus on business needs | Focus on clarity and feasibility |

---

## Q9. What is a Functional Requirement?

A requirement describing **what the system should do.**

Example:

> User shall log in using email and password.

---

## Q10. What is a Non-Functional Requirement?

A requirement describing **how well the system should perform.**

Example:

> Login shall complete within 2 seconds.

---

## Q11. What is an SRS?

A formal document containing all agreed software requirements.

---

# Section 3 — Design & Development

## Q12. Difference between HLD and LLD.

| HLD | LLD |
|-----|-----|
| Overall architecture | Internal implementation |
| Modules | Classes, methods, algorithms |

---

## Q13. What happens during development?

- Coding
- Unit testing
- Code reviews
- Version control
- Build generation

---

## Q14. Why is version control important?

- Collaboration
- History
- Rollback
- Branching
- Safe integration

---

# Section 4 — Testing & Deployment

## Q15. Verification vs Validation

| Verification | Validation |
|--------------|------------|
| Building the product correctly | Building the right product |

---

## Q16. Name testing levels.

- Unit
- Integration
- System
- User Acceptance Testing (UAT)

---

## Q17. What is regression testing?

Re-testing existing functionality after changes to ensure nothing breaks.

---

## Q18. What is smoke testing?

A quick test after deployment to verify that critical features work.

---

## Q19. Name deployment environments.

```text
Development
      ↓
QA
      ↓
Staging
      ↓
Production
```

---

## Q20. Explain Blue-Green Deployment.

Two production environments exist.

Traffic switches from the old environment (Blue) to the new one (Green), allowing quick rollback if needed.

---

# Section 5 — Maintenance

## Q21. Why is maintenance the longest SDLC phase?

Software continues evolving through bug fixes, security updates, feature enhancements, and compatibility changes.

---

## Q22. Types of software maintenance.

- Corrective
- Adaptive
- Perfective
- Preventive

---

# Section 6 — SDLC Models

## Q23. What is an SDLC model?

A framework describing how SDLC phases are executed.

---

## Q24. Differentiate Waterfall and Agile.

| Waterfall | Agile |
|-----------|--------|
| Sequential | Iterative |
| Stable requirements | Changing requirements |
| Late testing | Continuous testing |

---

## Q25. Which model is suitable for high-risk projects?

**Answer:** Spiral Model.

---

## Q26. Which model is suitable for frequently changing requirements?

**Answer:** Agile.

---

# Section 7 — Scenario Questions

## Scenario 1

The customer changes requirements after development starts.

Expected Answer:

- Perform impact analysis
- Update requirements
- Re-estimate effort
- Inform stakeholders
- Follow change management

---

## Scenario 2

A release works in QA but fails in Production.

Possible reasons:

- Environment differences
- Configuration errors
- Missing dependencies
- Database mismatch

---

## Scenario 3

The application becomes slow after user growth.

Quality attributes affected:

- Performance
- Scalability

---

## Scenario 4

Users report crashes after a new release.

Expected process:

```text
Incident
   |
Investigate
   |
Fix
   |
Test
   |
Deploy Patch
```

---

# Rapid Fire

1. What is SDLC?
2. Why is SDLC needed?
3. List SDLC phases.
4. What is SRS?
5. Functional vs Non-Functional Requirements?
6. HLD vs LLD?
7. Verification vs Validation?
8. Smoke vs Regression Testing?
9. Four maintenance types?
10. Waterfall vs Agile?

---

# Interview Tips

- Begin with a definition.
- Explain the purpose.
- Use a real-world example.
- Draw simple diagrams.
- Mention benefits and limitations.

---

# SDLC Memory Map

```text
Business Idea
      ↓
Requirements
      ↓
Analysis
      ↓
SRS
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
      ↓
SDLC Models
```

---

# Summary

Part 2 interview questions focus on understanding the SDLC as an end-to-end process. Interviewers expect candidates to explain the purpose of each phase, identify the deliverables, differentiate similar concepts, and describe how software moves from an idea to a maintainable production system.
