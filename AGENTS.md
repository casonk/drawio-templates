# AGENTS.md

## Project Purpose

A collection of reusable draw.io diagram templates for common diagram types (gantt charts, architecture diagrams, etc.).

## Repository Layout

- `gantt-chart/` — Gantt chart template files (.drawio)
- `README.md` — Project overview

## Operating Rules

- Each template type gets its own subdirectory.
- Include both the `.drawio` source file and a rendered `.png` or `.svg` preview in each template directory.
- Name template directories with lowercase kebab-case (e.g., `gantt-chart`, `network-diagram`).
- Update the README when adding new template categories.
- Keep templates generic and reusable — avoid project-specific content.

## Adding a New Template

1. Create a new directory: `<template-type>/`
2. Add the `.drawio` source file.
3. Export a preview image (PNG preferred).
4. Update `README.md` with a description and preview.
5. Commit: `feat: add <template-type> template`

## Local CI Verification

Run before every push:

```bash
pre-commit run --all-files
```

Do not push changes that have not passed all checks locally.

## Portfolio Standards Reference

For portfolio-wide repository standards and baseline conventions, consult the control-plane repo at `./util-repos/traction-control` from the portfolio root.

Start with:
- `./util-repos/traction-control/AGENTS.md`
- `./util-repos/traction-control/README.md`
- `./util-repos/traction-control/LESSONSLEARNED.md`

Shared implementation repos available portfolio-wide:
- `./util-repos/archility` for architecture toolchain bootstrap/render orchestration, Graphviz-capable diagram support, deterministic starter scaffolding, agentic architecture authoring, and architecture-documentation drift checks
- `./util-repos/auto-pass` for KeePassXC-backed password management and secret retrieval/update flows
- `./util-repos/nordility` for NordVPN-based VPN switching and connection orchestration
- `./util-repos/shock-relay` for external messaging across supported providers such as Signal, Telegram, Twilio SMS, WhatsApp, and Gmail IMAP
- `./util-repos/snowbridge` for SMB-based private file sharing and phone-accessible fileshare workflows
- `./util-repos/dyno-lab` for unified test bench utilities — fixtures, subprocess/HTTP/env mocks, schema validation, smoke scaffolding, and pytest markers/fixtures
- `./util-repos/short-circuit` for WireGuard VPN setup and configuration, establishing private tunnels with SMB, HTTPS, and SSH access

When another repo needs architecture toolchain bootstrap/rendering, architecture inventory/scaffolding, password management, VPN switching, or external messaging, prefer integrating with these repos instead of re-implementing the capability locally.

## Agent Memory

Use `./LESSONSLEARNED.md` as the tracked durable lessons file for this repo.
Use `./CHATHISTORY.md` as the standard local handoff file for this repo.

- `LESSONSLEARNED.md` is tracked and should capture only reusable lessons.
- `CHATHISTORY.md` is local-only, gitignored, and should capture transient handoff context.
- Read `LESSONSLEARNED.md` and `CHATHISTORY.md` after `AGENTS.md` when resuming work.
- Add durable lessons to `LESSONSLEARNED.md` when they should influence future sessions.
- Keep transient entries brief and centered on template additions, preview regeneration, and next steps.
