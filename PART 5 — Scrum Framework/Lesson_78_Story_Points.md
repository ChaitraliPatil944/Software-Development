# Lesson 78 — Story Points

# Part 5 — Scrum Framework

> **Objective**
>
> Understand Story Points, why Agile teams use them instead of hours, how estimation works, the Fibonacci scale, Planning Poker, and how Story Points help Sprint planning.

---

# Introduction

Software development contains uncertainty.

A feature that looks simple may become complicated because of:

- Unknown requirements
- Technical challenges
- Dependencies
- Testing effort

Agile teams estimate work using **Story Points**.

```text
User Story
      ↓
Estimate Effort
      ↓
Story Points
      ↓
Sprint Planning
```

---

# What are Story Points?

Story Points are a unit used to estimate the **relative effort** required to complete a User Story.

They consider:

- Complexity
- Effort
- Risk
- Uncertainty

---

# Important Concept

Story Points are NOT:

❌ Hours  
❌ Days  
❌ Developer performance score

Story Points represent relative size.

---

# Why Not Estimate in Hours?

Traditional estimation:

```
Feature = 20 hours
```

Problems:

- Difficult to predict accurately
- Different developers work differently
- Ignores complexity and risk

Agile estimation:

```
Feature A = 3 Points
Feature B = 8 Points
```

Teams compare size instead of guessing exact time.

---

# Story Point Factors

A team considers:

## 1. Complexity

How difficult is the work?

Example:

Simple login:

Low complexity

AI recommendation system:

High complexity

---

## 2. Effort

How much work is required?

Includes:

- Coding
- Testing
- Integration

---

## 3. Risk and Uncertainty

Unknown factors increase points.

Example:

Integrating a new external payment system.

---

# Relative Estimation

Teams compare stories.

Example:

```text
User Login

★★

Payment Gateway

★★★★★
```

Payment is larger because it has:

- More complexity
- More risk
- More testing

---

# Fibonacci Scale

Most Agile teams use:

```text
1
2
3
5
8
13
21
```

---

# Why Fibonacci Numbers?

As tasks become larger, uncertainty increases.

Example:

Difference between:

1 and 2

is small.

Difference between:

13 and 21

represents significant uncertainty.

---

# Story Point Examples

## Food Delivery Application

| User Story | Story Points |
|---|---:|
| Login | 2 |
| Profile Update | 3 |
| Restaurant Search | 5 |
| Order Placement | 8 |
| Payment Integration | 13 |

---

# Planning Poker

Planning Poker is a team-based estimation technique.

## Process

```text
Product Owner explains Story

        ↓

Team discusses requirements

        ↓

Everyone selects estimate

        ↓

Cards revealed

        ↓

Discussion

        ↓

Final Estimate
```

---

# Example

Story:

"Add payment gateway."

Estimates:

Developer A:

5 points

Developer B:

13 points

Developer C:

8 points

Discussion:

Why are estimates different?

Final agreement:

8 points

---

# Story Points and Velocity

Velocity is the amount of Story Points completed in a Sprint.

Example:

Sprint 1:

30 Points

Sprint 2:

35 Points

Sprint 3:

32 Points

Average:

```text
(30 + 35 + 32) / 3

= 32 Points
```

Future Sprint capacity:

≈ 32 Points

---

# Story Point Workflow

```text
User Story

      ↓

Team Discussion

      ↓

Estimate Complexity

      ↓

Assign Story Points

      ↓

Sprint Planning

      ↓

Track Velocity
```

---

# Industry Example

## Banking Application

Story:

"Enable international money transfer."

Factors:

Complexity:

High

Risk:

High security requirements

Testing:

Extensive

Estimate:

13 Story Points

---

# Story Points vs Hours

| Story Points | Hours |
|---|---|
| Relative measurement | Time measurement |
| Team-specific | Individual-specific |
| Includes complexity | Mainly duration |
| Used in Agile | Traditional estimation |

---

# Common Mistakes

## Mistake 1

Treating points as hours.

Wrong:

"5 points means 5 hours."

Correct:

Points represent relative effort.

---

## Mistake 2

Comparing different teams.

Example:

Team A velocity = 50

Team B velocity = 30

This does not mean Team A is better.

---

## Mistake 3

Using points to measure individual performance.

Velocity measures team capacity.

---

# Interview Questions

1. What are Story Points?
2. Why does Agile use Story Points?
3. Do Story Points represent hours?
4. Why is Fibonacci used?
5. What factors affect Story Points?
6. Explain Planning Poker.
7. How are Story Points related to Velocity?

---

# Cheat Sheet

```text
Story Points

Measure:
✓ Complexity
✓ Effort
✓ Risk
✓ Uncertainty


Not:
✗ Hours
✗ Days
✗ Developer Ranking
```

---

# Summary

Story Points provide Agile teams with a practical way to estimate work by focusing on relative effort instead of exact time predictions. By considering complexity, effort, risk, and uncertainty, teams can create more realistic Sprint plans and improve delivery forecasting through historical velocity.
