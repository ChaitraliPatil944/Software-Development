# Lesson 59 — Agile Estimation

# Part 4 — Agile Software Development

> **Objective**
>
> Understand how Agile teams estimate work, why estimation is necessary, the most common estimation techniques used in industry, and how estimates help with sprint planning and release forecasting.

---

# Introduction

Software teams are often asked:

- How long will this feature take?
- Can we finish it this sprint?
- When can we release it?

Instead of estimating exact hours for every task, Agile focuses on estimating the **relative effort**.

```text
New Feature
      ↓
Estimate Effort
      ↓
Sprint Planning
      ↓
Development
```

---

# Why Agile Estimation Exists

Estimation helps teams:

- Plan sprints
- Predict delivery
- Balance workload
- Reduce uncertainty
- Improve forecasting

It is **not** meant to measure developer performance.

---

# Relative Estimation

Instead of asking:

> "Will this take exactly 14 hours?"

Agile asks:

> "Is Feature A easier or harder than Feature B?"

```text
Login        ★★
Search       ★★★
Payments     ★★★★★
```

---

# Story Points

## What are Story Points?

Story Points measure the **relative effort, complexity, risk, and uncertainty** of a user story.

They do **not** represent hours.

Factors considered:

- Complexity
- Amount of work
- Unknowns
- Risk

### Example

| User Story | Story Points |
|------------|-------------:|
| Login | 2 |
| Profile | 3 |
| Shopping Cart | 8 |
| Payment Gateway | 13 |

---

# Fibonacci Sequence

Most Scrum teams use:

```text
1 2 3 5 8 13 21 34 55
```

Why?

As work becomes larger, uncertainty grows. The increasing gaps reflect this uncertainty.

---

# Planning Poker

A collaborative estimation technique.

## Steps

1. Product Owner explains the story.
2. Team discusses requirements.
3. Everyone secretly selects a card.
4. Cards are revealed together.
5. Differences are discussed.
6. Consensus is reached.

```text
Developer A → 5
Developer B → 8
Developer C → 5

Discuss
      ↓
Final Estimate = 5
```

Benefits:

- Encourages discussion
- Reduces bias
- Improves shared understanding

---

# T-Shirt Sizing

Useful for high-level estimation.

```text
XS → Very Small
S  → Small
M  → Medium
L  → Large
XL → Very Large
```

Example:

| Feature | Size |
|---------|------|
| Login | S |
| Search | M |
| Reports | L |
| AI Recommendation Engine | XL |

---

# Affinity Estimation

Stories are grouped by similar effort.

```text
Small
  |
Login
Profile

Medium
  |
Search
Notifications

Large
  |
Payments
Analytics
```

Fast and useful for estimating many stories.

---

# Ideal Days

Some organizations estimate using **Ideal Days**.

Definition:

The number of days required if a developer works without interruptions.

Example:

```text
Task = 2 Ideal Days

Actual Calendar Time
≈ 3–4 Days
```

This approach is less common than Story Points.

---

# Velocity-Based Planning

Once a team's average velocity is known:

```text
Average Velocity = 30 Story Points
```

Sprint Backlog should contain approximately:

```text
≈ 30 Story Points
```

This improves sprint predictability.

---

# Industry Example

## Online Shopping Platform

Stories:

- Login → 3 SP
- Search → 5 SP
- Cart → 8 SP
- Payments → 13 SP

Average Velocity:

29 SP

Selected Sprint Work:

3 + 5 + 8 + 13 = 29 SP

The sprint is planned within the team's historical capacity.

---

# Comparison of Estimation Techniques

| Technique | Best Use |
|-----------|----------|
| Story Points | Sprint planning |
| Planning Poker | Team estimation |
| Fibonacci | Relative sizing |
| T-Shirt Sizing | Early planning |
| Affinity Estimation | Large backlogs |
| Ideal Days | Small projects or legacy teams |

---

# Best Practices

- Estimate as a team.
- Break large stories into smaller ones.
- Re-estimate when requirements change.
- Use historical velocity.
- Focus on consistency rather than precision.

---

# Common Mistakes

❌ Converting Story Points directly into hours.

✔ Story Points represent relative effort.

❌ Comparing story points across teams.

✔ Every team has its own estimation scale.

❌ Treating estimates as guarantees.

✔ Estimates are informed forecasts.

---

# Interview Questions

1. What are Story Points?
2. Why doesn't Agile estimate only in hours?
3. Why is the Fibonacci sequence used?
4. Explain Planning Poker.
5. What is T-Shirt Sizing?
6. What is Affinity Estimation?
7. How does Velocity help sprint planning?

---

# Cheat Sheet

```text
Story Points → Relative Effort
Fibonacci    → 1 2 3 5 8 13...
Planning Poker → Team Consensus
T-Shirt Sizes → XS S M L XL
Affinity      → Group Similar Work
Ideal Days    → Uninterrupted Work
Velocity      → Sprint Capacity
```

---

# Summary

Agile estimation helps teams make realistic planning decisions by measuring relative effort instead of exact time. Techniques such as Story Points, Planning Poker, Fibonacci estimation, T-Shirt Sizing, Affinity Estimation, and Velocity-based planning improve collaboration, forecasting, and sprint predictability while acknowledging the uncertainty inherent in software development.
