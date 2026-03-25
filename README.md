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

> Cursor + Claude Code + Figma MCP · Sections 12–14 · March 2026
