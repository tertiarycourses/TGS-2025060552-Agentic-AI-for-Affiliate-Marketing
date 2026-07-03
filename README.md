# TGS-2024042605 - Designing and Implementing Microsoft DevOps Solutions (AZ-400)

> Course: Designing and Implementing Microsoft DevOps Solutions (AZ-400)  
> Course Code: TGS-2024042605  
> Register here: https://www.tertiarycourses.com.sg/wsq-designing-and-implementing-microsoft-devops-solutions-az-400.html

Hands-on AZ-400 labs for learners designing and implementing Microsoft DevOps solutions. The labs cover work tracking, collaboration, GitHub Flow, Azure Boards, source control strategy, YAML pipelines, package management, testing, deployment strategies, infrastructure as code, secrets, compliance scanning, monitoring, telemetry, KQL, and exam-ready DevOps scenarios.

## Courseware

| File | Description |
| --- | --- |
| [Learner Guide](LG-Designing-and-Implementing-Microsoft-DevOps-Solutions-AZ-400.md) | Detailed step-by-step guide for the full course. |
| [Labs Index](labs/README.md) | Quick access to all hands-on labs. |
| [Tools Reference](labs/tools.md) | Free tools, command references, YAML snippets, and KQL examples used in the labs. |

## How to Use

1. Open the learner guide first and review the account, repository, and pipeline safety checklist.
2. Complete the labs in order because later labs reuse the repository, pipeline, IaC, secrets, and monitoring artifacts from earlier labs.
3. Use Azure DevOps, GitHub, Azure free/training subscription resources, or trainer-provided sandbox access.
4. Delete or disable billable cloud resources when the lab is complete.
5. Record repository settings, pipeline runs, deployment evidence, monitoring queries, and security findings in your lab journal.

## Lab Catalogue

### Processes, Communication, and Source Control

| Lab | Title | Skills Practised |
| --- | --- | --- |
| [Lab 01](labs/lab-01-devops-processes-boards-traceability.md) | DevOps Processes, Boards, and Traceability | Azure Boards, GitHub Issues, work items, dashboards, traceability, metrics |
| [Lab 02](labs/lab-02-source-control-branching-pull-requests.md) | Source Control, Branching, and Pull Requests | GitHub Flow, branch policies, PR reviews, tags, Git recovery |

### Pipelines, Delivery, and Infrastructure

| Lab | Title | Skills Practised |
| --- | --- | --- |
| [Lab 03](labs/lab-03-yaml-ci-pipelines-testing-artifacts.md) | YAML CI Pipelines, Testing, and Artifacts | GitHub Actions/Azure Pipelines, triggers, tests, coverage, artifacts |
| [Lab 04](labs/lab-04-release-pipelines-deployment-strategies.md) | Release Pipelines and Deployment Strategies | Environments, approvals, blue-green, canary, slots, rollback, feature flags |
| [Lab 05](labs/lab-05-infrastructure-as-code-bicep-templates.md) | Infrastructure as Code with Bicep and Templates | Bicep, ARM concepts, validation, deployment, parameters, drift notes |

### Security, Compliance, Monitoring, and Capstone

| Lab | Title | Skills Practised |
| --- | --- | --- |
| [Lab 06](labs/lab-06-devsecops-secrets-compliance-scanning.md) | DevSecOps, Secrets, and Compliance Scanning | Key Vault, OIDC, service connections, Dependabot, CodeQL, secret scanning |
| [Lab 07](labs/lab-07-instrumentation-monitoring-kql-feedback.md) | Instrumentation, Monitoring, KQL, and Feedback | Azure Monitor, Application Insights, alerts, pipeline health, KQL |
| [Lab 08](labs/lab-08-capstone-az400-end-to-end-devops.md) | AZ-400 Capstone: End-to-End DevOps Solution | Integrated scenario, design decisions, pipeline evidence, exam review |

## References

- Microsoft AZ-400 Study Guide: https://learn.microsoft.com/en-us/credentials/certifications/resources/study-guides/az-400
- Course registration: https://www.tertiarycourses.com.sg/wsq-designing-and-implementing-microsoft-devops-solutions-az-400.html
- Azure DevOps documentation: https://learn.microsoft.com/azure/devops/
- GitHub Actions documentation: https://docs.github.com/actions

## Free Tools Used

- Azure DevOps
- GitHub and GitHub Actions
- Azure CLI
- Visual Studio Code
- Git
- Bicep CLI
- Azure Monitor and Application Insights
- Kusto Query Language (KQL)
