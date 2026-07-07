# Lesson 175 --- Infrastructure as Code (Overview)

# Part 11 --- DevOps

> **Objective**
>
> Understand Infrastructure as Code (IaC), why it exists, problems with
> manual infrastructure management, IaC principles, declarative and
> imperative approaches, Terraform overview, cloud infrastructure
> automation, benefits, challenges, and its role in modern DevOps.

------------------------------------------------------------------------

# Introduction

Modern applications require infrastructure:

-   Servers
-   Networks
-   Databases
-   Storage
-   Security configurations

Traditionally, engineers created infrastructure manually.

This created problems.

``` text
Manual Setup

      ↓

Human Errors

      ↓

Inconsistent Infrastructure
```

Infrastructure as Code solves this problem.

------------------------------------------------------------------------

# What is Infrastructure as Code (IaC)?

**Infrastructure as Code (IaC)** is a DevOps practice where
infrastructure is created, configured, and managed using code instead of
manual processes.

Simple definition:

    Infrastructure + Code = IaC

------------------------------------------------------------------------

# Examples of Infrastructure

Infrastructure includes:

## Compute

Examples:

-   Virtual machines
-   Containers
-   Servers

------------------------------------------------------------------------

## Networking

Examples:

-   Virtual networks
-   Load balancers
-   Firewalls

------------------------------------------------------------------------

## Storage

Examples:

-   Databases
-   Object storage
-   File systems

------------------------------------------------------------------------

# Why Do We Need IaC?

Before IaC:

    Engineer Creates Server

            ↓

    Manual Configuration

            ↓

    Documentation

Problems:

-   Slow setup
-   Human mistakes
-   Difficult replication
-   Configuration drift

------------------------------------------------------------------------

# IaC Approach

With IaC:

    Infrastructure Code

            ↓

    Automation Tool

            ↓

    Cloud Infrastructure

The same infrastructure can be recreated anytime.

------------------------------------------------------------------------

# Principles of Infrastructure as Code

## 1. Automation

Infrastructure creation is automated.

------------------------------------------------------------------------

## 2. Version Control

Infrastructure code is stored like application code.

Example:

    Git Repository

          ↓

    Infrastructure Files

------------------------------------------------------------------------

## 3. Reproducibility

Same code creates the same infrastructure.

------------------------------------------------------------------------

## 4. Consistency

All environments can use the same definitions.

------------------------------------------------------------------------

## 5. Documentation Through Code

Code describes infrastructure clearly.

------------------------------------------------------------------------

# Manual Infrastructure vs IaC

  Manual Infrastructure   Infrastructure as Code
  ----------------------- ------------------------
  Human setup             Automated setup
  Error prone             Consistent
  Difficult replication   Easy recreation
  Poor tracking           Version controlled

------------------------------------------------------------------------

# Types of IaC Approaches

There are two main approaches:

1.  Declarative
2.  Imperative

------------------------------------------------------------------------

# 1. Declarative Approach

The user defines the desired final state.

Example:

    I need:

    3 servers

    Database

    Load Balancer

The tool decides how to create it.

------------------------------------------------------------------------

## Characteristics

-   Focuses on result
-   Automatically manages changes
-   Common in cloud tools

Example:

Terraform

------------------------------------------------------------------------

# 2. Imperative Approach

The user defines exact steps.

Example:

    Create Server

    Install Software

    Configure Network

    Start Service

------------------------------------------------------------------------

## Characteristics

-   Focuses on instructions
-   More control
-   More maintenance

Example:

Shell scripts

------------------------------------------------------------------------

# Declarative vs Imperative

  Declarative              Imperative
  ------------------------ -------------------------
  Defines desired state    Defines steps
  Tool decides execution   User controls execution
  Easier maintenance       More manual work

------------------------------------------------------------------------

# Infrastructure as Code Tools

Popular IaC tools:

-   Terraform
-   AWS CloudFormation
-   Pulumi
-   Ansible

------------------------------------------------------------------------

# Terraform Overview

Terraform is an open-source Infrastructure as Code tool created by
HashiCorp.

It allows users to define infrastructure using configuration files.

------------------------------------------------------------------------

# Terraform Workflow

