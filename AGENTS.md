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

## Agent Memory

Use `./LESSONSLEARNED.md` as the tracked durable lessons file for this repo.
Use `./CHATHISTORY.md` as the standard local handoff file for this repo.

- `LESSONSLEARNED.md` is tracked and should capture only reusable lessons.
- `CHATHISTORY.md` is local-only, gitignored, and should capture transient handoff context.
- Read `LESSONSLEARNED.md` and `CHATHISTORY.md` after `AGENTS.md` when resuming work.
- Add durable lessons to `LESSONSLEARNED.md` when they should influence future sessions.
- Keep transient entries brief and centered on template additions, preview regeneration, and next steps.
