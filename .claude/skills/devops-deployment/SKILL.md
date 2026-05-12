---
name: devops-deployment
description: Use when working with deployment, CI/CD, Docker, containers, cloud configuration, environment variables, build pipelines, release workflows, infrastructure as code, monitoring, logging, rollback plans, or production readiness.
---

# DevOps Deployment

## Workflow

1. Inspect scripts, Dockerfiles, compose files, CI workflows, deployment config, and environment docs.
2. Identify build, test, package, migration, release, health check, and rollback steps.
3. Keep secrets out of source control and logs.
4. Prefer incremental deploy changes that can be verified independently.
5. Preserve compatibility with package manager, runtime version, and deployment target.

## Guidance

- Use deterministic dependency installation with lockfiles.
- Separate build-time and runtime configuration.
- Keep pipelines fast, explicit, and reproducible.
- Make required secrets and target environments clear.

## Verification

- Run local builds or container builds when possible.
- Validate CI YAML syntax and command availability.
- Provide deploy order, migration order, and rollback notes.
