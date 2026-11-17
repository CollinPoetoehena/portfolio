# Cloud-native Car Rental Platform

A cloud-native car rental platform built with Node.js, Next.js, MongoDB, Docker, and AWS Cognito. Terraform provisions its infrastructure, and GitHub Actions automates CI/CD. This profile is based on the project description; no source repository or project documentation was available to verify its feature set, deployment status, or infrastructure topology.

## Main techniques and lessons

- **Application and infrastructure as code**: The application stack and Terraform-managed infrastructure provide separate, explicit areas to develop and maintain.
- **Containerized delivery**: Docker and GitHub Actions support a repeatable path from application changes through build and deployment automation.
- **Identity as a platform concern**: AWS Cognito places authentication alongside the application rather than treating identity as an ad hoc feature.
- **Likely lesson (inferred)**: Cloud scalability depends on how application behavior, data, identity, and infrastructure fit together; using cloud tools alone does not establish that a system scales.

These lessons are inferred from the described technology choices and are not independently verified project findings.

## High-level organization

The tree is a conceptual view based on the project description, not a verified source layout.

```text
Cloud-native car rental platform
├── Application
│   ├── Node.js and Next.js
│   └── MongoDB
├── Identity
│   └── AWS Cognito
└── Cloud delivery
    ├── Docker
    ├── Terraform infrastructure
    └── GitHub Actions CI/CD
```
