# Learner Guide - Designing and Implementing Microsoft DevOps Solutions (AZ-400)

## Course Overview

This learner guide supports practical AZ-400 training for learners who design and implement Microsoft DevOps solutions across Azure DevOps and GitHub. It focuses on continuous delivery of value through work tracking, collaboration, source control, automation, testing, deployment, security, compliance, monitoring, and feedback.

The current Microsoft study guide highlights these skill areas:

1. Design and implement processes and communications.
2. Design and implement a source control strategy.
3. Design and implement build and release pipelines.
4. Develop a security and compliance plan.
5. Implement an instrumentation strategy.

## Before You Start

### Recommended Lab Environment

Use one or more of the following:

- Azure DevOps organization and project.
- GitHub account and repository.
- Azure subscription or trainer-provided sandbox.
- Visual Studio Code.
- Git.
- Azure CLI.
- Bicep CLI.

### Safety and Cost Checklist

1. Use a training subscription where possible.
2. Do not store real secrets in repositories.
3. Use Key Vault, GitHub secrets, Azure Pipelines variables, or OIDC-based authentication.
4. Delete or stop billable resources after labs.
5. Review repository visibility before pushing code.
6. Avoid granting broad owner permissions to service principals.

### Lab Journal

For every lab, record:

- Repository URL or project name.
- Work items and traceability links.
- Branching and PR evidence.
- Pipeline YAML.
- Pipeline run results.
- Deployment target and evidence.
- Security findings and remediation.
- Monitoring queries and alerts.
- Lessons learned.

## Learning Outcomes

By the end of the course, you should be able to:

1. Design flow of work using Azure Boards or GitHub Issues.
2. Implement dashboards and DevOps metrics.
3. Configure collaboration and documentation with Markdown, wikis, and release notes.
4. Design branching, pull request, and repository governance strategies.
5. Build YAML CI pipelines with tests and artifacts.
6. Design release pipelines with approvals, environments, and deployment strategies.
7. Implement IaC with Bicep or ARM-style templates.
8. Secure pipelines with least privilege, service connections, Key Vault, and OIDC concepts.
9. Automate code, dependency, secret, and container scanning.
10. Configure Azure Monitor, Application Insights, alerts, and KQL queries.
11. Present an end-to-end DevOps design for an exam-style scenario.

## Course Flow

### Day 1

| Time | Activity |
| --- | --- |
| 09:00 | Course briefing, AZ-400 domains, account setup |
| 09:30 | Lab 01 - DevOps Processes, Boards, and Traceability |
| 11:30 | Lab 02 - Source Control, Branching, and Pull Requests |
| 14:00 | Lab 03 - YAML CI Pipelines, Testing, and Artifacts |
| 16:00 | Pipeline review and troubleshooting |

### Day 2

| Time | Activity |
| --- | --- |
| 09:00 | Day 1 recap |
| 09:30 | Lab 04 - Release Pipelines and Deployment Strategies |
| 11:30 | Lab 05 - Infrastructure as Code with Bicep and Templates |
| 14:00 | Lab 06 - DevSecOps, Secrets, and Compliance Scanning |
| 16:00 | Security and compliance review |

### Day 3

| Time | Activity |
| --- | --- |
| 09:00 | DevOps operations recap |
| 09:30 | Lab 07 - Instrumentation, Monitoring, KQL, and Feedback |
| 13:00 | Lab 08 - AZ-400 Capstone: End-to-End DevOps Solution |
| 16:00 | Final study plan and exam readiness checklist |

## Lab 01 Guide - DevOps Processes, Boards, and Traceability

### Objectives

- Create work tracking structure.
- Connect work to code and releases.
- Define DevOps metrics.
- Configure project documentation.

### Steps

