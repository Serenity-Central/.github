# 🧠 Serenity Developer Brief

### Version 1.0 — June 2025
**Contact:** Kieron Skelton (Executive Director & Lead Developer)
<br>📧 [kieron-skelton@serenitycentral.cloud](mailto:kieron-skelton@serenitycentral.cloud) | 🌐 [www.serenitycentral.cloud](www.serenitycentral.cloud)

---

### 🌱 Mission & Context

**What is Serenity?** 
<br>Serenity is a mental health ecosystem designed to build safe, supportive spaces for peer-support, healing, and emotional wellbeing. It exists to bridge the gap between digital platforms and meaningful, accessible mental health support.

**Who are our users?**
<br>~40,000 Discord users aged 16+, many of whom are vulnerable, neurodivergent, or living with mental health challenges. They come to Serenity for anonymous support, resources, and a sense of safety.

**What do we offer (right now)?**

- A modular Discord bot with:
    - Anonymous peer support
    - Wellbeing tools (affirmations, self-care tools, mood tracking)
    - Serenity-side moderation and safety tools
- A public website with community info, blog posts, and recruitment tools

**Where are we going?**
<br>Within 6–12 months, we aim to:

- Expand the bot to Slack, Telegram, and other platforms
- Launch an independent, standalone Serenity support platform (web-based)
- Build the foundations of a sustainable, ethical mental health tech ecosystem

---

### 🛠️ Tech Stack & Codebase

**Frontend (Website):** React
<br>**Backend:** Node.js

- MongoDB: policies, blog, recruitment, team
- MySQL: Discord bot & services
- Redis: Used for real-time data exchange between the site and bots

**Discord Bot:** discord.js + MySQL + Redis (some HTML rendering for UI previews)

**Repositories:** (all on GitHub)
- [Serenity API](https://github.com/Serenity-Central/serenityApi) - Backend API
- [Serenity Website](https://github.com/Serenity-Central/serenityWebsite) - Frontend
- [Serenity Discord](https://github.com/Serenity-Central/serenity) - Discord Bot
- [Cloudiie Application](https://github.com/Serenity-Central/cloudiie) - Independent moderation tool (non-core)

Each repository uses `development` and `production` branches with manual deployments.

---

### 🚀 Infrastructure & Deployment
- Bots & API are containerised using **Pterodactyl**, hosted on an **OVH VPS**
- Website is hosted on a separate **Hostinger VPS**
- Secrets are managed via local `.env` files (not versioned)
- Manual deployments via **WinSCP** and **PuTTY (Ubuntu)**
- Weekly deployments every **Monday**, with pre-deploy backups created and locked
- Grafana dashboard tracks error logs pulled from a custom MySQL error table

---

### 🧭 Workflow & Team

**Current Dev Team:**
<br> Just Kieron, for now. This is why we **want you** here!

**Task Tracking:**
<br> Jira Scrum Board (epics, sprints, backlog grooming).

**Bug Reporting:**
<br>User-reported bugs flow via Discord or GitHub.
<br>Triage and prioritisation are manual for now.

**Communication:**
<br>Email, Discord, and Jira.
<br> Kieron is flexible and responsive, so however you feel comfortable contacting him is up to you.

**Onboard:**
<br>Currently handled 1:1 via conversation. You'll help define a proper dev onboarding flow.
<br> Each repository has its own `README.md` file with configuration instructions.

---

### 🔧 Short-Term Developer Priorities

**Immediate Needs:**
-  Stabilise and refactor the React + Node SPA (the backbone of our future standalone
platform)
- Improve developer onboarding + DX (docs, env setup, GitHub clarity)
- Build internal dashboards for:
    - Trust & safety moderation
    - Outreach/contact tools
- Expand bot features and start building Slack/Telegram-ready tooling
- Improve error handling, logging, and observability
- Evaluate CI/CD and testing frameworks — help define what “better” looks like here

---

### 🧩 Ideal First Tasks (Low Lift, High Value)

- Improve current error logging UI (Grafana or custom frontend)
- Modularise outdated React components
- Review SerenityAPI endpoints and propose structural improvements
- Begin documenting setup instructions for one of the repos
- Audit our .env usage and suggest safe restructuring

---

### 🌄 Growth & Future Vision

- This is not a short-term fire-and-forget project.
- Our goal is to grow into a full-stack platform for community-based mental health support—one that scales without compromising safety or empathy.
- Contributors today may evolve into core developers or paid leads when funding is secured.

---

**Ready to join the mission?**
<br>Let Kieron know what excites you, what scares you, and where you’d like to begin.

You don’t need to know everything. You just need to care.
