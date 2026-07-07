# Lesson 181 --- DevOps Revision Notes

# Part 11 --- DevOps

> **Objective**
>
> Revise complete DevOps concepts including DevOps fundamentals, CI/CD,
> pipelines, deployment strategies, environment management,
> configuration management, Infrastructure as Code, monitoring, logging,
> incident management, tools, and interview-focused points.

------------------------------------------------------------------------

# 1. DevOps Overview

## What is DevOps?

DevOps combines:

    Development

    +

    Operations

    ↓

    DevOps

It is a culture and set of practices that improves software delivery
through:

-   Collaboration
-   Automation
-   Continuous delivery
-   Monitoring
-   Improvement

------------------------------------------------------------------------

# Why DevOps Exists

Before DevOps:

    Development

          X

    Operations

Problems:

-   Poor communication
-   Slow releases
-   Manual deployment
-   Environment issues
-   Production failures

DevOps solves these through:

-   Automation
-   Collaboration
-   Shared responsibility

------------------------------------------------------------------------

# 2. DevOps Lifecycle

Complete DevOps lifecycle:

    Plan

     ↓

    Code

     ↓

    Build

     ↓

    Test

     ↓

    Release

     ↓

    Deploy

     ↓

    Operate

     ↓

    Monitor

     ↓

    Improve

------------------------------------------------------------------------

# 3. Development vs Operations

## Development

Responsible for:

-   Writing code
-   Building features
-   Testing applications

------------------------------------------------------------------------

## Operations

Responsible for:

-   Infrastructure
-   Deployment
-   Monitoring
-   Reliability

------------------------------------------------------------------------

## DevOps Model

Both teams share responsibility for:

-   Quality
-   Deployment
-   Security
-   Reliability

------------------------------------------------------------------------

# 4. Continuous Integration (CI)

## Definition

CI is the practice of frequently integrating code changes and
automatically building and testing them.

------------------------------------------------------------------------

## CI Workflow

    Code Commit

     ↓

    Checkout

     ↓

    Build

     ↓

    Test

     ↓

    Feedback

------------------------------------------------------------------------

## CI Benefits

-   Early bug detection
-   Faster feedback
-   Better quality
-   Reduced conflicts

------------------------------------------------------------------------

## CI Tools

Examples:

-   Jenkins
-   GitHub Actions
-   GitLab CI/CD
-   CircleCI

------------------------------------------------------------------------

# 5. Continuous Delivery and Deployment

## Continuous Delivery

Software is always ready for release.

    Build

     ↓

    Test

     ↓

    Release Ready

------------------------------------------------------------------------

## Continuous Deployment

Software changes are automatically deployed.

    Build

     ↓

    Test

     ↓

    Production

------------------------------------------------------------------------

# CI vs CD

  CI                  CD
  ------------------- ------------------------
  Validates code      Delivers software
  Build and testing   Release and deployment

------------------------------------------------------------------------

# 6. Build Pipeline

## Purpose

Converts source code into software artifacts.

Workflow:

    Source Code

     ↓

    Dependencies

     ↓

    Build

     ↓

    Test

     ↓

    Artifact

------------------------------------------------------------------------

## Build Tools

Examples:

-   Maven
-   Gradle
-   npm
-   Make

------------------------------------------------------------------------

# 7. Release Pipeline

## Purpose

Moves artifacts into environments.

Workflow:

    Artifact

     ↓

    Development

     ↓

    Testing

     ↓

    Staging

     ↓

    Production

------------------------------------------------------------------------

# Build Pipeline vs Release Pipeline

  Build Pipeline     Release Pipeline
  ------------------ -------------------
  Creates artifact   Deploys artifact
  Code validation    Software delivery

------------------------------------------------------------------------

# 8. Deployment Strategies

Deployment strategies control how software is released.

------------------------------------------------------------------------

# Recreate Deployment

    Stop Old

     ↓

    Deploy New

Simple but causes downtime.

------------------------------------------------------------------------

# Rolling Deployment

Gradually replaces old versions.

Benefits:

-   Low downtime
-   Controlled release

------------------------------------------------------------------------

# Blue-Green Deployment

Two environments:

    Blue

    (Current)


    Green

    (New)

Traffic switches after validation.

------------------------------------------------------------------------

# Canary Deployment

Small user release first.

    5%

     ↓

    50%

     ↓

    100%

------------------------------------------------------------------------

# 9. Environment Management

## Environments

    Development

     ↓

    Testing

     ↓

    Staging

     ↓

    Production

------------------------------------------------------------------------

## Purpose

Provides:

-   Safe testing
-   Controlled releases
-   Reduced risk

------------------------------------------------------------------------

# 10. Configuration Management

## Definition

Managing application and infrastructure settings consistently.

