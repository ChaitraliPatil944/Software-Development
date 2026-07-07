# Lesson 118 --- Encapsulation

# Part 8 --- Software Design

> **Objective**
>
> Understand Encapsulation in software design, why data hiding is
> important, how access control works, encapsulation in Object-Oriented
> Programming, benefits, and its role in building secure and
> maintainable software systems.

------------------------------------------------------------------------

# Introduction

Software objects contain:

-   Data
-   Behavior

A good design should protect internal data from unwanted access.

This concept is called **Encapsulation**.

``` text
Data

 +

Methods

      ↓

Encapsulated Object
```

------------------------------------------------------------------------

# What is Encapsulation?

**Encapsulation** is the process of bundling data and methods together
inside a single unit and restricting direct access to internal details.

It focuses on:

**How data is protected and controlled**

------------------------------------------------------------------------

# Real-Life Example

## Bank Account

A customer cannot directly modify:

    balance = 100000

Instead, the customer uses:

    deposit()

    withdraw()

The bank controls how balance changes.

This is encapsulation.

------------------------------------------------------------------------

# Why Do We Need Encapsulation?

Without encapsulation:

``` text
Direct Data Access

        ↓

Incorrect Changes

        ↓

Data Inconsistency
```

Encapsulation provides:

-   Data security
-   Controlled access
-   Better maintainability
-   Reduced complexity
-   Improved reliability

------------------------------------------------------------------------

# Encapsulation in Object-Oriented Programming

Encapsulation is achieved using:

-   Classes
-   Access modifiers
-   Getter methods
-   Setter methods

------------------------------------------------------------------------

# Class as an Encapsulation Unit

A class combines:

``` text
Class

├── Data Members

└── Methods
```

Example:

``` java
class BankAccount {

    private double balance;

    public void deposit(double amount){

        balance += amount;

    }

}
```

The balance cannot be directly modified.

------------------------------------------------------------------------

# Data Hiding

Data hiding means restricting direct access to internal data.

Example:

``` java
private password;
```

Only controlled methods can access it.

------------------------------------------------------------------------

# Access Modifiers

Access modifiers control visibility.

## 1. Private

Accessible only inside the class.

Example:

``` java
private int balance;
```

------------------------------------------------------------------------

## 2. Public

Accessible from anywhere.

Example:

``` java
public void login()
```

------------------------------------------------------------------------

## 3. Protected

Accessible within class and subclasses.

------------------------------------------------------------------------

## 4. Default

Accessible within the same package.

------------------------------------------------------------------------

# Getter and Setter Methods

Getters read data.

Setters modify data.

Example:

``` java
class Student {

private String name;


public String getName(){

return name;

}


public void setName(String name){

this.name = name;

}

}
```

------------------------------------------------------------------------

# Encapsulation Example

## User Account System

Without encapsulation:

    User

    password = "12345"

Anyone can modify it.

------------------------------------------------------------------------

With encapsulation:

    User Class

    private password

           ↓

    validatePassword()

Access is controlled.

------------------------------------------------------------------------

# Benefits of Encapsulation

## 1. Data Security

Protects sensitive information.

Example:

-   Passwords
-   Bank balance
-   Personal data

------------------------------------------------------------------------

## 2. Controlled Access

Changes happen through defined methods.

------------------------------------------------------------------------

## 3. Maintainability

Internal implementation can change without affecting external code.

------------------------------------------------------------------------

## 4. Flexibility

Validation rules can be added easily.

Example:

``` text
withdraw(amount)

checks:

- sufficient balance
- transaction limit
```

------------------------------------------------------------------------

# Encapsulation and Abstraction

Both hide details but have different purposes.

  Encapsulation              Abstraction
  -------------------------- --------------------------
  Hides data                 Hides complexity
  Protects internal state    Shows essential behavior
  Implementation technique   Design concept

Example:

ATM:

Abstraction:

    withdraw()

Encapsulation:

    private accountBalance

------------------------------------------------------------------------

# Encapsulation and Modularity

Encapsulation supports modular design.

Example:

    Payment Module

    private transaction details

    public processPayment()

Other modules use the interface without accessing internal data.

------------------------------------------------------------------------

# Industry Example

## E-Commerce Application

Product class:

    Product

    private price

    private inventory

Methods:

    updatePrice()

    checkAvailability()

Rules are controlled inside the object.

------------------------------------------------------------------------

# Common Mistakes

## Mistake 1

Making all variables public.

Problem:

Anyone can modify data.

Solution:

Keep fields private.

------------------------------------------------------------------------

## Mistake 2

Creating unnecessary getters and setters.

Solution:

Expose only required operations.

------------------------------------------------------------------------

## Mistake 3

Putting too much logic inside setters.

Solution:

Keep responsibilities clear.

------------------------------------------------------------------------

# Best Practices

-   Keep data private
-   Expose meaningful methods
-   Validate input before updating data
-   Hide implementation details
-   Follow single responsibility principle

------------------------------------------------------------------------

# Interview Questions

1.  What is Encapsulation?
2.  Why is encapsulation important?
3.  Explain data hiding.
4.  How is encapsulation achieved in Java?
5.  Difference between abstraction and encapsulation?
6.  What are access modifiers?
7.  Give a real-world example of encapsulation.

------------------------------------------------------------------------

# Cheat Sheet

``` text
Encapsulation

Bundle

Data + Methods

        ↓

Hide Internal Data

        ↓

Controlled Access

        ↓

Secure Object
```

------------------------------------------------------------------------

# Summary

Encapsulation is a core Object-Oriented Programming principle that
combines data and methods while protecting internal details from direct
access. By using classes, access modifiers, and controlled methods,
encapsulation improves security, maintainability, and reliability of
software systems.
