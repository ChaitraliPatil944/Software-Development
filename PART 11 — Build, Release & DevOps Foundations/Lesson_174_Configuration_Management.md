# Lesson 174 --- Configuration Management

# Part 11 --- DevOps

> **Objective**
>
> Understand Configuration Management, why it is needed, configuration
> vs code, configuration files, environment variables, secrets
> management, configuration automation tools, best practices, and its
> role in DevOps workflows.

------------------------------------------------------------------------

# Introduction

Applications depend on many settings to run correctly.

Examples:

-   Database connections
-   Server settings
-   API keys
-   Application behavior

These settings are called **configuration**.

Managing them properly is essential in DevOps.

``` text
Application Code

        +

Configuration

        ↓

Running Application
```

------------------------------------------------------------------------

# What is Configuration Management?

**Configuration Management** is the process of managing, organizing,
storing, and maintaining application and infrastructure configurations.

It ensures systems are:

-   Consistent
-   Reliable
-   Reproducible
-   Easy to update

------------------------------------------------------------------------

# Why Do We Need Configuration Management?

Without proper management:

    Manual Configuration

            ↓

    Different Environments

            ↓

    Application Failures

Problems:

-   Configuration errors
-   Security risks
-   Difficult deployments
-   Environment differences

------------------------------------------------------------------------

# Configuration vs Code

Code defines application behavior.

Example:

    Login Function

    Payment API

    User Management

Configuration defines application settings.

Example:

    Database URL

    Port Number

    API Keys

    Environment Settings

------------------------------------------------------------------------

# Code vs Configuration

  Code                      Configuration
  ------------------------- ----------------------
  Application logic         Application settings
  Changes less frequently   Changes frequently
  Written by developers     Managed by teams
  Compiled/package          Loaded at runtime

------------------------------------------------------------------------

# Examples of Configuration

## Database Configuration

Example:

    DATABASE_HOST=server.com

    DATABASE_PORT=3306

------------------------------------------------------------------------

## Application Configuration

Example:

    SERVER_PORT=8080

    DEBUG_MODE=false

------------------------------------------------------------------------

## External Service Configuration

Example:

    PAYMENT_API_URL

    EMAIL_SERVICE_KEY

------------------------------------------------------------------------

# Configuration Files

Applications often store settings in files.

Common formats:

## JSON

Example:

``` json
{
 "server": "localhost",
 "port": 8080
}
```

------------------------------------------------------------------------

## YAML

Example:

``` yaml
server:
  port: 8080
```

------------------------------------------------------------------------

## Properties Files

Example:

    database.url=value

------------------------------------------------------------------------

# Environment Variables

Environment variables store configuration outside application code.

Example:

    DATABASE_PASSWORD

            ↓

    Environment Variable

            ↓

    Application

------------------------------------------------------------------------

# Why Use Environment Variables?

Benefits:

-   Security
-   Environment flexibility
-   Easier deployment

Example:

Development:

    DATABASE=local_db

Production:

    DATABASE=cloud_db

Same code, different configuration.

------------------------------------------------------------------------

# Secrets Management

Some configurations are sensitive.

Examples:

-   Passwords
-   API keys
-   Access tokens
-   Certificates

These should not be stored in code.

Bad:

``` python
password="admin123"
```

Good:

    PASSWORD

            ↓

    Secret Manager

------------------------------------------------------------------------

# Secret Management Tools

Examples:

## HashiCorp Vault

Used for:

-   Secret storage
-   Access control

------------------------------------------------------------------------

## AWS Secrets Manager

Cloud-based secret management.

------------------------------------------------------------------------

## Kubernetes Secrets

Used for container environments.

------------------------------------------------------------------------

# Configuration Management Tools

Configuration management tools automate system setup.

------------------------------------------------------------------------

# 1. Ansible

Ansible automates:

-   Server configuration
-   Software installation
-   Deployment tasks

Example:

    New Server

          ↓

    Ansible Playbook

          ↓

    Configured Server

------------------------------------------------------------------------

# 2. Puppet

Used for:

-   Infrastructure configuration
-   System management

------------------------------------------------------------------------

# 3. Chef

Uses code-based configuration management.

------------------------------------------------------------------------

# 4. Terraform

Used mainly for infrastructure provisioning.

Example:

    Infrastructure Code

          ↓

    Cloud Resources

------------------------------------------------------------------------

# Configuration Management Workflow

Typical process:

    Create Configuration

            ↓

    Store in Version Control

            ↓

    Apply Automatically

            ↓

    Deploy Application

            ↓

    Monitor

------------------------------------------------------------------------

# Configuration Management in CI/CD

CI/CD pipelines use configuration management.

Example:

    Code

     ↓

    Build

     ↓

    Load Configuration

     ↓

    Deploy

     ↓

    Run Application

------------------------------------------------------------------------

# Configuration Drift

Configuration drift occurs when systems become different over time.

Example:

Server A:

    Java 17

Server B:

    Java 11

Result:

    Different Behavior

------------------------------------------------------------------------

# Preventing Configuration Drift

Solutions:

-   Infrastructure as Code
-   Automation
-   Version-controlled configuration
-   Regular audits

------------------------------------------------------------------------

# Configuration Management Best Practices

## 1. Separate Code and Configuration

Keep settings outside application code.

------------------------------------------------------------------------

## 2. Version Control Configuration

Track changes.

------------------------------------------------------------------------

## 3. Protect Secrets

Never commit passwords or keys.

------------------------------------------------------------------------

## 4. Automate Configuration

Avoid manual setup.

------------------------------------------------------------------------

## 5. Document Configurations

Maintain clear documentation.

------------------------------------------------------------------------

# Real-World Example

## E-Commerce Application

Configuration:

    Development

    Database = Local


    Testing

    Database = Test Server


    Production

    Database = Cloud Database

Same application, different configurations.

------------------------------------------------------------------------

# Common Configuration Problems

## Problem 1

Secret accidentally committed.

Solution:

Use secret management tools.

------------------------------------------------------------------------

## Problem 2

Different server configurations.

Solution:

Use automation tools.

------------------------------------------------------------------------

## Problem 3

Manual configuration mistakes.

Solution:

Use Infrastructure as Code.

------------------------------------------------------------------------

# Interview Questions

## 1. What is Configuration Management?

Configuration Management manages application and infrastructure settings
to maintain consistency and reliability.

------------------------------------------------------------------------

## 2. Difference between code and configuration?

Code defines application logic.

Configuration defines application settings.

------------------------------------------------------------------------

## 3. Why should secrets not be stored in code?

Because they create security risks.

------------------------------------------------------------------------

## 4. What are environment variables?

External variables used to provide configuration values to applications.

------------------------------------------------------------------------

## 5. Name configuration management tools.

Examples:

-   Ansible
-   Puppet
-   Chef
-   Terraform

------------------------------------------------------------------------

# Cheat Sheet

    Configuration Management

    Code

     +

    Settings

     +

    Automation

          ↓

    Consistent Systems

------------------------------------------------------------------------

# Summary

Configuration Management is a fundamental DevOps practice that ensures
applications and infrastructure are configured consistently across
environments. By separating configuration from code, managing secrets
securely, and automating setup, organizations achieve reliable and
repeatable software delivery.
