# Lesson 176 --- Monitoring Basics

# Part 11 --- DevOps

> **Objective**
>
> Understand monitoring fundamentals, why monitoring is required,
> application monitoring, infrastructure monitoring, metrics, logs,
> alerts, health checks, observability basics, monitoring tools, and how
> DevOps teams use monitoring in production systems.

------------------------------------------------------------------------

# Introduction

Deploying software is not the end of software delivery.

After deployment, teams need to know:

-   Is the application working?
-   Are users facing problems?
-   Is infrastructure healthy?

Monitoring provides visibility into system behavior.

``` text
Application

      ↓

Monitoring

      ↓

Insights

      ↓

Actions
```

------------------------------------------------------------------------

# What is Monitoring?

**Monitoring** is the process of collecting, analyzing, and observing
information about applications, systems, and infrastructure to ensure
they are working correctly.

Monitoring helps identify:

-   Failures
-   Performance issues
-   Security problems
-   Availability issues

------------------------------------------------------------------------

# Why Do We Need Monitoring?

Without monitoring:

    Production Issue

            ↓

    Users Report Problem

            ↓

    Team Investigates

Problems:

-   Slow detection
-   Longer downtime
-   Poor user experience

------------------------------------------------------------------------

# With Monitoring

    System Issue

          ↓

    Monitoring Detects

          ↓

    Alert Generated

          ↓

    Team Responds

------------------------------------------------------------------------

# Goals of Monitoring

Monitoring helps achieve:

-   High availability
-   Faster problem detection
-   Better performance
-   Improved reliability
-   Data-driven decisions

------------------------------------------------------------------------

# Types of Monitoring

Main categories:

1.  Infrastructure Monitoring
2.  Application Monitoring
3.  Network Monitoring
4.  Security Monitoring
5.  Database Monitoring

------------------------------------------------------------------------

# 1. Infrastructure Monitoring

Focuses on hardware and system resources.

Monitors:

-   CPU usage
-   Memory usage
-   Disk space
-   Server health
-   Network activity

Example:

    CPU Usage = 95%

          ↓

    Warning Alert

------------------------------------------------------------------------

# 2. Application Monitoring

Focuses on application behavior.

Monitors:

-   Response time
-   Errors
-   Requests
-   Application availability

Example:

    API Response Time

    Normal: 200ms

    Current: 5 seconds

          ↓

    Alert

------------------------------------------------------------------------

# 3. Network Monitoring

Tracks:

-   Network traffic
-   Latency
-   Connectivity
-   Bandwidth usage

------------------------------------------------------------------------

# 4. Security Monitoring

Detects:

-   Unauthorized access
-   Suspicious activity
-   Security threats

------------------------------------------------------------------------

# 5. Database Monitoring

Tracks:

-   Query performance
-   Connections
-   Storage usage
-   Database errors

------------------------------------------------------------------------

# Monitoring Metrics

Metrics are measurable values that describe system behavior.

Examples:

-   CPU percentage
-   Memory usage
-   Request count
-   Error rate
-   Response time

------------------------------------------------------------------------

# Important Application Metrics

## 1. Response Time

Time taken to process a request.

Example:

    API Request

          ↓

    200 milliseconds

------------------------------------------------------------------------

## 2. Error Rate

Percentage of failed requests.

Example:

    1000 Requests

    50 Failures

    Error Rate = 5%

------------------------------------------------------------------------

## 3. Throughput

Number of requests processed.

Example:

    Requests per second

------------------------------------------------------------------------

## 4. Availability

System uptime percentage.

Example:

    99.9% Availability

------------------------------------------------------------------------

# Four Golden Signals

Google introduced four important monitoring signals:

## 1. Latency

Time taken to respond.

------------------------------------------------------------------------

## 2. Traffic

Amount of requests.

------------------------------------------------------------------------

## 3. Errors

Failed requests.

------------------------------------------------------------------------

## 4. Saturation

Resource usage level.

Example:

CPU or memory pressure.

------------------------------------------------------------------------

# Logs vs Metrics

  Logs                    Metrics
  ----------------------- -------------------
  Detailed events         Numerical values
  Explain what happened   Show system state
  Text-based              Data points

