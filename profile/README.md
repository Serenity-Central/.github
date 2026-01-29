[![Typing SVG](https://readme-typing-svg.herokuapp.com?font=Fira+Code&pause=1000&color=00A3FF&width=435&lines=🚀+Building+Serenity;💭+Coding+with+purpose;🧩+Not+chasing+badges.)](https://git.io/typing-svg)

# 🧠 Serenity Developer Brief

### Version 2.0.0 — January 2026
**Contact:** <br>
Kieron Skelton (Executive Director & Lead Developer)
<br>📧 [kieron-skelton@serenitycentral.cloud](mailto:kieron-skelton@serenitycentral.cloud) | 🌐 [www.serenitycentral.cloud](www.serenitycentral.cloud)

---

## Welcome!

Thank you for contributing to **The Serenity Project**.

Serenity is a mental-health–focused social enterprise building safe, ethical, and accessible support systems. Our codebase underpins real people, real vulnerability, and real outcomes, so clarity, care, and correctness matter here.

This document explains **how we work**, **how to contribute**, and **how to avoid breaking things that keep people safe**.

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

If something feels unclear, that’s a documentation issue, not a personal failure.

**Ready to join the mission?**
<br>Let us know what excites you, what scares you, and where you’d like to begin.

You don’t need to know everything. You just need to care.

https://serenitycentral.cloud/contact
