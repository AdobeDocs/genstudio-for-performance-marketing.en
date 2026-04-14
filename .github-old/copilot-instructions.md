## Purpose

Help AI coding assistants make small, safe edits to the GenStudio for Performance Marketing documentation repo.

## High-level architecture (short)
- This repo is a documentation site composed of Markdown under `help/` with shared includes in `help/_includes/` and curated images under `help/_includes/assets/`.
- Release notes, user-guide, and extensibility content live under `help/`. Large content changes should preserve frontmatter and existing heading structure.
- The site is built using Jekyll and hosted on GitHub Pages. The build process uses standard Jekyll conventions with some custom plugins.

## Project-specific conventions
- Cursor rules: Custom automation and guidance lives in `.cursor/rules/*.mdc`. Examples: `.cursor/rules/docs-lint.mdc` (lint process), `.cursor/rules/generate-release-notes.mdc` (points to the release notes skill when editing `help/user-guide/release-notes.md`). Follow these for automated tasks.
- Agent skills: Task workflows live under `.cursor/skills/<name>/SKILL.md`. Example: `.cursor/skills/generate-release-notes/SKILL.md` (full GenStudio release notes procedure; use with `examples.md` and `reference.md` in the same folder).
- Filenames and frontmatter:
  - Release notes: preserve existing Experience League frontmatter on `help/user-guide/release-notes.md` (see `.cursor/skills/generate-release-notes/reference.md#frontmatter`); the thin rule `.cursor/rules/generate-release-notes.mdc` auto-attaches when that file is edited.
  - Use kebab-case for rule files and `.mdc` extension.
- Formatting conventions: Docs use GitHub-flavored Markdown. Headings generally follow sentence case and short paragraphs. Prefer `*` bullets for lists in release notes and `###` for feature sections.

## Documentation style guidelines
- Follow the [Microsoft Writing Style Guide](https://learn.microsoft.com/en-us/style-guide/) for technical documentation best practices:
  - Write clear, concise sentences focused on user actions
  - Use active voice and present tense
  - Break text into short, scannable chunks
  - Keep a warm, direct tone while maintaining technical accuracy
- Markdown authoring:
  - Use sentence case for headings (capitalize first word only)
  - Keep paragraphs short (2-3 sentences) for readability
  - Add blank lines before and after headings and lists
  - Use backticks for UI elements, file paths, and code
  - Include alt text for all images
  - Link to specific sections using descriptive text

## Safety rules for edits (what AI should do)
- Never add Jira IDs, internal links, or corporate-only references to public docs. See `.cursor/skills/generate-release-notes/SKILL.md` (section **Prohibited content**).
- Preserve frontmatter YAML exactly when editing files that include it. Many templates and release notes rely on fixed keys (title, description, role, exl-id).
- For lint fixes, prefer automated, idempotent edits from `.cursor/rules/docs-lint.mdc` (remove trailing spaces, ensure final newline). Example commands used by humans:

```sh
sed -i '' 's/ $//' <file>
sed -i '' '$ { /^$/d; }' <file> && echo "" >> <file>
```

## Examples (what to change and how)
- Small copy fixes: update text inside `help/` Markdown files, keep headings and anchors intact.
- Image updates: reference images under `help/_includes/assets/`. Do not move or rename images without updating all references.

## Where to look first
- `help/_includes/` — shared fragments and images.
- `.cursor/rules/` — automation and linting guidance; use these as authoritative rules for formatting and processes.
- `markdownlint_custom.json` — local markdownlint overrides.
- `.github/pull_request_template.md` — PR expectations.

## When to ask the human
- If a change requires running or modifying Docker-based tooling (the lint rule mentions Docker) or affects site build pipelines.
- If a file references unknown external config (for example `markdownlint.json` is missing) — ask whether to create or ignore.

## Minimal commands for humans
```sh
# Install linter (if not present)
npm install -g markdownlint-cli

# Run lint locally using project config
markdownlint --config markdownlint_custom.json "help/**/*.md"

# Project lint via yarn (preferred if available in environment)
yarn lint
```

---
If you want, I can merge this into `.github/copilot-instructions.md` in the repo (or adjust wording/length). What should I change or add?