Example:

Log:

    Database connection failed

Metric:

    Error count = 50

------------------------------------------------------------------------

# Alerts

An alert notifies teams when problems occur.

Example:

    CPU > 90%

          ↓

    Send Alert

------------------------------------------------------------------------

# Types of Alerts

## Warning Alert

Indicates potential issues.

Example:

    Memory Usage 80%

------------------------------------------------------------------------

## Critical Alert

Requires immediate action.

Example:

    Server Down

------------------------------------------------------------------------

# Health Checks

Health checks verify whether systems are working.

Example:

    Application

          ↓

    /health endpoint

          ↓

    Status: OK

------------------------------------------------------------------------

# Monitoring vs Observability

Monitoring tells:

    Is something wrong?

Observability helps answer:

    Why is it wrong?

------------------------------------------------------------------------

# Observability Pillars

Three main pillars:

## 1. Metrics

Numerical measurements.

Example:

    CPU = 80%

------------------------------------------------------------------------

## 2. Logs

Detailed event records.

Example:

    User login failed

------------------------------------------------------------------------

## 3. Traces

Track requests across services.

Example:

    User Request

     ↓

    API Service

     ↓

    Database

     ↓

    Response

------------------------------------------------------------------------

# Monitoring Tools

## Prometheus

Used for:

-   Metrics collection
-   Alerting

------------------------------------------------------------------------

## Grafana

Used for:

-   Dashboards
-   Visualization

------------------------------------------------------------------------

## ELK Stack

Includes:

-   Elasticsearch
-   Logstash
-   Kibana

Used for log analysis.

------------------------------------------------------------------------

## Datadog

Cloud monitoring platform.

------------------------------------------------------------------------

# Monitoring Workflow

    Application

          ↓

    Collect Data

          ↓

    Analyze Metrics

          ↓

    Generate Alerts

          ↓

    Take Action

------------------------------------------------------------------------

# Monitoring in DevOps

Monitoring completes the DevOps lifecycle.

    Plan

     ↓

    Code

     ↓

    Build

     ↓

    Deploy

     ↓

    Monitor

     ↓

    Improve

------------------------------------------------------------------------

# Real-World Example

## Banking Application

Monitoring checks:

    Transaction API

    Database

    Server Health

    Security Events

If failure occurs:

    Alert

     ↓

    Engineer Investigation

     ↓

    Fix Issue

------------------------------------------------------------------------

# Monitoring Best Practices

-   Monitor critical systems
-   Set meaningful alerts
-   Avoid alert overload
-   Track important metrics
-   Maintain dashboards
-   Review monitoring data regularly

------------------------------------------------------------------------

# Common Monitoring Problems

## Problem 1

Too many alerts.

Solution:

Configure meaningful thresholds.

------------------------------------------------------------------------

## Problem 2

Missing important metrics.

Solution:

Define business and technical metrics.

------------------------------------------------------------------------

## Problem 3

No response process.

Solution:

Create incident management procedures.

------------------------------------------------------------------------

# Interview Questions

## 1. What is monitoring?

Monitoring is the process of collecting and analyzing system information
to ensure reliability and performance.

------------------------------------------------------------------------

## 2. Why is monitoring important in DevOps?

It helps detect issues quickly and improves system reliability.

------------------------------------------------------------------------

## 3. Difference between logs and metrics?

Logs provide detailed events.

Metrics provide numerical measurements.

------------------------------------------------------------------------

## 4. What are the four golden signals?

-   Latency
-   Traffic
-   Errors
-   Saturation

------------------------------------------------------------------------

## 5. Difference between monitoring and observability?

Monitoring detects problems.

Observability helps understand the cause.

------------------------------------------------------------------------

# Cheat Sheet

    Monitoring

    Collect Data

          ↓

    Metrics

          ↓

    Logs

          ↓

    Alerts

          ↓

    Response

          ↓

    Improvement

------------------------------------------------------------------------

# Summary

Monitoring is a critical DevOps practice that provides visibility into
applications and infrastructure after deployment. By collecting metrics,
logs, and traces, teams can detect problems early, improve reliability,
and maintain high-quality software systems.

Monitoring is the bridge between deployment and continuous improvement.
