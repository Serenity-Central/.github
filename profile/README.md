<div align="center">

# Serenity

### A safer space to breathe.

**The Serenity Project Mental Health CIC**

Building safer, calmer and more human digital spaces for mental health support.

[![Website](https://img.shields.io/badge/Website-serenitycentral.cloud-7656A8?style=for-the-badge)](https://serenitycentral.cloud)
[![Public Beta](https://img.shields.io/badge/Public_Beta-Live-4F8A8B?style=for-the-badge)](https://serenitycentral.cloud)
[![Status](https://img.shields.io/badge/Status-Active_Development-2E7D32?style=for-the-badge)](#current-roadmap)

</div>

## About Serenity

**The Serenity Project Mental Health CIC** is a UK-registered Community Interest Company (CIC), limited by shares, dedicated to creating accessible digital mental health support built around safety, privacy and genuine human connection.

Our mission is to make emotional support, reliable information and meaningful human connection more accessible through thoughtfully designed digital services.

We believe that everyone deserves somewhere they can express themselves, explore their feelings and seek support without judgement.

Serenity is not a crisis service or a replacement for professional healthcare. Our community services are designed to complement existing support systems, while our longer-term development includes dedicated therapeutic services delivered by appropriately qualified professionals.

## Our platform

Serenity has launched its public beta, introducing the first generation of our digital mental health platform.

### Serenity Central

Our central digital platform brings together community support, mental health information and accessible resources in one environment.

Designed with accessibility, privacy and safeguarding in mind, Serenity Central provides the foundation for our expanding ecosystem of services.

### Anonymous venting

A moderated space where people can express difficult thoughts, emotions and experiences without unnecessary pressure to disclose their identity.

The service incorporates privacy-conscious identities, community interactions, moderation controls and safeguarding workflows.

Users can share experiences, respond supportively and engage with others while retaining control over how they participate.

### Serenity Hubs

A growing collection of structured mental health resources and educational content.

Serenity Hubs aim to make reliable information easier to discover, understand and navigate, helping users explore topics relevant to their wellbeing.

### Guides & Tools

Practical resources designed to help people understand mental health, explore coping strategies and navigate everyday emotional challenges.

Our guides and tools complement the wider Serenity experience by making information and self-directed resources accessible in a calm, approachable format.

### Moderation & safeguarding

Safety is fundamental to Serenity's design and operations.

Our platform incorporates dedicated internal systems supporting:

- Community moderation and content review
- Safeguarding and risk escalation
- Staff access controls and permissions
- Operational auditing and accountability
- Privacy-conscious data management
- Consistent safety and moderation workflows

These tools support our trained team members in maintaining a responsible and supportive environment.

## Current roadmap

With the initial public beta now launched, our focus has shifted towards expanding Serenity's support services and strengthening the underlying platform.

### 1-on-1 Listening

We are developing private listening sessions that provide individuals with opportunities to speak with trained listeners in a supportive, non-judgemental environment.

This service requires dedicated training, safeguarding and operational preparation before becoming publicly available.

### Audio & Video Therapy Services

We are developing secure audio and video therapy capabilities designed to connect patients with qualified therapists.

These services are distinct from our peer-support and community offerings and will require appropriate clinical, privacy, safeguarding and operational controls.

### Platform development

Alongside new services, we continue to improve:

- Community experience and accessibility
- Moderation and safeguarding capabilities
- Platform security and privacy
- Backend reliability and performance
- Automated testing and release assurance
- Monitoring, deployment and recovery processes

Our roadmap remains guided by the principle that safety and reliability must take priority over release speed.

## Our principles

- **Safety by design:** Safeguarding is embedded into product development, engineering and organisational operations.
- **Privacy with purpose:** We collect, process and expose only the information necessary to deliver our services safely and responsibly.
- **Human-led support:** We do not use AI to imitate human care or replace human mental health support.
- **Accessible by default:** Inclusive design, readable interfaces and accessible interaction patterns are core requirements.
- **Responsible engineering:** Security, testing, auditability, monitoring and recovery are integral to how we build and maintain our platform.
- **Honest boundaries:** We clearly distinguish community support, listening services, professional therapy and emergency care.

## Engineering at Serenity

Serenity is developed around a modular architecture that separates public-facing services, internal staff systems and backend infrastructure.

### Technology stack

| Technology | Purpose |
| --- | --- |
| React | Public Serenity platform |
| React & Vite | Internal staff dashboard |
| Node.js & Express | Backend API and application services |
| MariaDB / MySQL | Relational accounts, sessions and operational data |
| MongoDB | Community content and flexible document storage |
| Redis | Caching, real-time and performance-sensitive workloads |
| GitHub Actions | Continuous Integration and automated validation |
| Cloudflare Zero Trust | Protected access to internal QA environments |

Our infrastructure and development processes are designed to support controlled deployments, secure operations and continuous improvement.

## Core repositories

| Repository | Purpose |
| --- | --- |
| [serenityAPI_v1](https://github.com/Serenity-Central/serenityAPI_v1) | Backend API, authentication, data services and platform integrations |
| [serenityWebsite_v1](https://github.com/Serenity-Central/serenityWebsite_v1) | Public Serenity platform and community experience |

## Development & release workflow

Serenity follows a structured, multi-stage development and release process.

### Branching strategy

All new features, bug fixes and engineering improvements should be developed on dedicated branches.

Pull Requests should ordinarily target **`release/next`**, which serves as our staging and integration branch.

**Feature / Fix Branch → `release/next` → `development` → `production`**

| Branch | Purpose |
| --- | --- |
| Feature / Fix branches | Isolated development of individual changes |
| `release/next` | Staging, integration and initial validation |
| `development` | Deployment to the live, Cloudflare Zero Trust-protected QA environment for acceptance testing |
| `production` | Production releases promoted following successful validation |

### Release validation

Changes progress through a controlled validation process:

1. Development and initial manual testing in the local environment.
2. Pull Request review and automated CI validation.
3. Integration and staging through `release/next`.
4. Promotion to `development` and deployment to the protected QA environment.
5. Manual QA, regression checks and acceptance testing.
6. Promotion to `production` following successful validation and approval.

Production deployments are not treated as an automatic consequence of completing development work.

## Continuous Integration

Serenity uses **GitHub Actions** to automate backend quality checks and identify regressions before changes progress through the release process.

The **Backend CI** workflow runs automatically on Pull Requests targeting `release/next` or `development`, on pushes to `refactor/backend-test-suite`, and when manually triggered.

### Automated checks

1. **Isolated infrastructure:** Provision disposable MariaDB, MongoDB and Redis services, separate from operational environments.
2. **Database preparation:** Initialise a MongoDB replica set for transaction testing and import the dedicated MariaDB CI schema, verifying all 38 expected tables.
3. **Code quality:** Run ESLint against the backend codebase.
4. **Automated tests:** Execute the complete Jest backend test suite.
5. **Diagnostics:** Report the results in GitHub Actions and collect MongoDB diagnostics when a job fails.

The CI environment uses test-only credentials, disables background jobs and email delivery, and cleans up temporary MongoDB infrastructure after execution.

**Developers are expected to resolve failing CI checks before requesting final Pull Request approval.** Automated tests complement, rather than replace, peer review and manual QA.

> **Note:** GitHub Actions runs the checks. Enforcing successful checks as a merge requirement depends on the repository's branch protection rules or rulesets.

## Working with us

Most Serenity repositories are private because they contain proprietary platform code and security-sensitive implementation details. Access is provided to authorised contributors working under Serenity's confidentiality and engineering processes.

Contributors are expected to:

- Work from focused feature or fix branches.
- Open Pull Requests into `release/next` unless otherwise directed.
- Explain why a change is needed and how it was validated.
- Resolve failed CI checks before requesting final approval.
- Identify security, privacy, data and safeguarding implications.
- Keep unrelated refactors out of focused work.
- Treat review as collaboration, not ceremony.

If something feels unsafe or unclear, raise it early. Silence is rarely a useful engineering control.

## Connect with Serenity

- **Website:** [serenitycentral.cloud](https://serenitycentral.cloud)
- **Contact:** [serenitycentral.cloud/contact](https://serenitycentral.cloud/contact)
- **Instagram:** [@officialserenitycentral](https://www.instagram.com/officialserenitycentral/)

<div align="center">

Built with care for the people who rely on it.

</div>
