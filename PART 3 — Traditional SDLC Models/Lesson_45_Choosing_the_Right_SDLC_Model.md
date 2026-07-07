# Lesson 45 — Choosing the Right SDLC Model

# Part 3 — Traditional SDLC Models

> **Objective**
>
> Learn how software architects, project managers, and engineering teams choose the most appropriate SDLC model based on project characteristics rather than personal preference.

---

# Introduction

A common interview question is:

> "Which SDLC model is the best?"

The correct answer is:

> **There is no universally best SDLC model. The best model depends on the project.**

Choosing the wrong model can increase cost, delay delivery, and reduce software quality.

---

# Decision Factors

Before selecting a model, evaluate:

- Requirement stability
- Project size
- Risk level
- Budget
- Timeline
- Customer involvement
- Regulatory requirements
- Team experience
- Technology maturity

```text
Project
   |
Analyze Factors
   |
Select SDLC Model
```

---

# 1. Requirement Stability

| Situation | Recommended Model |
|-----------|-------------------|
| Stable requirements | Waterfall, V-Model |
| Frequently changing | Iterative, Prototype |
| Partially changing | Incremental, RAD |

---

# 2. Project Size

| Project Size | Suitable Models |
|--------------|-----------------|
| Small | RAD, Prototype, Big Bang |
| Medium | Incremental, Iterative |
| Large | Waterfall, Spiral, CBD |

---

# 3. Risk Level

```text
Low Risk  → Waterfall
Medium    → Incremental
High      → Spiral
Critical  → V-Model + Spiral
```

---

# 4. Timeline

| Delivery Need | Suitable Models |
|---------------|-----------------|
| Very fast | RAD |
| Fast | Incremental |
| Moderate | Iterative |
| Long-term | Waterfall |

---

# 5. Customer Participation

| Customer Availability | Model |
|------------------------|-------|
| Low | Waterfall |
| Moderate | Incremental |
| High | Iterative, Prototype, RAD |

---

# 6. Compliance

Industries such as banking, healthcare, aerospace, and government usually require:

- Extensive documentation
- Reviews
- Traceability
- Formal approvals

Recommended:

- Waterfall
- V-Model

---

# 7. Team Experience

Experienced teams can successfully manage:

- Spiral
- CBD
- RAD

Newer teams often benefit from:

- Waterfall
- Incremental

---

# Selection Workflow

```text
Requirements Stable?
        |
     Yes ----------- No
      |              |
Compliance?     Customer Feedback?
      |              |
Waterfall/V     Yes -------- No
                    |         |
            Prototype   Incremental
                    |
              High Risk?
                    |
                 Spiral
```

---

# Industry Examples

## Government Tax Portal

- Stable laws
- Heavy documentation
- Formal approvals

**Model:** Waterfall

---

## Medical Device Software

- Patient safety
- Regulatory testing
- Traceability

**Model:** V-Model

---

## Startup SaaS Platform

- Weekly feature updates
- Rapid feedback
- Market uncertainty

**Model:** Iterative or RAD

---

## AI Research Project

- Experimental
- Unknown outcomes

**Model:** Prototype or Big Bang

---

## Enterprise ERP

- Many reusable modules
- Long-term maintenance

**Model:** Component-Based Development

---

# Comparison Matrix

| Project Characteristic | Best Choice |
|-------------------------|-------------|
| Stable requirements | Waterfall |
| Safety critical | V-Model |
| Feature-by-feature delivery | Incremental |
| Continuous improvement | Iterative |
| High risk | Spiral |
| Fast delivery | RAD |
| Unclear requirements | Prototype |
| Research | Big Bang |
| Reusable architecture | CBD |

---

# Common Mistakes

❌ Choosing a model because it is popular.

✔ Choose based on project needs.

❌ Ignoring customer involvement.

✔ Match the process to stakeholder availability.

❌ Ignoring compliance requirements.

✔ Consider regulations before selecting a model.

---

# Interview Questions

1. Is there a universally best SDLC model?
2. Which factors influence SDLC model selection?
3. Which model suits a startup?
4. Which model suits banking software?
5. Why is Spiral preferred for high-risk projects?
6. Which model is best for unclear requirements?

---

# Cheat Sheet

```text
Stable Requirements  → Waterfall
Critical Systems     → V-Model
Feature Releases     → Incremental
Continuous Improvement → Iterative
High Risk            → Spiral
Fast Delivery        → RAD
Unclear Requirements → Prototype
Research             → Big Bang
Reuse                → CBD
```

---

# Summary

Selecting an SDLC model is an engineering decision based on project context. Requirement stability, risk, compliance, customer involvement, delivery timelines, and team capability all influence the choice. Successful organizations adapt the development process to the problem they are solving instead of forcing every project into the same methodology.
