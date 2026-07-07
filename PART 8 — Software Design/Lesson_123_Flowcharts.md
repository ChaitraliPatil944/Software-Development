# Lesson 123 --- Flowcharts

# Part 8 --- Software Design

> **Objective**
>
> Understand Flowcharts, their purpose in software design, standard
> symbols, decision making, loops, process representation, and how they
> help developers visualize logic before implementation.

------------------------------------------------------------------------

# Introduction

Before writing code, developers often need to understand the steps of a
process.

A flowchart represents the sequence of operations visually.

``` text
Problem

   ↓

Flowchart

   ↓

Algorithm

   ↓

Code
```

------------------------------------------------------------------------

# What is a Flowchart?

A **Flowchart** is a graphical representation of a process, algorithm,
or workflow using standardized symbols.

It shows:

-   Steps
-   Decisions
-   Inputs
-   Outputs
-   Flow direction

------------------------------------------------------------------------

# Why Do We Need Flowcharts?

Without visualization:

``` text
Complex Logic

      ↓

Poor Understanding

      ↓

Coding Errors
```

Flowcharts help:

-   Understand logic clearly
-   Plan algorithms
-   Communicate processes
-   Find logical errors
-   Simplify complex workflows

------------------------------------------------------------------------

# Basic Flowchart Structure

A typical flowchart follows:

``` text
Start

 ↓

Process

 ↓

Decision

 ↓

Output

 ↓

End
```

------------------------------------------------------------------------

# Common Flowchart Symbols

## 1. Terminator Symbol

Represents start and end.

Example:

    (Start)

    (End)

------------------------------------------------------------------------

## 2. Process Symbol

Represents an operation or action.

Example:

    +-------------+
    | Calculate   |
    | Total       |
    +-------------+

------------------------------------------------------------------------

## 3. Decision Symbol

Represents a condition.

Example:

           /\
          /  \
         / Yes\
        /______\
           |
          No

------------------------------------------------------------------------

## 4. Input/Output Symbol

Represents data input or output.

Example:

     /------------/
    | Enter Data |
    /------------/

------------------------------------------------------------------------

## 5. Flow Line

Shows direction of execution.

Example:

    Step 1

      ↓

    Step 2

------------------------------------------------------------------------

# Flowchart Example

## Login System

``` text
Start

  ↓

Enter Username and Password

  ↓

Validate Credentials

  ↓

Are credentials valid?

      /        \

    Yes        No

     ↓          ↓

Dashboard   Error Message

     ↓

    End
```

------------------------------------------------------------------------

# Decision Making in Flowcharts

Decisions use conditions.

Example:

## Check Number

``` text
Start

 ↓

Enter Number

 ↓

Number > 0?

    /     \

  Yes      No

   ↓        ↓

Positive  Negative
```

------------------------------------------------------------------------

# Loops in Flowcharts

Loops represent repeated execution.

Example:

## Print Numbers

``` text
Start

 ↓

Initialize i = 1

 ↓

i <= 10?

  /      \

Yes      No

 |        |

Print i  End

 |

Increase i

 |

Back to condition
```

------------------------------------------------------------------------

# Flowcharts in Software Development

Flowcharts are used for:

-   Algorithm design
-   Business processes
-   Program logic
-   Debugging
-   Documentation

------------------------------------------------------------------------

# Flowchart Example: ATM Withdrawal

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

     /       \

   Yes        No

    ↓          ↓

Enter Amount Error

    ↓

Check Balance

    ↓

Withdraw Money

    ↓

End
```

------------------------------------------------------------------------

# Flowchart vs Algorithm

  Flowchart                  Algorithm
  -------------------------- -------------------
  Visual representation      Written steps
  Uses symbols               Uses text
  Easier for visualization   Easier for coding

------------------------------------------------------------------------

# Flowchart vs UML

  Flowchart             UML
  --------------------- ------------------------
  Shows process logic   Shows software design
  Algorithm focused     System focused
  Simple workflow       Multiple diagram types

------------------------------------------------------------------------

# Advantages of Flowcharts

-   Easy understanding
-   Better communication
-   Helps debugging
-   Improves planning
-   Documents processes

------------------------------------------------------------------------

# Limitations of Flowcharts

-   Large systems become complex
-   Updating may be difficult
-   Not suitable for every design problem

------------------------------------------------------------------------

# Common Mistakes

## Mistake 1

Creating overly complex flowcharts.

Solution:

Break processes into smaller flows.

------------------------------------------------------------------------

## Mistake 2

Missing decision paths.

Solution:

Include all possible outcomes.

------------------------------------------------------------------------

## Mistake 3

Using incorrect symbols.

Solution:

Follow standard notation.

------------------------------------------------------------------------

# Best Practices

-   Keep flow direction clear
-   Use meaningful labels
-   Avoid unnecessary complexity
-   Validate with stakeholders
-   Update when logic changes

------------------------------------------------------------------------

# Industry Example

## Online Payment Process

``` text
Start

 ↓

Select Payment Method

 ↓

Enter Payment Details

 ↓

Validate Payment

 ↓

Payment Successful?

    /       \

  Yes        No

   ↓          ↓

Order Done  Retry

 ↓

End
```

------------------------------------------------------------------------

# Interview Questions

1.  What is a Flowchart?
2.  Why are flowcharts used?
3.  Explain common flowchart symbols.
4.  Difference between flowchart and algorithm?
5.  How are decisions represented?
6.  How are loops represented?
7.  Where are flowcharts used in software development?

------------------------------------------------------------------------

# Cheat Sheet

``` text
Flowchart

Start

 ↓

Input

 ↓

Process

 ↓

Decision

 ↓

Output

 ↓

End
```

------------------------------------------------------------------------

# Summary

Flowcharts provide a simple visual way to represent algorithms,
workflows, and processes. They help developers understand logic,
identify problems, and communicate ideas before implementation. Although
modern systems often use advanced modeling tools, flowcharts remain a
useful technique for explaining processes clearly.