Examples:

-   Database configuration
-   API keys
-   Environment values

------------------------------------------------------------------------

## Best Practices

-   Separate code and configuration
-   Protect secrets
-   Use automation
-   Version control configurations

------------------------------------------------------------------------

# 11. Infrastructure as Code (IaC)

## Definition

Managing infrastructure using code instead of manual setup.

    Infrastructure

    +

    Code

    =

    IaC

------------------------------------------------------------------------

## IaC Benefits

-   Automation
-   Consistency
-   Repeatability
-   Version control

------------------------------------------------------------------------

## IaC Tools

Examples:

-   Terraform
-   Ansible
-   AWS CloudFormation
-   Pulumi

------------------------------------------------------------------------

# Declarative vs Imperative

  Declarative              Imperative
  ------------------------ ------------------------
  Desired state            Steps
  Tool decides execution   User defines execution

------------------------------------------------------------------------

# 12. Monitoring

## Purpose

Observe system health and performance.

Monitors:

-   CPU
-   Memory
-   Response time
-   Errors
-   Availability

------------------------------------------------------------------------

# Four Golden Signals

1.  Latency

2.  Traffic

3.  Errors

4.  Saturation

------------------------------------------------------------------------

# Monitoring Tools

Examples:

-   Prometheus
-   Grafana
-   Datadog

------------------------------------------------------------------------

# 13. Logging

## Purpose

Records system events.

Used for:

-   Debugging
-   Security
-   Troubleshooting

------------------------------------------------------------------------

# Log Levels

    DEBUG

    INFO

    WARNING

    ERROR

    CRITICAL

------------------------------------------------------------------------

# ELK Stack

Components:

## Elasticsearch

Stores logs.

## Logstash

Processes logs.

## Kibana

Visualizes logs.

------------------------------------------------------------------------

# 14. Incident Management

## Definition

Process of handling system failures.

Lifecycle:

    Detect

     ↓

    Respond

     ↓

    Resolve

     ↓

    Analyze

     ↓

    Improve

------------------------------------------------------------------------

# Incident Metrics

## MTTR

Mean Time To Recovery

Measures recovery speed.

------------------------------------------------------------------------

## MTTD

Mean Time To Detect

Measures detection speed.

------------------------------------------------------------------------

## MTBF

Mean Time Between Failures

Measures reliability.

------------------------------------------------------------------------

# Root Cause Analysis

Find actual reason behind failure.

Methods:

-   Five Whys
-   Fishbone Diagram

------------------------------------------------------------------------

# 15. DevOps Tools Overview

  Category              Tools
  --------------------- -------------------------
  Version Control       Git, GitHub
  CI/CD                 Jenkins, GitHub Actions
  Containers            Docker, Kubernetes
  IaC                   Terraform, Ansible
  Monitoring            Prometheus, Grafana
  Logging               ELK Stack
  Cloud                 AWS, Azure, GCP
  Incident Management   PagerDuty, ServiceNow

------------------------------------------------------------------------

# 16. DevOps Interview Quick Revision

## What is DevOps?

DevOps combines development and operations to deliver software faster
and reliably.

------------------------------------------------------------------------

## Why CI?

To integrate and test code continuously.

------------------------------------------------------------------------

## Why CD?

To automate software delivery.

------------------------------------------------------------------------

## Why IaC?

To automate infrastructure management.

------------------------------------------------------------------------

## Why Monitoring?

To detect and solve issues quickly.

------------------------------------------------------------------------

## Why Logging?

To understand system behavior and troubleshoot problems.

------------------------------------------------------------------------

# Complete DevOps Workflow

    Developer

     ↓

    Git

     ↓

    CI Pipeline

     ↓

    Build

     ↓

    Test

     ↓

    Artifact

     ↓

    CD Pipeline

     ↓

    Deployment

     ↓

    Monitoring

     ↓

    Feedback

------------------------------------------------------------------------

# Final DevOps Checklist

✓ Understand DevOps culture

✓ Understand CI/CD

✓ Build pipelines

✓ Release pipelines

✓ Deployment strategies

✓ Environment management

✓ Configuration management

✓ Infrastructure as Code

✓ Monitoring

✓ Logging

✓ Incident management

✓ DevOps tools

✓ Real-world workflows

------------------------------------------------------------------------

# Summary

DevOps is a combination of culture, processes, and automation practices
that enable organizations to build, deploy, monitor, and improve
software continuously.

A successful DevOps engineer understands the complete software
lifecycle:

    Code

    ↓

    Build

    ↓

    Test

    ↓

    Deploy

    ↓

    Monitor

    ↓

    Improve

DevOps is not only about tools; it is about creating reliable systems
through collaboration, automation, and continuous improvement.
