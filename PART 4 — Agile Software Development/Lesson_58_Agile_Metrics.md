# Lesson 58 — Agile Metrics

# Part 4 — Agile Software Development

> **Objective**
>
> Understand how Agile teams measure progress, predict delivery, identify bottlenecks, and continuously improve using Agile metrics.

---

# Introduction

Agile teams make decisions using **data**, not guesses.

Metrics help answer questions such as:

- Are we improving?
- Can we finish the sprint?
- Where are bottlenecks?
- How fast do we deliver value?

> **Important:** Metrics should improve the process, **not** judge individuals.

---

# Why Agile Metrics Matter

```text
Collect Data
      ↓
Measure Progress
      ↓
Find Problems
      ↓
Improve Process
      ↓
Better Software
```

Benefits:

- Better planning
- Higher transparency
- Predictable delivery
- Continuous improvement

---

# Common Agile Metrics

```text
Agile Metrics

├── Velocity
├── Burndown Chart
├── Burnup Chart
├── Lead Time
├── Cycle Time
├── Throughput
├── Cumulative Flow Diagram (CFD)
└── Defect Metrics
```

---

# 1. Velocity

## What is Velocity?

Velocity is the **total story points completed in a sprint**.

Formula:

```text
Velocity = Completed Story Points
```

### Example

Sprint 1 = 30 SP

Sprint 2 = 34 SP

Sprint 3 = 32 SP

Average Velocity:

```text
(30 + 34 + 32) / 3 = 32 Story Points
```

### Why it matters

- Sprint planning
- Capacity prediction
- Release forecasting

---

# 2. Burndown Chart

Shows **remaining work over time**.

```text
Story Points

40 |\
35 | \
30 |  \
20 |   \
10 |    \
 0 +-----\--------> Time
```

Ideal trend:

Remaining work steadily decreases until zero.

Uses:

- Sprint tracking
- Detecting delays early

---

# 3. Burnup Chart

Shows:

- Work completed
- Total scope

```text
Completed
 ^
 |        /
 |      /
 |    /
 |__/
 +---------------> Time

Total Scope ─────────────
```

Useful when project scope changes frequently.

---

# 4. Lead Time

Lead Time measures:

```text
Customer Request
        ↓
Delivered to Customer
```

Formula:

```text
Lead Time = Delivery Date − Request Date
```

Lower lead time generally means faster customer value.

---

# 5. Cycle Time

Measures:

```text
Work Started
      ↓
Work Completed
```

Formula:

```text
Cycle Time = Completion Date − Start Date
```

Unlike Lead Time, waiting before development is not included.

---

# Lead Time vs Cycle Time

| Lead Time | Cycle Time |
|-----------|------------|
| Request → Delivery | Start → Completion |
| Includes waiting | Excludes waiting |
| Customer perspective | Team perspective |

---

# 6. Throughput

Throughput measures:

**Number of work items completed in a given period.**

Example:

```text
Monday      5 Tasks
Tuesday     7 Tasks
Wednesday   6 Tasks
```

Higher throughput often indicates better delivery flow.

---

# 7. Cumulative Flow Diagram (CFD)

Tracks work in different stages.

```text
Done
──────────────

Testing
────────────

Development
─────────

To Do
──────
```

Purpose:

- Identify bottlenecks
- Monitor work-in-progress
- Improve workflow

---

# 8. Defect Metrics

Useful metrics include:

- Defect Density
- Defect Leakage
- Defect Resolution Time
- Reopened Defects

Goal:

Improve software quality over time.

---

# Industry Example

## Food Delivery App

Sprint Metrics

Velocity:

32 Story Points

Cycle Time:

3 Days

Lead Time:

6 Days

Throughput:

18 Tasks

Burndown:

Completed before sprint end.

Result:

Predictable delivery with stable performance.

---

# Choosing the Right Metric

| Goal | Metric |
|------|--------|
| Sprint Planning | Velocity |
| Remaining Work | Burndown |
| Scope Tracking | Burnup |
| Customer Delivery Speed | Lead Time |
| Development Speed | Cycle Time |
| Work Output | Throughput |
| Workflow Bottlenecks | CFD |
| Quality | Defect Metrics |

---

# Best Practices

- Measure trends, not individuals.
- Review metrics every sprint.
- Combine multiple metrics.
- Use metrics for improvement.
- Keep data transparent.

---

# Common Mistakes

❌ Comparing team velocities.

✔ Velocity is team-specific.

❌ Maximizing story points.

✔ Focus on customer value.

❌ Ignoring quality metrics.

✔ Track both speed and quality.

---

# Interview Questions

1. What is Velocity?
2. How is Velocity calculated?
3. Differentiate Lead Time and Cycle Time.
4. What is a Burndown Chart?
5. What is a Burnup Chart?
6. Why is a CFD useful?
7. Which metric measures completed work items?

---

# Cheat Sheet

```text
Velocity      → Story Points Completed
Burndown      → Remaining Work
Burnup        → Completed Work + Scope
Lead Time     → Request → Delivery
Cycle Time    → Start → Finish
Throughput    → Items Completed
CFD           → Workflow Health
Defects       → Quality
```

---

# Summary

Agile metrics provide objective insights into delivery speed, workflow efficiency, predictability, and software quality. Metrics such as Velocity, Burndown, Burnup, Lead Time, Cycle Time, Throughput, and Cumulative Flow Diagrams help Agile teams make better decisions, identify improvement opportunities, and deliver greater value without losing sight of quality.
