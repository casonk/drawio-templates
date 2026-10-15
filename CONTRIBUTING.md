# Contributing

This repository stores reusable draw.io templates. New additions should stay generic, easy to preview, and ready to reuse in other projects.

## Workflow

1. Create a dedicated directory for the template family using lowercase kebab-case.
2. Commit the `.drawio` source file.
3. Export at least one preview image so the template is visible from GitHub.
4. Update `README.md` with the new template name, source path, and preview.
5. Use a focused Conventional Commit such as `feat: add network-diagram template`.

## Template Standards

- Keep labels and sample content generic rather than project-specific.
- Prefer consistent canvas sizing and legible defaults.
- Include both editable source and rendered preview assets in the same change.
- When refreshing an existing template, update the preview images so the documentation stays accurate.

## Pull Requests

- Keep each pull request to one template family or one cleanup theme.
- Fill out the PR template.
- Ensure any relevant checks pass before merging.
- Do not commit secrets, credentials, or sensitive data.
- Mention whether previews were regenerated.
- Call out any compatibility considerations for draw.io or diagrams.net users.

## AI Contribution Disclosure

Parts of this repository's code, documentation and commit history were drafted
with AI coding assistants, including Claude Code, OpenAI Codex, GitHub Copilot
and Continue. The maintainer directs that work, reviews and tests each change
before it merges, and is responsible for the result.

This section is the repository-wide disclosure. Individual commits, pull
requests and files do not carry per-tool attribution lines.
