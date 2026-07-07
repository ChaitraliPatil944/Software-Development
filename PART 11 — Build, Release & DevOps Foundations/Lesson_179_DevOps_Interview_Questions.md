# Lesson 179 --- DevOps Interview Questions

# Part 11 --- DevOps

> **Objective**
>
> Prepare for DevOps interviews by understanding frequently asked
> questions related to DevOps fundamentals, CI/CD, pipelines, deployment
> strategies, monitoring, logging, Infrastructure as Code, configuration
> management, and incident management.

------------------------------------------------------------------------

# Section 1 --- DevOps Fundamentals

## Q1. What is DevOps?

**Answer:**

DevOps is a culture, practice, and set of tools that combines
Development and Operations to improve software delivery through
collaboration, automation, continuous integration, continuous delivery,
and monitoring.

------------------------------------------------------------------------

## Q2. Why was DevOps introduced?

DevOps was introduced to solve problems between development and
operations teams:

-   Poor communication
-   Slow releases
-   Manual deployments
-   Deployment failures
-   Environment differences

------------------------------------------------------------------------

## Q3. Is DevOps a tool?

No.

DevOps is a combination of:

-   Culture
-   Processes
-   Automation
-   Tools

------------------------------------------------------------------------

## Q4. What are the main principles of DevOps?

Main principles:

-   Collaboration
-   Automation
-   Continuous Integration
-   Continuous Delivery
-   Monitoring
-   Continuous Improvement

------------------------------------------------------------------------

# Section 2 --- Development and Operations

## Q5. Difference between Development and Operations?

  Development        Operations
  ------------------ ------------------------
  Builds software    Runs software
  Writes code        Manages infrastructure
  Creates features   Maintains reliability

------------------------------------------------------------------------

## Q6. How does DevOps bridge the gap between Dev and Ops?

DevOps creates:

-   Shared responsibility
-   Better communication
-   Automated workflows
-   Collaborative teams

------------------------------------------------------------------------

# Section 3 --- Continuous Integration (CI)

## Q7. What is Continuous Integration?

Continuous Integration is a practice where developers frequently merge
code changes and automatically build and test them.

------------------------------------------------------------------------

## Q8. Why is CI important?

CI provides:

-   Early bug detection
-   Faster feedback
-   Better code quality
-   Reduced integration problems

------------------------------------------------------------------------

## Q9. Explain CI pipeline.

Typical CI pipeline:

    Code Commit

    ↓

    Checkout

    ↓

    Build

    ↓

    Test

    ↓

    Quality Check

    ↓

    Report

------------------------------------------------------------------------

## Q10. Name CI tools.

Examples:

-   Jenkins
-   GitHub Actions
-   GitLab CI/CD
-   CircleCI

------------------------------------------------------------------------

# Section 4 --- Continuous Delivery and Deployment

## Q11. What is Continuous Delivery?

Continuous Delivery keeps software ready for release after automated
validation.

------------------------------------------------------------------------

## Q12. What is Continuous Deployment?

Continuous Deployment automatically releases validated changes into
production.

------------------------------------------------------------------------

## Q13. Difference between Continuous Delivery and Continuous Deployment?

  Continuous Delivery        Continuous Deployment
  -------------------------- -------------------------
  Manual approval possible   Fully automated release
  Release ready              Automatically released

------------------------------------------------------------------------

# Section 5 --- Build and Release Pipeline

## Q14. What is a Build Pipeline?

A Build Pipeline converts source code into a tested software artifact.

Stages:

-   Checkout
-   Dependency installation
-   Compilation
-   Testing
-   Artifact creation

------------------------------------------------------------------------

## Q15. What is a Release Pipeline?

A Release Pipeline delivers software artifacts across environments and
manages deployment.

------------------------------------------------------------------------

## Q16. Difference between Build Pipeline and Release Pipeline?

Build Pipeline:

    Code → Artifact

Release Pipeline:

    Artifact → Production

------------------------------------------------------------------------

# Section 6 --- Deployment Strategies

## Q17. What are deployment strategies?

Deployment strategies define how new software versions are released into
production.

------------------------------------------------------------------------

## Q18. Explain Rolling Deployment.

Rolling deployment gradually replaces old application instances with new
ones.

Advantages:

-   Low downtime
-   Controlled release

------------------------------------------------------------------------

## Q19. Explain Blue-Green Deployment.

Two environments are maintained:

    Blue = Current Version

    Green = New Version

Traffic switches after validation.

------------------------------------------------------------------------

## Q20. Explain Canary Deployment.

A new version is released to a small percentage of users before full
deployment.

------------------------------------------------------------------------

# Section 7 --- Environment and Configuration Management