Typical workflow:

    Write Configuration

            ↓

    terraform init

            ↓

    terraform plan

            ↓

    terraform apply

            ↓

    Infrastructure Created

------------------------------------------------------------------------

# Terraform Concepts

## Configuration File

Defines infrastructure.

Example:

    main.tf

------------------------------------------------------------------------

## Provider

Defines cloud platform.

Examples:

-   AWS
-   Azure
-   Google Cloud

------------------------------------------------------------------------

## Resource

Infrastructure component.

Examples:

-   VM
-   Database
-   Network

------------------------------------------------------------------------

# IaC in Cloud Computing

Cloud platforms use IaC to automate:

-   Server creation
-   Network setup
-   Storage configuration
-   Security rules

Example:

    Terraform Code

          ↓

    AWS Resources

------------------------------------------------------------------------

# IaC in CI/CD

Infrastructure can be deployed automatically.

Workflow:

    Developer

          ↓

    Git Repository

          ↓

    CI/CD Pipeline

          ↓

    Terraform

          ↓

    Cloud Infrastructure

------------------------------------------------------------------------

# Benefits of IaC

## Faster Deployment

Infrastructure can be created quickly.

------------------------------------------------------------------------

## Reduced Errors

Automation removes manual mistakes.

------------------------------------------------------------------------

## Better Consistency

Same configuration everywhere.

------------------------------------------------------------------------

## Easy Recovery

Infrastructure can be recreated.

------------------------------------------------------------------------

## Better Collaboration

Teams can review infrastructure changes.

------------------------------------------------------------------------

# Challenges of IaC

## 1. Learning Curve

Requires knowledge of tools and cloud platforms.

------------------------------------------------------------------------

## 2. State Management

Infrastructure state must be maintained.

------------------------------------------------------------------------

## 3. Security Risks

Incorrect code can create insecure infrastructure.

------------------------------------------------------------------------

## 4. Complexity

Large systems require careful management.

------------------------------------------------------------------------

# Infrastructure State

IaC tools track infrastructure state.

Example:

    Desired State

            vs

    Current State

Tools compare and update differences.

------------------------------------------------------------------------

# Real-World Example

## E-Commerce Platform

Need:

-   Web servers
-   Database
-   Load balancer

Without IaC:

    Manual Creation

    Hours Required

With IaC:

    Terraform Code

          ↓

    Automatic Infrastructure Creation

------------------------------------------------------------------------

# IaC Best Practices

-   Store infrastructure code in Git
-   Review infrastructure changes
-   Secure credentials
-   Use reusable modules
-   Automate deployments
-   Test infrastructure

------------------------------------------------------------------------

# Common IaC Problems

## Problem 1

Infrastructure mismatch.

Solution:

Use version-controlled IaC.

------------------------------------------------------------------------

## Problem 2

Security mistakes.

Solution:

Review and scan infrastructure code.

------------------------------------------------------------------------

## Problem 3

Manual changes outside IaC.

Solution:

Avoid configuration drift.

------------------------------------------------------------------------

# Interview Questions

## 1. What is Infrastructure as Code?

IaC is a DevOps practice where infrastructure is managed using code
instead of manual processes.

------------------------------------------------------------------------

## 2. Why is IaC important?

IaC provides automation, consistency, repeatability, and easier
infrastructure management.

------------------------------------------------------------------------

## 3. Difference between declarative and imperative IaC?

Declarative defines the desired state.

Imperative defines the exact steps.

------------------------------------------------------------------------

## 4. What is Terraform?

Terraform is an IaC tool used to create and manage cloud infrastructure
using configuration files.

------------------------------------------------------------------------

## 5. Benefits of IaC?

Benefits include:

-   Automation
-   Consistency
-   Version control
-   Faster deployment

------------------------------------------------------------------------

# Cheat Sheet

    Infrastructure as Code

    Write Code

          ↓

    Version Control

          ↓

    Automation Tool

          ↓

    Cloud Infrastructure

------------------------------------------------------------------------

# Summary

Infrastructure as Code allows organizations to manage infrastructure
using software development practices. By automating infrastructure
creation, maintaining version control, and ensuring consistency, IaC
improves reliability, scalability, and efficiency in modern DevOps
environments.
