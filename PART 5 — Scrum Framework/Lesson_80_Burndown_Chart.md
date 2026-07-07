# Lesson 80 — Burndown Chart

# Part 5 — Scrum Framework

> **Objective**
>
> Understand Burndown Charts, why Scrum teams use them, how they visualize Sprint progress, how to interpret them, and how they help teams identify delivery risks.

---

# Introduction

A Scrum Team needs visibility into Sprint progress.

A Burndown Chart answers:

- How much work remains?
- Are we progressing as planned?
- Will we achieve the Sprint Goal?

```text
Sprint Work

      ↓

Progress Tracking

      ↓

Burndown Chart

      ↓

Better Decisions
```

---

# What is a Burndown Chart?

A **Burndown Chart** is a graphical representation of remaining work over time during a Sprint.

It shows:

- Remaining effort
- Time remaining
- Sprint progress

---

# Basic Burndown Chart Structure

```text
Remaining Work

100 |
    |
 80 |\
    | \
 60 |  \
    |   \
 40 |    \
    |     \
 20 |      \
    |       \
  0 |________\________

       Time →
```

The ideal goal:

```text
Remaining Work decreases to Zero
```

---

# Why Do We Need Burndown Charts?

Without tracking:

```text
Sprint Starts
      ↓
No Visibility
      ↓
Problems Found Late
      ↓
Sprint Failure
```

With Burndown Charts:

```text
Progress Visible
      ↓
Problems Detected Early
      ↓
Team Adapts
```

---

# What Does a Burndown Chart Measure?

Usually:

- Story Points remaining
- Tasks remaining
- Hours remaining

Most Scrum teams track:

```text
Remaining Story Points
```

---

# Components of Burndown Chart

## 1. X-Axis

Represents time.

Example:

```text
Days of Sprint
```

---

## 2. Y-Axis

Represents remaining work.

Example:

```text
Story Points
```

---

## 3. Ideal Line

Shows expected progress.

```text
Start
 |
 |
 \ 
  \
   \
    End
```

---

## 4. Actual Progress Line

Shows real team progress.

---

# Ideal vs Actual Burndown

## Ideal Progress

```text
40 Points

Day 1
 |
30 Points
 |
20 Points
 |
10 Points
 |
0
```

---

## Actual Progress

Example:

```text
Day 1: 40 Points

Day 3: 35 Points

Day 5: 30 Points

Day 8: 10 Points

Day 10: 0
```

---

# Interpreting Burndown Charts

## Scenario 1 — On Track

```text
Actual Line ≈ Ideal Line
```

Meaning:

Team is progressing normally.

---

## Scenario 2 — Behind Schedule

```text
Actual Work
      |
      |
      Above Ideal Line
```

Meaning:

Team has more remaining work than expected.

Possible reasons:

- Blockers
- Underestimation
- Technical issues

---

## Scenario 3 — Ahead of Schedule

```text
Actual Line
      |
      |
Below Ideal Line
```

Meaning:

Work is completing faster.

---

# Burndown Chart Example

## Food Delivery Application

Sprint:

2 Weeks

Sprint Backlog:

40 Story Points

Progress:

Day 1:

40 Points

Day 5:

25 Points

Day 10:

5 Points

Day 14:

0 Points

Result:

Sprint completed successfully.

---

# How Teams Use Burndown Charts

During Daily Scrum:

Team checks:

- Remaining work
- Progress trend
- Possible risks

Example:

Problem:

Remaining work is not decreasing.

Action:

- Remove blockers
- Re-plan tasks
- Get help from team members

---

# Burndown Chart Workflow

```text
Sprint Planning

      ↓

Estimate Work

      ↓

Start Sprint

      ↓

Track Remaining Work Daily

      ↓

Analyze Trend

      ↓

Adjust Plan
```

---

# Burndown Chart vs Velocity

| Burndown Chart | Velocity |
|---|---|
| Shows Sprint progress | Shows completed work capacity |
| Used during Sprint | Used across Sprints |
| Daily tracking | Historical measurement |

---

# Burndown Chart vs Burnup Chart

| Burndown | Burnup |
|---|---|
| Shows remaining work | Shows completed work |
| Line goes downward | Line goes upward |
| Good for Sprint tracking | Good for scope changes |

---

# Industry Example

## Banking Application

Sprint Goal:

"Enable mobile money transfer."

Sprint Backlog:

50 Story Points

Burndown shows:

Day 7:

Still 40 points remaining.

Team identifies:

- API dependency issue
- Testing delay

Action:

Scrum Master removes blockers.

---

# Common Mistakes

## Mistake 1

Using Burndown to judge developers.

Solution:

Use it for team planning.

---

## Mistake 2

Updating only at Sprint end.

Solution:

Track progress regularly.

---

## Mistake 3

Ignoring reasons behind changes.

Solution:

Discuss problems during Daily Scrum.

---

# Interview Questions

1. What is a Burndown Chart?
2. Why is Burndown Chart used in Scrum?
3. What does the X-axis represent?
4. What does the Y-axis represent?
5. Difference between Burndown and Burnup Chart?
6. How does Burndown help identify risks?
7. Can Burndown measure developer performance?

---

# Cheat Sheet

```text
Burndown Chart

X-Axis:
Time

Y-Axis:
Remaining Work


Purpose:
Track Sprint Progress

Goal:
Work → Zero
```

---

# Summary

A Burndown Chart is a visual Scrum tool that helps teams monitor remaining work throughout a Sprint. It improves transparency, identifies delivery risks early, and supports better decision-making. It is a forecasting and communication tool, not a performance measurement system.
