# Lab 06 - DevSecOps, Secrets, and Compliance Scanning

## Objectives

- Manage secrets safely.
- Design secure pipeline authentication.
- Configure scanning checks.
- Document compliance evidence.

## Steps

1. Identify secrets used by the sample app or pipeline.
2. Move secrets to GitHub secrets, Azure Pipelines variables, or Key Vault.
3. Compare service principals, managed identities, and OIDC.
4. Review service connections or GitHub Actions authentication.
5. Enable dependency scanning where available.
6. Enable secret scanning or add a secret scanning step.
7. Add CodeQL or static analysis conceptually or practically.
8. Review container scanning concepts.
9. Define a policy for critical findings.
10. Create a compliance evidence table.

## Validation

- No secrets are stored in code.
- Authentication design follows least privilege.
- Scanning plan covers code, dependencies, secrets, and containers.
- Evidence table is audit-friendly.

## Review Questions

1. Why avoid long-lived secrets?
2. What is OIDC workload identity federation?
3. Why scan dependencies?
4. What should block a release?
