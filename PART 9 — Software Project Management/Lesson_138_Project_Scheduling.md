# Lesson 138 --- Project Scheduling

# Part 9 --- Software Project Management

> **Objective**
>
> Understand Project Scheduling, why schedules are important, scheduling
> processes, task sequencing, dependencies, duration estimation,
> schedule baseline, monitoring, and techniques used by project managers
> to deliver software projects on time.

------------------------------------------------------------------------

# Introduction

A software project contains many activities.

These activities must happen:

-   In the correct order
-   Within planned time
-   With available resources

Project Scheduling creates a timeline for completing project work.

``` text
Project Tasks

      ↓

Schedule

      ↓

Execution

      ↓

Delivery
```

------------------------------------------------------------------------

# What is Project Scheduling?

**Project Scheduling** is the process of defining project activities,
arranging them in sequence, estimating durations, and creating a
timeline for project completion.

It defines:

-   When tasks start
-   When tasks finish
-   Task dependencies
-   Milestones
-   Deadlines

------------------------------------------------------------------------

# Why Do We Need Project Scheduling?

Without scheduling:

``` text
No Timeline

      ↓

Poor Coordination

      ↓

Task Delays

      ↓

Project Failure
```

Scheduling helps:

-   Track progress
-   Allocate resources
-   Manage deadlines
-   Identify delays
-   Improve productivity

------------------------------------------------------------------------

# Project Scheduling Process

``` text
Define Activities

        ↓

Sequence Activities

        ↓

Estimate Duration

        ↓

Develop Schedule

        ↓

Monitor Schedule
```

------------------------------------------------------------------------

# 1. Define Activities

Activities are tasks required to complete the project.

Example:

## Software Development Project

    Requirement Analysis

    System Design

    Coding

    Testing

    Deployment

------------------------------------------------------------------------

# 2. Activity Sequencing

Tasks must follow logical order.

Example:

    Requirement Analysis

            ↓

    Design

            ↓

    Development

            ↓

    Testing

            ↓

    Deployment

------------------------------------------------------------------------

# 3. Task Dependencies

Dependencies define relationships between activities.

------------------------------------------------------------------------

# Types of Dependencies

## Finish-to-Start (FS)

Most common dependency.

Example:

    Design Completed

            ↓

    Development Begins

------------------------------------------------------------------------

## Start-to-Start (SS)

Tasks start together.

Example:

    Frontend Development

            ↓

    Backend Development

------------------------------------------------------------------------

## Finish-to-Finish (FF)

Tasks finish together.

Example:

    Testing

            ↓

    Documentation

------------------------------------------------------------------------

## Start-to-Finish (SF)

Rare dependency.

Example:

A new support system starts before an old system finishes.

------------------------------------------------------------------------

# 4. Duration Estimation

Duration estimation predicts task completion time.

Methods:

-   Expert estimation
-   Analogous estimation
-   Three-point estimation

------------------------------------------------------------------------

# Three-Point Estimation

Uses:

    Optimistic (O)

    Most Likely (M)

    Pessimistic (P)

Formula:

    Expected Duration =

    (O + 4M + P) / 6

------------------------------------------------------------------------

# 5. Schedule Development

Schedule development combines:

-   Activities
-   Dependencies
-   Duration
-   Resources

Example:

    Task              Duration

    Requirement       2 weeks

    Design            3 weeks

    Development       8 weeks

    Testing           3 weeks

------------------------------------------------------------------------

# Schedule Baseline

A **Schedule Baseline** is the approved project timeline used for
comparison.

It helps identify:

-   Delays
-   Progress differences
-   Schedule changes

Example:

Planned:

    Release: June

Actual:

    Release: August

Delay:

    2 Months

------------------------------------------------------------------------

# Schedule Monitoring

Schedule monitoring tracks actual progress.

Activities:

-   Compare planned vs actual progress
-   Identify delays
-   Update schedule
-   Take corrective actions

------------------------------------------------------------------------

# Schedule Control

Schedule control manages changes affecting timelines.

Actions:

-   Reassign resources
-   Adjust priorities
-   Update deadlines

------------------------------------------------------------------------

# Scheduling Techniques

------------------------------------------------------------------------

# 1. Gantt Chart

A visual timeline showing:

-   Tasks
-   Duration
-   Progress

Example:

    Task          Jan Feb Mar

    Design        ███

    Development      ██████

    Testing              ███

------------------------------------------------------------------------

# 2. Network Diagram

Shows task relationships.

Example:

    A

    ↓

    B

    ↓

    C

------------------------------------------------------------------------

# 3. Critical Path Method (CPM)

Identifies the longest sequence of dependent tasks.

The critical path determines minimum project duration.

Example:

    Requirement

          ↓

    Development

          ↓

    Testing

          ↓

    Release

------------------------------------------------------------------------

# Schedule Compression

When projects are delayed:

------------------------------------------------------------------------

# 1. Crashing

Adding resources.

Example:

Adding developers.

Advantages:

-   Reduces time

Disadvantages:

-   Increases cost

------------------------------------------------------------------------

# 2. Fast Tracking

Running activities in parallel.

Example:

Testing starts before development completes.

Advantages:

-   Saves time

Disadvantages:

-   Higher risk

------------------------------------------------------------------------

# Agile Project Scheduling

Agile uses:

-   Sprints
-   Backlogs
-   Iterations

Example:

    Sprint 1

    Feature A


    Sprint 2

    Feature B

Benefits:

-   Frequent delivery
-   Continuous feedback
-   Flexible planning

------------------------------------------------------------------------

# Project Scheduling Example

## Online Learning Platform

Schedule:

    Requirement Analysis

    2 weeks

            ↓

    UI Design

    3 weeks

            ↓

    Development

    12 weeks

            ↓

    Testing

    4 weeks

            ↓

    Deployment

    1 week

------------------------------------------------------------------------

# Common Scheduling Challenges

## 1. Unrealistic Deadlines

Solution:

Use accurate estimation.

------------------------------------------------------------------------

## 2. Dependency Problems

Solution:

Identify dependencies early.

------------------------------------------------------------------------

## 3. Resource Conflicts

Solution:

Use resource planning.

------------------------------------------------------------------------

## 4. Requirement Changes

Solution:

Use change management.

------------------------------------------------------------------------

# Project Scheduling vs Time Management

  Project Scheduling         Time Management
  -------------------------- -----------------------
  Creates project timeline   Controls project time
  Defines task dates         Monitors time usage
  Activity focused           Overall process

------------------------------------------------------------------------

# Best Practices

-   Create realistic schedules
-   Identify dependencies early
-   Include buffer time
-   Track progress regularly
-   Update schedules when needed
-   Communicate changes

------------------------------------------------------------------------

# Interview Questions

1.  What is Project Scheduling?
2.  Why is scheduling important?
3.  Explain scheduling process.
4.  What are task dependencies?
5.  Explain schedule baseline.
6.  What is Critical Path Method?
7.  Difference between crashing and fast tracking?
8.  How does Agile handle scheduling?

------------------------------------------------------------------------

# Cheat Sheet

``` text
Project Scheduling

Activities

     ↓

Sequence

     ↓

Estimate

     ↓

Schedule

     ↓

Monitor

     ↓

Control
```

------------------------------------------------------------------------

# Summary

Project Scheduling creates a structured timeline for software project
execution. It involves defining activities, sequencing tasks, estimating
duration, developing schedules, and monitoring progress. Effective
scheduling helps teams deliver software on time while managing
dependencies, resources, and project constraints.
