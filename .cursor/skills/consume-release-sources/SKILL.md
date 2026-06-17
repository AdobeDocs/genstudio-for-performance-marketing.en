---
name: consume-release-sources
description: >-
  Phase 0 for GenStudio monthly release notes: resolve the Jira work ticket,
  fetch the release ceremony wiki, parse GA and Beta feature group tables, pull
  linked KT pages via Confluence MCP, and hand structured inputs to
  generate-release-notes. Use when Jira and Confluence MCP are available and the
  user is adding or rotating release notes.
---

# Consume release sources (Jira + Confluence MCP)

**Downstream drafting:** [generate-release-notes](../generate-release-notes/SKILL.md) → optional [polish-release-notes](../polish-release-notes/SKILL.md)

**Parsing reference:** [reference.md](reference.md)

**Target output file (downstream only):** [help/user-guide/release-notes.md](../../help/user-guide/release-notes.md)

## Prerequisites

- **Jira MCP** (`jira_getIssue`, `jira_searchIssues`) authenticated
- **Confluence MCP** (`confluence_getContent`, `confluence_searchContent`) authenticated
- Jira ticket key from branch name (`GS-#####`), user input, or ticket description

## Workflow checklist

1. [ ] **Resolve Jira ticket** — `jira_getIssue` with `issueKey`. Read `description` for the ceremony wiki link and release month.
2. [ ] **Locate ceremony page** — use wiki URL from ticket; fallback CQL: `title ~ "YYYY/MM Release Ceremony" AND space = GenStudio`.
3. [ ] **Fetch ceremony body** — `confluence_getContent` with `bodyMode: storage` (required; `text` loses KT links and table structure).
4. [ ] **Parse feature groups** — extract rows from **GA Release Features** and **Beta Release Features** (see [reference.md](reference.md#ceremony-feature-groups)).
5. [ ] **Apply inclusion filter** — per user scope (see [reference.md](reference.md#inclusion-filters)); confirm Beta row count (may be zero).
6. [ ] **Resolve KT pages** — `confluence_searchContent` per KT title; `confluence_getContent` with `bodyMode: text`.
7. [ ] **Extract KT fields** — Description, Elevator pitch, Feature(s) delivered, Problem statement, Release Type & Date.
8. [ ] **Set Beta flags** — `requiresBetaBadge: true` for Beta section rows or GA-table rows with Type `Beta`.
9. [ ] **Hand off** to [generate-release-notes](../generate-release-notes/SKILL.md) with structured row list (no wiki/Jira refs in shipped copy).

## Beta labeling (handoff to generate skill)

When `requiresBetaBadge: true`, the downstream `###` section must include immediately under the heading:

```markdown
[!BADGE Beta]{type=Informative tooltip="This feature is currently in Beta, so some functionality may be limited or subject to change."}
```

Do not add italic scheduling disclaimers for Beta; the badge is the supported pattern.

## Prohibited in shipped release notes

Internal IDs, wiki URLs, KT citations, and Jira keys stay in this ingest phase only. Summarize user-facing outcomes in the public page per [generate-release-notes prohibited content](../generate-release-notes/SKILL.md#prohibited-content).

## Fallback

If MCP calls fail, ask the user to paste ceremony and KT content, then continue with generate-release-notes using [reference.md KT field mapping](../generate-release-notes/reference.md#internal-sources-kt-and-release-wikis).

## Additional resources

- [reference.md](reference.md) — ceremony parsing, CQL, inclusion filters, MCP parameters
- [generate-release-notes](../generate-release-notes/SKILL.md) — archive, draft, links, quality checks
- [polish-release-notes](../polish-release-notes/SKILL.md) — editorial pass on new `###` under `{#latest}`
