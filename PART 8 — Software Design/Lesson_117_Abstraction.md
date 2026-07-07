# Lesson 117 --- Abstraction

# Part 8 --- Software Design

> **Objective**
>
> Understand Abstraction in software design, why hiding complexity is
> important, how abstraction works in Object-Oriented Programming,
> abstract classes, interfaces, benefits, and its relationship with good
> software design.

------------------------------------------------------------------------

# Introduction

Software systems are complex.

Users do not need to know every internal detail.

They only need a simple way to interact with the system.

This concept is called **Abstraction**.

``` text
Complex Internal Logic

          ↓

Simple Interface

          ↓

User Interaction
```

------------------------------------------------------------------------

# What is Abstraction?

**Abstraction** is the process of hiding unnecessary implementation
details and exposing only essential information.

It focuses on:

**What an object does**

rather than:

**How it does it**

------------------------------------------------------------------------

# Real-Life Example

## Car Driving

A driver uses:

-   Steering wheel
-   Accelerator
-   Brake

The driver does not need to know:

-   Engine combustion process
-   Fuel injection mechanism
-   Internal electronics

The car hides complexity.

This is abstraction.

------------------------------------------------------------------------

# Why Do We Need Abstraction?

Without abstraction:

``` text
User

 ↓

Complex Internal Details

 ↓

Difficulty of Use
```

Abstraction provides:

-   Simplicity
-   Better maintainability
-   Reduced complexity
-   Easier changes
-   Improved security

------------------------------------------------------------------------

# Abstraction in Software

Example:

Payment System

User sees:

    Pay(amount)

Internal system handles:

    Validate Payment

    Check Account

    Process Transaction

    Update Database

The user only interacts with the simple operation.

------------------------------------------------------------------------

# Abstraction in Object-Oriented Programming

OOP provides abstraction using:

1.  Abstract Classes

2.  Interfaces

------------------------------------------------------------------------

# 1. Abstract Class

An abstract class is a class that cannot be instantiated directly.

It can contain:

-   Abstract methods
-   Concrete methods

Example:

``` java
abstract class Payment {

    abstract void processPayment();

    void validate() {
        System.out.println("Validating");
    }
}
```

------------------------------------------------------------------------

# Abstract Method

A method without implementation.

Example:

``` java
abstract void makePayment();
```

The child class provides implementation.

------------------------------------------------------------------------

# Example

``` text
          Payment

             |
-----------------------

      |              |

Credit Card        UPI

Payment            Payment
```

Each payment type implements its own behavior.

------------------------------------------------------------------------

# 2. Interface

An interface defines a contract that classes must follow.

Example:

``` java
interface Payment {

    void pay();

}
```

Implementation:

``` java
class UPI implements Payment {

    public void pay(){

    }

}
```

------------------------------------------------------------------------

# Abstraction Example

## Notification System

Interface:

    Notification

            |
    -----------------

    Email

    SMS

    Push Notification

Each notification type follows the same contract.

------------------------------------------------------------------------

# Benefits of Abstraction

## 1. Reduces Complexity

Users interact with simple interfaces.

------------------------------------------------------------------------

## 2. Improves Maintainability

Internal implementation can change without affecting users.

Example:

Changing payment provider does not affect checkout flow.

------------------------------------------------------------------------

## 3. Supports Reusability

Common interfaces can support multiple implementations.

------------------------------------------------------------------------

## 4. Improves Security

Internal details remain hidden.

------------------------------------------------------------------------

# Abstraction and Encapsulation

Both hide details, but they focus on different things.

  Abstraction                Encapsulation
  -------------------------- ---------------------------
  Hides complexity           Hides data
  Focuses on design          Focuses on implementation
  Shows essential behavior   Protects internal state

Example:

Abstraction:

    ATM.withdraw()

Encapsulation:

    balance variable is private

------------------------------------------------------------------------

# Abstraction and Polymorphism

Abstraction enables multiple implementations.

Example:

    Payment Interface

            |

    ----------------

    UPI

    Card

    Wallet

Same operation:

    pay()

Different behavior.

------------------------------------------------------------------------

# Abstraction in Software Architecture

Architectural layers use abstraction.

Example:

``` text
User Interface Layer

        ↓

Business Layer

        ↓

Database Layer
```

The UI does not need to know database implementation details.

------------------------------------------------------------------------

# Industry Example

## E-Commerce Payment System

Abstraction:

    Payment Gateway Interface

                 |

    --------------------------------

    PayPal

    Stripe

    Bank Payment

The checkout system only calls:

    processPayment()

------------------------------------------------------------------------

# Common Mistakes

## Mistake 1

Creating unnecessary abstractions.

Solution:

Use abstraction only when needed.

------------------------------------------------------------------------

## Mistake 2

Making abstractions too complex.

Solution:

Keep interfaces simple.

------------------------------------------------------------------------

## Mistake 3

Confusing abstraction with encapsulation.

Solution:

Remember:

Abstraction = Hide complexity

Encapsulation = Hide data

------------------------------------------------------------------------

# Best Practices

-   Design interfaces around behavior
-   Hide implementation details
-   Keep abstractions simple
-   Use abstraction for flexibility
-   Avoid unnecessary layers

------------------------------------------------------------------------

# Interview Questions

1.  What is Abstraction?
2.  Why is abstraction important?
3.  Difference between abstraction and encapsulation?
4.  What is an abstract class?
5.  What is an interface?
6.  How does abstraction support polymorphism?
7.  Give a real-world abstraction example.

------------------------------------------------------------------------

# Cheat Sheet

``` text
Abstraction

Hide Complexity

        ↓

Expose Essential Behavior

        ↓

Simple Interaction

        ↓

Flexible Design
```

------------------------------------------------------------------------

# Summary

Abstraction is a fundamental software design principle that hides
unnecessary complexity and exposes only essential functionality. Through
abstract classes and interfaces, developers create flexible,
maintainable, and scalable systems where implementation details can
change without affecting users of the system.