1. Create or open an Azure DevOps project or GitHub repository.
2. Create epics, features, user stories, tasks, and bugs for a sample application.
3. Define a workflow for backlog, active work, review, testing, and done.
4. Create labels or tags for priority, risk, security, and release.
5. Link a user story to a branch, commit, and pull request.
6. Create a simple dashboard with work item counts and cycle-time-style notes.
7. Define metrics such as lead time, cycle time, deployment frequency, change failure rate, and mean time to recovery.
8. Create a Markdown project wiki or README with architecture, contribution, and release notes sections.
9. Add a Mermaid diagram for flow of work.
10. Document traceability from requirement to commit to deployment.

### Deliverables

- Work item hierarchy.
- Dashboard or metrics table.
- Markdown documentation.
- Traceability example.

### Checkpoint

You can show how a requirement flows from planning to code, pipeline, deployment, and feedback.

## Lab 02 Guide - Source Control, Branching, and Pull Requests

### Objectives

- Design a branch strategy.
- Configure pull request workflow.
- Apply repository permissions and tags.
- Practise Git recovery.

### Steps

1. Initialize or use a sample Git repository.
2. Compare trunk-based, feature branch, and release branch strategies.
3. Choose a strategy for the sample project and explain why.
4. Create a feature branch.
5. Make a small change and commit it.
6. Open a pull request.
7. Configure branch protection or branch policy where available.
8. Require review, status checks, and no direct pushes to main.
9. Add tags for release or milestone tracking.
10. Practise recovering a previous file version with Git.
11. Document how to remove sensitive data from history conceptually and when to escalate.

### Deliverables

- Branching strategy note.
- Pull request evidence.
- Branch policy screenshot or notes.
- Git recovery notes.

### Checkpoint

You can defend a source control strategy that balances speed, quality, and governance.

## Lab 03 Guide - YAML CI Pipelines, Testing, and Artifacts

### Objectives

- Create a YAML pipeline.
- Configure triggers and jobs.
- Run tests and publish artifacts.
- Review pipeline health.

### Steps

1. Create a simple sample application or use trainer-provided code.
2. Add a YAML pipeline file.
3. Configure trigger rules for main and pull requests.
4. Add build steps.
5. Add a unit test step.
6. Add a code coverage or test result publishing step where supported.
7. Publish a build artifact.
8. Use variables and reusable steps where practical.
9. Run the pipeline and inspect logs.
10. Fix one controlled pipeline failure.
11. Record duration, failure cause, and improvement opportunities.

### Deliverables

- YAML pipeline file.
- Successful pipeline run.
- Test/artifact evidence.
- Pipeline troubleshooting note.

### Checkpoint

You can explain how CI increases confidence before code is merged or released.

## Lab 04 Guide - Release Pipelines and Deployment Strategies

### Objectives

- Design deployment stages.
- Configure environments and approvals.
- Compare deployment strategies.
- Plan rollback and hotfix paths.

### Steps

1. Define environments such as dev, test, staging, and production.
2. Add deployment stages to the pipeline.
3. Configure approvals or checks for higher environments.
4. Compare blue-green, canary, ring, rolling, feature flags, and deployment slots.
5. Choose a deployment strategy for the sample app.
6. Add a manual approval or environment gate.
7. Deploy a sample artifact to a safe target or simulated environment.
8. Define rollback criteria and steps.
9. Define a hotfix branch and deployment path.
10. Create release notes from commits or PR descriptions.

### Deliverables

- Deployment strategy table.
- Multi-stage pipeline notes.
- Approval/check evidence.
- Rollback and hotfix plan.

### Checkpoint

You can choose a deployment strategy based on risk, downtime tolerance, and feedback needs.

## Lab 05 Guide - Infrastructure as Code with Bicep and Templates

### Objectives

- Define IaC strategy.
- Create a Bicep or ARM-style template.
- Validate and deploy infrastructure.
- Document parameters and drift.

### Steps

1. Identify infrastructure needed for the sample app.
2. Create a Bicep template for a simple Azure resource or use trainer-provided code.
3. Add parameters for environment and location.
4. Add naming and tagging standards.
5. Run template validation where available.
6. Deploy to a sandbox or review a simulated deployment.
7. Store the template in source control.
8. Add the template to a pipeline step.
9. Document how drift can occur.
10. Define how IaC changes should be reviewed and approved.

