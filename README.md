# XC Design Offering — AI-Augmented Delivery

Resources, toolchain configuration, and workflow artifacts for XCentium's AI-powered design and delivery practice.

---

## What's in This Repo

| File | Description |
|------|-------------|
| `xcm-ai-workflow-matrix.html` | AI delivery workflow matrix mapping tools and agents across the full project lifecycle (Discovery → Design → Prototyping → Spec & Generation → Validation → Development) |
| `xcm_toolchain_setup.html` | Step-by-step setup guide for the XCentium AI toolchain — Figma MCP, Cursor, Claude Code, and Claude.ai |
| `xcm-prompt-library.html` | Curated prompt library for AI-assisted delivery workflows |

---

## The Stack

| Tool | Role |
|------|------|
| **Figma + Figma Console MCP** | Design source of truth; connects directly to AI agents via MCP |
| **Claude.ai** | Spec generation, user stories, QA narratives, prompt workflows |
| **Claude Code** | Agentic AI in terminal — spec generator, validator, and dev assistant |
| **Cursor** | AI-native IDE for implementation; consumes specs from Claude |
| **Make** | Automation layer for handoff and workflow orchestration |

---

## Delivery Phases
```
Discovery → Design → Prototyping → Spec & Generation → Validation → Development
```

Each phase maps to specific tools, AI agents, inputs, and outputs. See `xcm-ai-workflow-matrix.html` for the full breakdown.

---

## Getting Started

1. Open `xcm_toolchain_setup.html` and complete the toolchain setup for your OS
2. Configure Figma MCP and Cursor with the provided settings
3. Reference the prompt library during spec generation and delivery sprints
4. Use the workflow matrix to orient yourself within the delivery process

---

## Requirements

- Figma Dev, Professional, Org, or Enterprise seat
- Claude Pro ($20/mo) or Claude Max ($100–200/mo) — or Console API key
- Node.js (see setup guide for version requirements)
- Cursor (cursor.com)
- Recommended: WSL2 on Windows for full workflow compatibility

---

## Part of XCentium's AI Practice

This repo supports XCentium's AI delivery methodology — bridging onshore design intent with offshore development execution through structured specs, AI-generated artifacts, and validated handoff packages.

## Contributing

This repo is a living system — prompts get sharper, workflows evolve, and the toolchain changes. Here's how to contribute without breaking things for the team.

### Adding or Updating Prompts
- Edit `xcm-prompt-library.html` directly
- Include the phase it belongs to (Discovery, Spec & Generation, etc.), the intended output, and any known constraints or failure modes
- If a prompt replaces an existing one, keep the old version commented out with a note explaining what changed and why

### Updating the Workflow Matrix
- Changes to `xcm-ai-workflow-matrix.html` should reflect actual practice, not aspirational workflow
- If a tool or agent role changes, update the matrix and note it in your PR description
- Don't add a tool to the matrix until it's been validated in at least one sprint

### Toolchain Setup Changes
- If setup steps change (new MCP version, Node requirement, Cursor config), update `xcm_toolchain_setup.html` and flag it clearly — people follow this doc cold
- Test your changes on both Mac and Windows (WSL2) if possible

### Pull Request Guidelines
- Branch from `main` using the format: `update/[what-you-changed]` (e.g. `update/prompt-library-spec-gen`)
- PRs should include a one-line summary of what changed and why
- Tag a reviewer from the onshore team before merging anything that affects the offshore handoff workflow

### Questions or Issues
Open an issue or ping the design systems channel. If something in the toolchain is broken or a prompt is consistently underperforming, that's worth a ticket — not just a Slack thread.

> Cursor + Claude Code + Figma MCP · Sections 12–14 · March 2026
