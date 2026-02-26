# Pingara Coding Agent Instructions

Welcome to the Pingara codebase! This guide is for AI coding agents to maximize productivity and maintain project conventions.

## Big Picture Architecture
- **Purpose:** Pingara provides affordable uptime and performance monitoring for websites and services.
- **Key Components:**
  - **URL Monitoring:** Continuously monitors HTTP/HTTPS endpoints from multiple geographic regions with configurable check intervals.
  - **Alerting System:** Instant notifications via Email, Slack, and Webhooks when downtime or performance degradation is detected.
  - **Dashboard & Reporting:** Comprehensive dashboards with uptime percentages, latency charts (p50/p95/p99), and incident timelines.
  - **Status Pages:** Branded public status pages displaying service health, historical uptime, and ongoing incidents.
  - **Multi-Region with Quorum:** Monitors from US, EU, and APAC regions with intelligent quorum rules to reduce false positives.
  - **AI Root Cause Hints:** AI-driven suggestions for possible root causes based on collected metrics.
- **External Integrations:**
  - Multi-region monitoring infrastructure (US, EU, APAC).
  - AI models for root cause analysis and advisory suggestions.
  - Notification channels: Email, Slack, Webhooks.

## Developer Workflows
- **Bug Reports & Feature Requests:**
  - Use GitHub Issues for bugs: https://github.com/Pingara/.github/issues
  - Use GitHub Discussions for feedback: https://github.com/Pingara/.github/discussions
- **Documentation:**
  - Main project info is in `profile/README.md`.
  - Product website: [www.pingara.io](https://www.pingara.io)

## Project-Specific Conventions
- **Reliability First:** Monitoring checks must be accurate and minimize false positives using quorum-based decisions.
- **Multi-Region:** All monitoring should support checks from multiple geographic regions.
- **Affordable & Accessible:** Features should be designed to work within the free tier where possible, scaling for paid plans.
- **AI Insights:** Use AI to generate clear, actionable root cause suggestions for users.
- **Status Page Transparency:** Public status pages should be SEO-optimized and customer-friendly.

## Patterns & Examples
- **Monitoring Checks:**
  - Validate HTTP status codes, keywords, and SSL certificate expiry.
  - Use consecutive failure requirements and quorum rules before changing monitor state.
- **Alerting:**
  - Support escalation and repeat notifications with alert deduplication to reduce fatigue.
- **Apdex Scoring:**
  - Use configurable T thresholds with hourly and daily rollups.
- **User Feedback:**
  - Prioritize actionable, plain-language outputs over technical jargon.

## Key Files & Directories
- `profile/README.md`: Project overview, mission, and feature links.
- `.github/`: Central location for issues, discussions, and instructions.

---

For questions or unclear conventions, review `profile/README.md` or ask for clarification in GitHub Discussions.

---

*Last updated: February 2026*
