# BitSleuth AI Coding Agent Instructions

Welcome to the BitSleuth codebase! This guide is for AI coding agents to maximize productivity and maintain project conventions.

## Big Picture Architecture
- **Purpose:** BitSleuth provides AI-powered Bitcoin wallet analysis and privacy tools.
- **Key Components:**
  - **Wallet Analyzer:** Visualizes BTC transaction flows, explains wallet activity, and detects OPSEC risks.
  - **Privacy Wallet:** Client-side encrypted, privacy-focused Bitcoin wallet to minimize on-chain traceability.
- **External Integrations:**
  - Connects to Bitcoin blockchain data sources for analysis.
  - Uses AI models for plain-language wallet explanations and risk detection.

## Developer Workflows
- **Bug Reports & Feature Requests:**
  - Use GitHub Issues for bugs: https://github.com/BitSleuthAI/.github/issues
  - Use GitHub Discussions for feedback: https://github.com/BitSleuthAI/.github/discussions
- **Documentation:**
  - Main project info is in `profile/README.md`.
  - Product links: [Wallet Analyzer](https://app.bitsleuth.ai), [Privacy Wallet](https://www.bitsleuth.ai/wallet)

## Project-Specific Conventions
- **Privacy First:** All wallet features must minimize address reuse and on-chain exposure.
- **Client-Side Encryption:** Wallet data is encrypted before leaving the user's device.
- **AI Explanations:** Use AI to generate clear, actionable insights for users (e.g., "Where did these coins come from?").
- **Visual Intelligence:** Transaction flows and graphs are core to the user experience.

## Patterns & Examples
- **Transaction Analysis:**
  - Always trace coin origins and mixing events.
  - Flag OPSEC risks (e.g., address clustering, reused addresses).
- **Wallet Storage:**
  - Never store unencrypted wallet data server-side.
- **User Feedback:**
  - Prioritize actionable, plain-language outputs over technical jargon.

## Key Files & Directories
- `profile/README.md`: Project overview, mission, and tool links.
- `.github/`: Central location for issues, discussions, and instructions.

---

For questions or unclear conventions, review `profile/README.md` or ask for clarification in GitHub Discussions.

---

*Last updated: 25 October 2025*
