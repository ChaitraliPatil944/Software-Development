# Lesson 125 --- Activity Diagrams

# Part 8 --- Software Design

> **Objective**
>
> Understand Activity Diagrams, their purpose in software design,
> workflow modeling, activity diagram symbols, decisions, parallel
> activities, swimlanes, and how they represent system processes.

------------------------------------------------------------------------

# Introduction

Software systems contain many workflows.

Before implementation, teams need to understand:

-   What activities happen?
-   In what order do they happen?
-   What decisions affect the flow?
-   Which component performs each activity?

Activity Diagrams help visualize workflows.

``` text
Business Process

        ↓

Activity Diagram

        ↓

System Implementation
```

------------------------------------------------------------------------

# What is an Activity Diagram?

An **Activity Diagram** is a UML behavioral diagram that represents the
flow of activities and actions within a system or process.

It shows:

-   Activities
-   Decisions
-   Flow of control
-   Parallel execution
-   Start and end points

------------------------------------------------------------------------

# Why Do We Need Activity Diagrams?

Without workflow modeling:

``` text
Complex Process

        ↓

Unclear Execution Flow

        ↓

Implementation Errors
```

Activity diagrams help:

-   Understand business workflows
-   Analyze system behavior
-   Document processes
-   Identify missing steps
-   Improve communication

------------------------------------------------------------------------

# Activity Diagram Structure

Main elements:

``` text
Activity Diagram

        |
--------------------------------
|        |        |             |
Activity Decision Flow      Start/End
```

------------------------------------------------------------------------

# Basic Activity Diagram Symbols

## 1. Initial Node

Represents the beginning of a process.

Example:

    ● Start

------------------------------------------------------------------------

## 2. Activity

Represents an action or task.

Example:

    +----------------+
    | Login User     |
    +----------------+

------------------------------------------------------------------------

## 3. Decision Node

Represents a condition.

Example:

            ◇
           / \
         Yes  No

------------------------------------------------------------------------

## 4. Final Node

Represents completion.

Example:

    ◎ End

------------------------------------------------------------------------

## 5. Flow Arrow

Shows movement from one activity to another.

Example:

    Activity A

          ↓

    Activity B

------------------------------------------------------------------------

# Basic Activity Diagram Example

## Login Process

``` text
Start

  ↓

Enter Username Password

  ↓

Validate Credentials

  ↓

Credentials Valid?

       ◇
      / \

    Yes  No

     ↓    ↓

Dashboard Error Message

     ↓

    End
```

------------------------------------------------------------------------

# Decision Nodes

Decision nodes represent conditional logic.

Example:

## Payment Process

``` text
Start

 ↓

Make Payment

 ↓

Payment Successful?

        ◇
       / \

     Yes  No

      ↓    ↓

 Confirm  Retry

 Order
```

------------------------------------------------------------------------

# Fork and Join

Activity diagrams can represent parallel execution.

## Fork

Splits one activity into multiple parallel activities.

Example:

              Process Order

                   |
                  Fork

            /             \

    Update Inventory   Send Notification

------------------------------------------------------------------------

## Join

Combines parallel activities.

Example:

    Update Inventory

            \

             Join

            /

    Send Notification

------------------------------------------------------------------------

# Swimlanes

Swimlanes divide activities based on responsibility.

Example:

## Online Shopping

    Customer          System

       |                |

    Search Product     |

       |                |

    Place Order ------>

                      Process Order

                      Make Payment

They show:

-   Who performs an action
-   System responsibility
-   Role separation

------------------------------------------------------------------------

# Activity Diagram Example

## ATM Withdrawal

``` text
Start

 ↓

Insert Card

 ↓

Enter PIN

 ↓

Validate PIN

 ↓

PIN Correct?

       ◇
      / \

    Yes  No

     ↓    ↓

Enter   Display Error
Amount

     ↓

Check Balance

     ↓

Dispense Cash

     ↓

End
```

------------------------------------------------------------------------

# Activity Diagram vs Sequence Diagram

  Activity Diagram        Sequence Diagram
  ----------------------- ----------------------
  Shows workflow          Shows communication
  Focuses on activities   Focuses on objects
  Process-oriented        Interaction-oriented

------------------------------------------------------------------------

# Activity Diagram vs Flowchart

  Activity Diagram           Flowchart
  -------------------------- -----------------------------
  UML behavioral diagram     General process diagram
  Models system behavior     Models algorithms/processes
  Supports object concepts   Simpler representation

------------------------------------------------------------------------

# Activity Diagram in Software Design

Used for:

-   Business process modeling
-   Use case modeling
-   Algorithm visualization
-   System workflow analysis

Examples:

-   Order processing
-   Banking transactions
-   User registration
-   Approval workflows

------------------------------------------------------------------------

# Industry Example

## Loan Approval System

Workflow:

``` text
Customer Applies

        ↓

Document Verification

        ↓

Credit Check

        ↓

Approved?

       ◇
      / \

    Yes  No

     ↓    ↓

Loan    Rejection
Disbursed
```

------------------------------------------------------------------------

# Benefits of Activity Diagrams

-   Easy workflow understanding
-   Improves communication
-   Finds process issues
-   Helps requirement analysis
-   Supports system design

------------------------------------------------------------------------

# Limitations

-   Large workflows become complex
-   Not suitable for detailed implementation logic
-   Requires maintenance when processes change

------------------------------------------------------------------------

# Common Mistakes

## Mistake 1

Creating overly detailed diagrams.

Solution:

Focus on important workflow steps.

------------------------------------------------------------------------

## Mistake 2

Missing alternate paths.

Solution:

Include error and exception flows.

------------------------------------------------------------------------

## Mistake 3

Ignoring responsibilities.

Solution:

Use swimlanes when needed.

------------------------------------------------------------------------

# Best Practices

-   Start with clear process goals
-   Use meaningful activity names
-   Represent decisions clearly
-   Use swimlanes for responsibilities
-   Keep diagrams simple

------------------------------------------------------------------------

# Interview Questions

1.  What is an Activity Diagram?
2.  Why are activity diagrams used?
3.  Difference between activity and sequence diagrams?
4.  What is a decision node?
5.  Explain fork and join.
6.  What are swimlanes?
7.  How are activity diagrams used in software design?

------------------------------------------------------------------------

# Cheat Sheet

``` text
Activity Diagram

Start

 ↓

Activities

 ↓

Decision

 ↓

Parallel Flow

 ↓

End
```

------------------------------------------------------------------------

# Summary

Activity Diagrams represent workflows and system processes visually.
They help teams understand execution flow, decisions, parallel
activities, and responsibilities before implementation. They are widely
used during requirement analysis and software design to communicate
complex processes clearly.