### Deliverables

- Bicep or template file.
- Parameter and tag notes.
- Validation or deployment evidence.
- IaC review strategy.

### Checkpoint

You can explain why infrastructure belongs in source control and pipelines.

## Lab 06 Guide - DevSecOps, Secrets, and Compliance Scanning

### Objectives

- Design secure authentication for pipelines.
- Manage secrets safely.
- Configure scanning workflows.
- Document compliance evidence.

### Steps

1. Identify all secrets used by the sample pipeline.
2. Move secrets to GitHub secrets, Azure Pipelines variables, or Key Vault.
3. Compare service principals, managed identities, and OIDC/workload identity federation.
4. Review Azure DevOps service connections or GitHub Actions authentication patterns.
5. Enable dependency scanning where available.
6. Enable secret scanning or add a secret scanning check.
7. Add CodeQL or static analysis conceptually or practically.
8. Review container scanning concepts if the sample app uses containers.
9. Create a security gate policy for critical findings.
10. Document security evidence for audit.

### Deliverables

- Secrets inventory.
- Secure authentication design.
- Scanning checklist.
- Compliance evidence table.

### Checkpoint

You can explain how DevSecOps controls prevent secrets leakage and reduce vulnerable deployments.

## Lab 07 Guide - Instrumentation, Monitoring, KQL, and Feedback

### Objectives

- Configure monitoring strategy.
- Review Application Insights and Azure Monitor concepts.
- Query logs with KQL.
- Create feedback loops.

### Steps

1. Identify telemetry needed for the sample application and pipeline.
2. Define application, infrastructure, pipeline, security, and operations metrics.
3. Configure or review Application Insights.
4. Configure or review Azure Monitor Logs.
5. Create alert rules conceptually or in a sandbox.
6. Review GitHub Actions or Azure Pipelines run history and failure rates.
7. Write simple KQL queries for logs or sample data.
8. Identify distributed tracing and performance investigation concepts.
9. Define feedback notifications to Teams, GitHub Issues, or Azure Boards.
10. Create an instrumentation strategy note.

### Deliverables

- Monitoring metric table.
- Alert design.
- KQL query examples.
- Feedback loop plan.

### Checkpoint

You can connect telemetry to operational decisions and continuous improvement.

## Lab 08 Guide - AZ-400 Capstone: End-to-End DevOps Solution

### Objectives

- Design an end-to-end DevOps solution.
- Combine process, source control, pipelines, security, and monitoring.
- Make tradeoff decisions.
- Build an exam study plan.

### Steps

1. Review a trainer-provided scenario with application, team, compliance, and deployment constraints.
2. Design flow of work using Boards or Issues.
3. Choose a branching and PR strategy.
4. Design CI pipeline stages.
5. Design release strategy and environment gates.
6. Add IaC and configuration management plan.
7. Add secrets, security scanning, and compliance evidence plan.
8. Add instrumentation, KQL, and alerting plan.
9. Identify risks and mitigations.
10. Create an executive summary and technical design notes.
11. Map weak areas to AZ-400 domains.
12. Write a 14-day study plan.

### Deliverables

- End-to-end architecture and flow diagram.
- DevOps solution design.
- Risk and mitigation table.
- Executive summary.
- Personal study plan.

### Checkpoint

You can explain how the complete DevOps design delivers secure, tested, monitored software with traceability.

## Final Readiness Checklist

Before finishing the course, confirm that you can:

- Design work tracking and traceability.
- Configure collaboration documentation.
- Design source control and PR policies.
- Create YAML CI pipelines.
- Publish tests, coverage, and artifacts.
- Design deployment strategies and rollback paths.
- Implement IaC and environment governance.
- Secure secrets and service connections.
- Configure security scanning and compliance gates.
- Define monitoring, alerts, and KQL queries.
- Present an end-to-end DevOps solution for a scenario.
