# Tools Reference

## Tools

| Tool | Use |
| --- | --- |
| Azure DevOps | Boards, Repos, Pipelines, Artifacts, service connections. |
| GitHub | Repositories, Issues, Projects, Actions, branch protection, security features. |
| Visual Studio Code | YAML, Markdown, Bicep, Git workflows. |
| Git | Source control, branching, tags, recovery. |
| Azure CLI | Azure authentication and resource deployment. |
| Bicep CLI | Infrastructure as code authoring and validation. |
| Azure Monitor | Metrics, logs, alerts, dashboards. |
| Application Insights | Application telemetry and distributed tracing. |

## Git Commands

```bash
git status
git branch
git checkout -b feature/demo
git add .
git commit -m "Update sample"
git log --oneline
git tag v1.0.0
git restore --source HEAD~1 -- path/to/file
```

## YAML Pipeline Snippet

```yaml
trigger:
  branches:
    include:
      - main

jobs:
- job: build
  steps:
  - script: echo "Run build"
  - script: echo "Run tests"
```

## KQL Examples

```kusto
requests
| summarize count() by resultCode

traces
| where severityLevel >= 2
| order by timestamp desc
```