## Q21. What are software environments?

Software environments are setups required to run applications.

Examples:

-   Development
-   Testing
-   Staging
-   Production

------------------------------------------------------------------------

## Q22. Why are multiple environments required?

They provide:

-   Safe testing
-   Reduced production risk
-   Controlled releases

------------------------------------------------------------------------

## Q23. What is Configuration Management?

Configuration Management manages system and application settings
consistently.

------------------------------------------------------------------------

## Q24. Why should configuration be separated from code?

Benefits:

-   Security
-   Flexibility
-   Easier deployment

------------------------------------------------------------------------

# Section 8 --- Infrastructure as Code

## Q25. What is Infrastructure as Code?

IaC manages infrastructure using code instead of manual configuration.

------------------------------------------------------------------------

## Q26. Benefits of IaC?

Benefits:

-   Automation
-   Consistency
-   Version control
-   Reproducibility

------------------------------------------------------------------------

## Q27. Name IaC tools.

Examples:

-   Terraform
-   Ansible
-   AWS CloudFormation
-   Pulumi

------------------------------------------------------------------------

## Q28. Difference between Declarative and Imperative IaC?

Declarative:

Defines desired state.

Imperative:

Defines exact steps.

------------------------------------------------------------------------

# Section 9 --- Monitoring and Logging

## Q29. What is Monitoring?

Monitoring collects and analyzes system information to ensure
reliability and performance.

------------------------------------------------------------------------

## Q30. What are important monitoring metrics?

Examples:

-   Latency
-   Traffic
-   Errors
-   Saturation

------------------------------------------------------------------------

## Q31. Difference between Logs and Metrics?

  Logs              Metrics
  ----------------- -------------------
  Detailed events   Numerical values
  Explain events    Show system state

------------------------------------------------------------------------

## Q32. What is ELK Stack?

ELK consists of:

-   Elasticsearch
-   Logstash
-   Kibana

Used for log collection and analysis.

------------------------------------------------------------------------

# Section 10 --- Incident Management

## Q33. What is Incident Management?

Incident Management restores normal service after unexpected failures.

------------------------------------------------------------------------

## Q34. Explain incident lifecycle.

    Detection

    ↓

    Logging

    ↓

    Investigation

    ↓

    Resolution

    ↓

    Review

------------------------------------------------------------------------

## Q35. What is Root Cause Analysis?

RCA identifies the actual reason behind an incident.

------------------------------------------------------------------------

## Q36. What is MTTR?

MTTR means Mean Time To Recovery.

It measures how quickly systems recover after failure.

------------------------------------------------------------------------

# Section 11 --- Scenario-Based Questions

## Q37. Deployment failed in production. What will you do?

Answer:

1.  Check monitoring alerts
2.  Analyze logs
3.  Identify root cause
4.  Rollback if required
5.  Fix and redeploy

------------------------------------------------------------------------

## Q38. Application works locally but fails in production. Why?

Possible reasons:

-   Environment differences
-   Configuration issues
-   Dependency mismatch

Solutions:

-   Containerization
-   Configuration management

------------------------------------------------------------------------

## Q39. CI pipeline is failing. What will you check?

Steps:

1.  Check build logs
2.  Check dependencies
3.  Check test failures
4.  Fix issue
5.  Run pipeline again

------------------------------------------------------------------------

## Q40. Production server is down. How will you respond?

Steps:

1.  Create incident
2.  Assign owner
3.  Investigate
4.  Restore service
5.  Perform RCA

------------------------------------------------------------------------

# DevOps Tools Quick Revision

  Category              Tools
  --------------------- -------------------------
  Version Control       Git, GitHub
  CI/CD                 Jenkins, GitHub Actions
  Containers            Docker, Kubernetes
  IaC                   Terraform, Ansible
  Monitoring            Prometheus, Grafana
  Logging               ELK Stack
  Incident Management   PagerDuty, ServiceNow

------------------------------------------------------------------------

# Interview Tips

For DevOps answers:

1.  Explain concept
2.  Explain why it is needed
3.  Give workflow
4.  Provide real-world example

------------------------------------------------------------------------

# Final Revision

Important DevOps topics:

✓ DevOps fundamentals

✓ CI/CD

✓ Build pipeline

✓ Release pipeline

✓ Deployment strategies

✓ Environment management

✓ Configuration management

✓ Infrastructure as Code

✓ Monitoring

✓ Logging

✓ Incident management

------------------------------------------------------------------------

# Summary

DevOps interviews focus on understanding concepts, workflows, automation
practices, and real-world problem solving. A strong DevOps engineer
understands not only tools but also how development, deployment,
monitoring, and operations work together.
