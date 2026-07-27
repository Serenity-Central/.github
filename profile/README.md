<div align="center">

# Serenity

### A safer space to breathe.

We are building safer, calmer and more human digital spaces for mental health support.

[![Website](https://img.shields.io/badge/Website-serenitycentral.cloud-7656A8?style=for-the-badge)](https://serenitycentral.cloud)
[![Public Beta](https://img.shields.io/badge/Public_Beta-September_2026-4F8A8B?style=for-the-badge)](https://serenitycentral.cloud)
[![Status](https://img.shields.io/badge/Status-Active_Development-2E7D32?style=for-the-badge)](#current-roadmap)

</div>

## About Serenity

The Serenity Project is a UK mental health social enterprise creating accessible digital support built around safety, privacy and genuine human connection.

Our work is designed for the moments when someone needs space to breathe, make sense of how they feel, find reliable information or connect with a supportive community.

Serenity is not a crisis service or a replacement for professional healthcare. We are building a responsible layer of community and emotional support around the services people may already use.

## What we are building

### Serenity Community

A moderated community where people can share what they are going through, respond with support and feel less alone without being pushed to reveal more than they are comfortable sharing.

### Anonymous venting

A quieter space for people to express difficult thoughts and emotions, with privacy-conscious identities, content controls and safeguarding processes built into the platform.

### Serenity Hubs

A growing library of carefully structured mental health resources designed to make trustworthy information easier to understand and navigate.

### Staff safety tools

Purpose-built moderation, safeguarding, audit and operational tools that help trained team members protect the community and respond consistently.

### 1-on-1 listening

Private sessions with trained listeners are planned for December 2026. We moved this feature beyond the September MVP so it can receive the dedicated safety, training and operational preparation it deserves.

## Current roadmap

Our public beta is planned for **September 2026**.

The first release is focused on doing a smaller number of things properly:

- Secure account access
- Anonymous community venting
- Peer support interactions
- Mental health resource hubs
- Moderation and safeguarding workflows
- Reliable deployment, monitoring and rollback processes

We would rather release carefully than rush features that involve vulnerable people. That principle shapes both our roadmap and our engineering decisions.

## Our principles

- **Safety by design:** Safeguarding is part of product design, engineering and operations from the beginning.
- **Privacy with purpose:** We collect and expose only what is necessary for the service to work safely.
- **Human-led support:** We do not use AI to provide mental health support or imitate human care.
- **Accessible by default:** Calm language, readable interfaces and inclusive interaction patterns are treated as core requirements.
- **Responsible engineering:** Security, auditability, testing and recovery matter as much as shipping the feature.
- **Honest boundaries:** We are clear about what Serenity can provide and when someone may need specialist or emergency support.

## Engineering at Serenity

Our platform currently uses:

- **React** for the public website
- **React and Vite** for the staff dashboard
- **Node.js and Express** for the API
- **MySQL** for relational accounts, sessions and operational records
- **MongoDB** for flexible content and community data
- **Redis** for real-time and performance-sensitive workloads

The platform is separated across public, staff and API services so each area can evolve with appropriate security and deployment controls.

## Core repositories

| Repository | Purpose |
| --- | --- |
| [serenityAPI_v1](https://github.com/Serenity-Central/serenityAPI_v1) | Backend API, authentication, data services and platform integrations |
| [serenityWebsite_v1](https://github.com/Serenity-Central/serenityWebsite_v1) | Public Serenity platform and community experience |

## Working with us

Most Serenity repositories are private because they contain proprietary platform code and security-sensitive implementation details. Access is provided to authorised contributors working under Serenity's confidentiality and engineering processes.

Contributors are expected to:

- Work from focused feature or fix branches
- Open pull requests into `development`
- Explain why a change is needed and how it was validated
- Identify security, privacy, data and safeguarding implications
- Keep unrelated refactors out of focused work
- Treat review as collaboration, not ceremony

If something feels unsafe or unclear, raise it early. Silence is rarely a useful engineering control.

## Connect with Serenity

- **Website:** [serenitycentral.cloud](https://serenitycentral.cloud)
- **Contact:** [serenitycentral.cloud/contact](https://serenitycentral.cloud/contact)
- **Instagram:** [@officialserenitycentral](https://www.instagram.com/officialserenitycentral/)

<div align="center">

Built with care for the people who may eventually rely on it.

</div>
