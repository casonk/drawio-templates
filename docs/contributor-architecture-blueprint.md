# Contributor Architecture Blueprint

This document is the starter architecture map for `drawio-templates`.
Keep it aligned with the real repository layout and execution flow as the repo evolves.

## Standard Architecture Assets

- PlantUML source: `docs/diagrams/repo-architecture.puml`
- Draw.io source: `docs/diagrams/repo-architecture.drawio`
- Expected renders after `archility render`:
  - `docs/diagrams/repo-architecture.puml.svg`
  - `docs/diagrams/repo-architecture.puml.png`
  - `docs/diagrams/repo-architecture.drawio.svg`
  - `docs/diagrams/repo-architecture.drawio.png`
- Shared toolchain owner: `../util-repos/archility` from this repo

## Regeneration

```bash
cd ../util-repos/archility
PYTHONDONTWRITEBYTECODE=1 PYTHONPATH=src python3 -m archility generate ../../drawio-templates
PYTHONDONTWRITEBYTECODE=1 PYTHONPATH=src python3 -m archility render ../../drawio-templates
```

## Current Focus Roots

- `gantt-chart/`

## Automation

- `.github/workflows/` is the standard automation directory for repo validation.

## Contributor Notes

- Treat this file and the paired `docs/diagrams/` sources as the default architecture handoff surface.
- Expand this starter blueprint with repo-specific flow, dependency, and deployment details when the repository grows beyond the generated baseline.
- Update the blueprint and diagram sources together when folder structure, execution flow, or integration boundaries change.
