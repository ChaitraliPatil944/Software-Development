# Lesson 44 — SDLC Model Comparison

# Part 3 — Traditional SDLC Models

> **Objective**
>
> Compare all major traditional SDLC models, understand their strengths and weaknesses, and learn how to select the most suitable model for different projects.

---

# Why Compare SDLC Models?

Every project is different.

Different projects have different:

- Requirements
- Risks
- Budgets
- Team sizes
- Timelines
- Compliance needs

There is **no universal best model**.

```text
Project Characteristics
          |
Choose Appropriate SDLC Model
          |
Higher Success Probability
```

---

# Models Covered

```text
✓ Waterfall
✓ V-Model
✓ Incremental
✓ Iterative
✓ Spiral
✓ RAD
✓ Prototype
✓ Big Bang
✓ Component-Based Development (CBD)
```

---

# High-Level Comparison

| Model | Best For | Requirement Changes | Risk Handling | Customer Involvement | Speed |
|------|-----------|--------------------|---------------|----------------------|------|
| Waterfall | Stable projects | Low | Low | Low | Medium |
| V-Model | Safety-critical | Low | Medium | Low | Medium |
| Incremental | Large business apps | Medium | Medium | Medium | High |
| Iterative | Evolving products | High | Medium | High | High |
| Spiral | High-risk systems | High | Very High | High | Medium |
| RAD | Fast business apps | Medium | Medium | Very High | Very High |
| Prototype | Unclear requirements | Very High | Medium | Very High | High |
| Big Bang | Research | Very High | Very Low | Low | High |
| CBD | Enterprise systems | Medium | Medium | Medium | High |

---

# Requirement Stability

```text
Stable ------------------------------> Frequently Changing

Waterfall
V-Model
CBD
Incremental
RAD
Iterative
Prototype
Spiral
Big Bang
```

---

# Documentation

| Heavy Documentation | Moderate | Lightweight |
|---------------------|----------|-------------|
| Waterfall | Incremental | Big Bang |
| V-Model | CBD | Prototype |
| Spiral | RAD | Iterative |

---

# Customer Feedback

```text
Low
 |
Waterfall
V-Model
CBD
Incremental
Iterative
RAD
Prototype
 |
High
```

---

# Risk Management

| Model | Risk Capability |
|------|-----------------|
| Spiral | ★★★★★ |
| V-Model | ★★★★☆ |
| Incremental | ★★★☆☆ |
| Iterative | ★★★☆☆ |
| RAD | ★★★☆☆ |
| CBD | ★★★☆☆ |
| Waterfall | ★★☆☆☆ |
| Prototype | ★★☆☆☆ |
| Big Bang | ★☆☆☆☆ |

---

# Cost of Change

| Model | Cost of Late Changes |
|------|----------------------|
| Waterfall | Very High |
| V-Model | High |
| Incremental | Medium |
| Iterative | Low |
| Agile (Preview) | Very Low |

---

# Industry Mapping

| Project | Recommended Model |
|---------|-------------------|
| Government Portal | Waterfall |
| Medical Device | V-Model |
| Banking Core | V-Model / Spiral |
| E-commerce | Incremental |
| Startup SaaS | Iterative / RAD |
| AI Research | Big Bang / Prototype |
| Enterprise ERP | CBD |
| Hospital System | V-Model |

---

# Strengths Summary

- **Waterfall:** Simplicity, documentation
- **V-Model:** Quality assurance
- **Incremental:** Early value
- **Iterative:** Continuous improvement
- **Spiral:** Risk management
- **RAD:** Rapid delivery
- **Prototype:** Requirement clarity
- **Big Bang:** Innovation
- **CBD:** Reuse and productivity

---

# Weaknesses Summary

- **Waterfall:** Poor flexibility
- **V-Model:** Expensive changes
- **Incremental:** Integration effort
- **Iterative:** Scope growth
- **Spiral:** Costly and complex
- **RAD:** Customer dependency
- **Prototype:** Scope creep
- **Big Bang:** High uncertainty
- **CBD:** Third-party dependency

---

# Decision Matrix

```text
Stable Requirements?
      |
     Yes --------------------+
      |                      |
Need Heavy Compliance?       No
      |                      |
   Waterfall / V             Frequent Feedback?
                             |
                        Yes ----------- No
                         |              |
                Iterative / RAD     Incremental
                         |
               High Risk?
                    |
                 Spiral
```

---

# Interview Questions

1. Which SDLC model is best for stable requirements?
2. Which model emphasizes risk analysis?
3. Which model delivers software incrementally?
4. Difference between Iterative and Incremental?
5. Which model is suitable for research?
6. Why is V-Model preferred in healthcare?

---

# Memory Map

```text
Waterfall  → Sequential
V-Model    → Verification + Validation
Incremental→ Feature by Feature
Iterative  → Improve Again
Spiral     → Risk First
RAD        → Fast Build
Prototype  → Clarify Needs
Big Bang   → Experiment
CBD        → Reuse Components
```

---

# Summary

Every SDLC model solves a different engineering problem. Waterfall and V-Model emphasize predictability, Incremental and Iterative improve flexibility, Spiral manages risk, RAD accelerates delivery, Prototype clarifies uncertain requirements, Big Bang encourages experimentation, and CBD maximizes reuse. Selecting the right model depends on the project's goals, risks, and constraints rather than personal preference.
