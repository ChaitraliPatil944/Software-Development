# Lesson 79 — Velocity

# Part 5 — Scrum Framework

> **Objective**
>
> Understand Velocity in Scrum, why teams use it, how it is calculated, how it helps Sprint planning, common mistakes, and why Velocity should be used for forecasting rather than measuring individual performance.

---

# Introduction

A Scrum team needs a way to understand:

- How much work can we complete in a Sprint?
- How much work can we plan in future Sprints?
- Are we becoming more predictable?

Velocity provides this measurement.

```text
Completed Work
       ↓
Velocity
       ↓
Future Planning
```

---

# What is Velocity?

**Velocity** is the amount of work a Scrum Team completes during a Sprint, usually measured in Story Points.

Formula:

```text
Velocity = Completed Story Points in a Sprint
```

---

# Example

Sprint Completion:

```text
Login              3 Points
Search             5 Points
Profile            2 Points

Total Velocity = 10 Points
```

The team's Velocity for that Sprint is:

```text
10 Story Points
```

---

# Why Do We Need Velocity?

Without Velocity:

```text
Guessing Future Work
        ↓
Overcommitment
        ↓
Missed Sprint Goals
```

With Velocity:

```text
Historical Data
        ↓
Better Forecasting
        ↓
Realistic Sprint Planning
```

---

# How Velocity Works

A team completes multiple Sprints.

Example:

| Sprint | Completed Points |
|---|---:|
| Sprint 1 | 25 |
| Sprint 2 | 30 |
| Sprint 3 | 35 |

Average Velocity:

```text
(25 + 30 + 35) / 3

= 30 Story Points
```

Future Sprint Capacity:

Approximately:

```text
30 Points
```

---

# Velocity Calculation

Formula:

```text
Average Velocity =

Total Completed Story Points
----------------------------
Number of Sprints
```

Example:

Total:

```text
40 + 35 + 45 = 120
```

Sprints:

```text
3
```

Average:

```text
120 / 3 = 40
```

Velocity:

```text
40 Points
```

---

# Velocity and Sprint Planning

During Sprint Planning:

Team knows:

Average Velocity:

```text
35 Points
```

Selected Sprint Work:

```text
≈ 35 Points
```

This creates realistic planning.

---

# Velocity Example

## E-Commerce Application

Sprint History:

Sprint 1:

- Login
- Product Search

Velocity:

28 Points


Sprint 2:

- Cart
- Checkout

Velocity:

32 Points


Sprint 3:

- Payment

Velocity:

30 Points


Average Velocity:

```text
(28 + 32 + 30) / 3

= 30 Points
```

Next Sprint:

Plan around 30 Points.

---

# Velocity vs Productivity

Velocity:

Measures:

"How much work did the team complete?"

Productivity:

Measures:

"How efficiently did individuals work?"

They are different.

---

# Velocity Does NOT Measure

Velocity should not measure:

❌ Developer performance

❌ Individual contribution

❌ Code quality

❌ Business value directly

---

# Velocity Misuse

## Wrong Usage

Manager:

"Team A has 50 points, Team B has 30 points. Team A is better."

Incorrect.

Different teams:

- Estimate differently
- Have different complexity
- Work on different products

---

# Factors Affecting Velocity

Velocity can change because of:

## Team Changes

New members need time to adapt.

---

## Technical Complexity

Difficult features reduce completion.

---

## Dependencies

External delays affect delivery.

---

## Learning Curve

New technology affects speed.

---

# Velocity Trend

Teams track Velocity over time.

Example:

```text
Sprint 1
20 Points

Sprint 2
25 Points

Sprint 3
30 Points

Sprint 4
32 Points
```

Trend:

Improving predictability.

---

# Velocity Workflow

```text
Sprint Completed

        ↓

Calculate Completed Points

        ↓

Record Velocity

        ↓

Analyze Trend

        ↓

Plan Future Sprint
```

---

# Velocity and Release Planning

Example:

Product Remaining Work:

300 Story Points

Team Velocity:

30 Points/Sprint

Estimated Sprints:

```text
300 / 30 = 10 Sprints
```

If Sprint duration:

2 weeks

Estimated Release:

```text
20 Weeks
```

---

# Industry Example

## Banking Software

Remaining Work:

200 Points

Team Velocity:

25 Points/Sprint

Forecast:

```text
200 / 25

= 8 Sprints
```

The team can estimate delivery timeline.

---

# Common Mistakes

## Mistake 1

Increasing points to show improvement.

Solution:

Keep estimation consistent.

---

## Mistake 2

Comparing team velocities.

Solution:

Use Velocity only within the same team.

---

## Mistake 3

Using Velocity as a performance metric.

Solution:

Use it for planning.

---

# Interview Questions

1. What is Velocity in Scrum?
2. How is Velocity calculated?
3. Why is Velocity important?
4. Can Velocity measure developer performance?
5. How is Average Velocity calculated?
6. How does Velocity help release planning?
7. Difference between Velocity and Productivity?

---

# Cheat Sheet

```text
Velocity

Completed Story Points
          ↓
Sprint Capacity
          ↓
Future Forecasting


Use:
✓ Planning
✓ Prediction
✓ Improvement


Do Not Use:
✗ Ranking Teams
✗ Measuring Developers
```

---

# Summary

Velocity is a Scrum metric that helps teams understand their delivery capacity and improve forecasting. By measuring completed Story Points over multiple Sprints, teams can plan realistic workloads and estimate future releases. Velocity is a planning tool, not a performance measurement system.
