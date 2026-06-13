# arbiterForge

> Developer tooling that refuses to freelance.

## ⚖️ codeArbiter

An orchestration layer for [Claude Code](https://claude.com/claude-code). Every intent
routes through a slash command to a gated skill or reviewer agent; nothing commits until
the gates are green; decisions go through SMARTS; the audit trail is append-only and
mechanically guarded.

- **Spec-driven TDD** — no feature code before a failing test; no commit through a red suite.
- **Mechanical gates** — commit-gate, security controls, and audit trail enforced by hooks, not vibes.
- **Per-repo & explicit** — dormant everywhere until you run `/ca:init`. Writes only to `.codearbiter/`.

**Install**

    /plugin marketplace add arbiterForge/codeArbiter
    /plugin install ca@codearbiter

Requires Python 3 on `PATH`. → **[codeArbiter repository](https://github.com/arbiterForge/codeArbiter)**

## 🛠️ arbiterIDE

Our IDE project — currently in private development.

## Contact

📫 contact via GitHub issues
