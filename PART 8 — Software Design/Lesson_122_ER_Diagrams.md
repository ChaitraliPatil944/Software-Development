# Lesson 122 --- ER Diagrams

# Part 8 --- Software Design

> **Objective**
>
> Understand Entity Relationship (ER) Diagrams, why database modeling is
> required, entities, attributes, relationships, cardinality, ER
> notation, and conversion of ER models into database schemas.

------------------------------------------------------------------------

# Introduction

Software applications store and manage large amounts of data.

Before creating database tables, developers need to understand:

-   What data is required?
-   How data is connected?
-   What relationships exist?

ER Diagrams help visualize database structure.

``` text
Business Requirements

        ↓

ER Diagram

        ↓

Database Tables

        ↓

Application
```

------------------------------------------------------------------------

# What is an ER Diagram?

An **Entity Relationship Diagram (ER Diagram)** is a visual
representation of database structure.

It shows:

-   Entities
-   Attributes
-   Relationships

It is used during database design.

------------------------------------------------------------------------

# Why Do We Need ER Diagrams?

Without proper database design:

``` text
Poor Data Design

        ↓

Duplicate Data

        ↓

Inconsistent Information

        ↓

Database Problems
```

ER diagrams help:

-   Design databases clearly
-   Identify relationships
-   Reduce redundancy
-   Improve data organization
-   Communicate database structure

------------------------------------------------------------------------

# Components of ER Diagram

An ER Diagram contains three main elements:

``` text
ER Model

   |
----------------
|       |      |
Entity Attribute Relationship
```

------------------------------------------------------------------------

# 1. Entity

An entity represents a real-world object or concept.

Examples:

-   Customer
-   Product
-   Employee
-   Order

Representation:

    +-----------+
    | Customer  |
    +-----------+

------------------------------------------------------------------------

# Types of Entities

## Strong Entity

Exists independently.

Example:

    Customer

------------------------------------------------------------------------

## Weak Entity

Depends on another entity.

Example:

    Order Item

    depends on

    Order

------------------------------------------------------------------------

# 2. Attributes

Attributes describe properties of an entity.

Example:

Entity:

    Customer

Attributes:

    Customer_ID

    Name

    Email

    Phone

------------------------------------------------------------------------

# Types of Attributes

## Simple Attribute

Cannot be divided.

Example:

    Age

------------------------------------------------------------------------

## Composite Attribute

Can be divided.

Example:

    Address

     |
     ----------------
     |
    City
    State
    Country

------------------------------------------------------------------------

## Multivalued Attribute

Can have multiple values.

Example:

    Phone Numbers

------------------------------------------------------------------------

## Derived Attribute

Calculated from another attribute.

Example:

    Age

    derived from

    Date of Birth

------------------------------------------------------------------------

# 3. Relationship

A relationship describes how entities interact.

Example:

    Customer

        places

    Order

------------------------------------------------------------------------

# Relationship Types

## One-to-One (1:1)

One entity relates to one entity.

Example:

    Person

       |

    Passport

------------------------------------------------------------------------

## One-to-Many (1:N)

One entity relates to many entities.

Example:

    Customer

        |

        |

    Orders

One customer can place many orders.

------------------------------------------------------------------------

## Many-to-Many (M:N)

Many entities relate to many entities.

Example:

    Student

        |

    Courses

A student can enroll in many courses.

A course can have many students.

------------------------------------------------------------------------

# Cardinality

Cardinality defines the number of relationships between entities.

Types:

    1:1

    1:N

    N:M

Example:

    Department

         1

         |

         |

        N

    Employees

One department has many employees.

------------------------------------------------------------------------

# ER Diagram Example

## Online Shopping System

Entities:

    Customer

    Product

    Order

    Payment

Relationships:

    Customer

        places

    Order


    Order

        contains

    Product


    Order

        has

    Payment

------------------------------------------------------------------------

# ER Diagram Representation

Example:

    +-------------+
    |  Customer   |
    +-------------+
    | customer_id |
    | name        |
    | email       |
    +-------------+

            |

          places

            |

    +-------------+
    |   Order     |
    +-------------+
    | order_id    |
    | date        |
    +-------------+

------------------------------------------------------------------------

# ER Diagram to Relational Schema

ER Model:

    Customer

       |

    Order

Converted Tables:

Customer Table:

    Customer

    customer_id PK

    name

    email

Order Table:

    Order

    order_id PK

    customer_id FK

    date

------------------------------------------------------------------------

# Primary Key and Foreign Key

## Primary Key

Uniquely identifies a record.

Example:

    Customer_ID

------------------------------------------------------------------------

## Foreign Key

Connects two tables.

Example:

    customer_id

inside Order table.

------------------------------------------------------------------------

# ER Diagram vs UML Class Diagram

  ER Diagram                     UML Class Diagram
  ------------------------------ -------------------------
  Database focused               Software design focused
  Entities and attributes        Classes and methods
  Relationships between tables   Object relationships

------------------------------------------------------------------------

# Industry Example

## Banking Database

Entities:

    Customer

    Account

    Transaction

    Loan

Relationships:

    Customer

    owns

    Account


    Account

    has

    Transaction

------------------------------------------------------------------------

# Common Mistakes

## Mistake 1

Ignoring relationships.

Solution:

Identify how entities interact.

------------------------------------------------------------------------

## Mistake 2

Creating duplicate attributes.

Solution:

Normalize data structure.

------------------------------------------------------------------------

## Mistake 3

Wrong cardinality.

Solution:

Analyze business rules carefully.

------------------------------------------------------------------------

# Best Practices

-   Identify entities clearly
-   Define primary keys
-   Use correct relationships
-   Avoid unnecessary duplication
-   Validate with business requirements

------------------------------------------------------------------------

# Interview Questions

1.  What is an ER Diagram?
2.  Why are ER diagrams used?
3.  What are entities and attributes?
4.  Explain relationship types.
5.  What is cardinality?
6.  Difference between ER Diagram and UML?
7.  How is ER model converted into tables?

------------------------------------------------------------------------

# Cheat Sheet

``` text
ER Diagram

Entity

   ↓

Attributes

   ↓

Relationships

   ↓

Database Schema
```

------------------------------------------------------------------------

# Summary

ER Diagrams provide a visual model of database design. They help
identify entities, attributes, relationships, and constraints before
implementation. A well-designed ER model reduces data problems and
creates a strong foundation for efficient database systems.
