[![Typing SVG](https://readme-typing-svg.herokuapp.com?font=Fira+Code&pause=1000&color=00A3FF&width=435&lines=🚀+Building+Serenity;💭+Coding+with+purpose;🧩+Not+chasing+badges.)](https://git.io/typing-svg)

# 🧠 Serenity Developer Brief

### Version 2.1.0 — March 2026
**Contact:** <br>
Kieron Skelton (Executive Director)
<br>📧 [kieron-skelton@serenitycentral.cloud](mailto:kieron-skelton@serenitycentral.cloud) <br> 🌐 [www.serenitycentral.cloud](www.serenitycentral.cloud) <br><br>
Monika Lumi (Director of Engineering)
<br>📧 [monika-lumi@serenitycentral.cloud](mailto:monika-lumi@serenitycentral.cloud) <br> 🌐 [www.serenitycentral.cloud](www.serenitycentral.cloud) 

---
![Node](https://img.shields.io/badge/node-%3E=18-green)
[![License](https://img.shields.io/badge/license-proprietary-red)](./LICENSE)
![Status](https://img.shields.io/badge/status-active-success)

![Build](https://img.shields.io/badge/build-passing-brightgreen)
![Coverage](https://img.shields.io/badge/coverage-85%25-yellowgreen)
![Lint](https://img.shields.io/badge/lint-eslint-blue)

![GDPR](https://img.shields.io/badge/GDPR-compliant-blue)
![Audit Logs](https://img.shields.io/badge/audit%20logging-enabled-blueviolet)

![Safeguarding](https://img.shields.io/badge/safeguarding-active-important)
![Mental Health](https://img.shields.io/badge/focus-mental%20health-critical)

---

## Welcome!

Thank you for contributing to **The Serenity Project**.

Serenity is a mental-health–focused social enterprise building safe, ethical, and accessible support systems. Our codebase underpins real people, real vulnerability, and real outcomes, so clarity, care, and correctness matter here.

This document explains **how we work**, **how to contribute**, and **how to avoid breaking things that keep people safe**.

---

> **Confidential & Proprietary:**  
> This repository contains private Serenity Project code. Access is restricted to authorised contributors under NDA.

---

## Tech Stack & Codebase

### Frontend
- **Website:** React
- **Staff Dashboard:** React + Vite (Seperate repository from the primary platform)

### Backend
- **API:** Node.js (Express)
- **MongoDB:**
<br> Used for flexible / document based data:
  - Policies
  - Blog Posts
  - Recruitment
  - Team data
  - peer-to-peer messages
- **MySQL:**
  <br> Used only for *hard, relational date* (e.g. subscribers, users & sessions).
- **Redis:**
  <br> Used for:
  - Real-time data exchange
  - Cross service communitcation
  - Performance-sensitive operations 
   
---

## Repositories: 
All repositories are hosted on GitHub
- **[Serenity API](https://github.com/Serenity-Central/serenityAPI_v1)** - Backend API
- **[Serenity Website](https://github.com/Serenity-Central/serenityWebsite_v1)** - Public Frontend
- **[Serenity Staff Dashboard](https://github.com/Serenity-Central/serenityStaffDashboard)** - Staff Frontend

---

## Branching Strategy (Important)

<br>We use a **simple, deliberate flow**:
- `production` → Live environment
- `development` → Staging / integration
- `feature/*` → All new work

### Correct workflow

**Do not open PRs directly from `development` into `production`.**  
If this happens accidentally, we will ask you to re-branch, no drama, just process.
1. Create a feature branch from `development`
2. Commit work to your feature branch
3. Open a PR **into `development`**
4. `development` → `production` merges are handled manually

---

## Pull Requests

When opening a PR:
- Keep scope focused
- Explain *why* the change exists, not just *what* it does
- Flag:
  - security impact
  - data model changes
  - safeguarding implications (if applicable)
 
### Templates:
- PR Template → [ISSUE_TEMPLATE/PR_template.md](https://github.com/Serenity-Central/.github/blob/main/ISSUE_TEMPLATE/PR_template.md)
- Task Template → [ISSUE_TEMPLATE/task_template.md](https://github.com/Serenity-Central/.github/blob/main/ISSUE_TEMPLATE/task_template.md)


---

## Security, Privacy & Safeguarding

This platform handles sensitive mental health data.

Please:
- Never log personal data unnecessarily
- Avoid console logging in production code
- Treat anything user-related as potentially sensitive
- Flag uncertainty early — silence is riskier than questions

If you spot a security concern, raise it immediately.

---

## Tech Debt

Debt is officially recorded and documented by the leadership team. But you will see comments sush as:
```js
// TODO(tech-debt): ...
```
This **is intentional and tracked.**

Do not silently "fix" tech debt unless it is:
- directly related to your task, or
- explicitly agreed with the Lead Developer / CTO

We track debt deliberately to avoid accidental regressions.

---

## Communication & Expectations
- Ask questions early
- No one is expected to know everything
- Protect your boundaries — expectation creep helps nobody
- We host bi-weekly stand-ups
- We optimise for clarity over speed

### Internal Channels:
- WhatsApp (team coordination)
- Sling (rostering and aailability)
- Serenity Mail (Private & Confidentail internal correspondence) 

---

**Ready to join the mission?**
<br>Let us know what excites you, what scares you, and where you’d like to begin.

You don’t need to know everything. You just need to care.

https://serenitycentral.cloud/contact
