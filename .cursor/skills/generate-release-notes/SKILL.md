---
name: generate-release-notes
description: >-
  Drafts or updates Adobe GenStudio for Performance Marketing release notes in
  help/user-guide/release-notes.md. Use when adding a monthly release,
  archiving the previous {#latest} section, editing release notes content, or
  summarizing Knowledge Transfer or internal release inputs into user-facing
  bullets. Follows ExL structure, Beta badges, doc links, and archival
  collapsible sections. Edits target only the {#latest} block; Earlier release
  notes are read-only except the archive cut/paste when rotating a new month.
---

# Generate GenStudio release notes

**Canonical target file:** [help/user-guide/release-notes.md](help/user-guide/release-notes.md)

**Full examples:** [examples.md](examples.md)

**KT/wiki field mapping and doc paths:** [reference.md](reference.md)

## Editing scope (strict)

When using this skill, **the only place** you may **add** or **edit** release note body content is the section headed with **`## … {#latest}`** (the single block that carries the `{#latest}` anchor).

- **Do not** edit **Earlier release notes**—any `+++Notes from YYYY.MM.DD+++` collapsible block—or **any** older `##` monthly section that no longer has `{#latest}`, even when the topic seems related, a link looks wrong, or copy appears duplicated or outdated there.
- **Do not** “touch up” prior `###` subsections, bullets, links, or wording outside the current `{#latest}` block unless the user gives an **explicit, separate** request that is not covered by this skill.
- **Exception:** [Archive previous latest](#archive-previous-latest) when introducing a **new** top `{#latest}` block: **move** the entire former `{#latest}` section into a **new** collapsible under **Earlier release notes** as described below. During that pass, **do not** rewrite or add to **other, older** archive blocks.

If new information belongs in the doc, place it under the current **`{#latest}`** heading (or archive first, then add only under the new `{#latest}`).

## Workflow checklist

Work in this order. Copy the checklist and track progress for multi-step edits.

0. [ ] If **Jira** and **Confluence** MCP are available, run [consume-release-sources](../consume-release-sources/SKILL.md) first to ingest the work ticket, ceremony wiki (GA and Beta feature groups), and KT pages. If MCP is unavailable, use pasted KT/wiki content and [reference.md](reference.md#internal-sources-kt-and-release-wikis) field mapping.
1. [ ] Open `help/user-guide/release-notes.md` and read the current `## YYYY.MM {#latest}` block. Treat **Earlier release notes** as **read-only** context unless you are performing the archive step in step 2.
2. [ ] If adding a **new** monthly release: archive the current latest (see [Archive previous latest](#archive-previous-latest)).
3. [ ] Add or edit **only** the top `## YYYY.MM {#latest}` section (newest month at top of the release list).
4. [ ] For each item, apply [Decision rules](#decision-rules) (feature `###` vs **Fixes and enhancements**, Beta badge or not).
5. [ ] Add or verify documentation links on the most relevant phrase (see [reference.md](reference.md#documentation-linking)).
6. [ ] Run [Quality checks](#quality-checks) before finishing.
7. [ ] Preserve [frontmatter](reference.md#frontmatter) on the page unless the task explicitly updates metadata.

## Decision rules

Use these if/then rules so content lands in the right place:

| If | Then |
|----|------|
| The capability is new and in Beta | Add the Beta badge line immediately under the `###` heading (see [examples.md](examples.md)). |
| Source material explicitly labels the item as a **fix** or **enhancement** | Put it under `### Fixes and enhancements` with `*` bullets only. |
| The item is a net-new capability or feature story | Use a `###` feature section with 1–3 sentences (not the fixes list). |
| You are unsure whether something is a fix or a feature | Default to a `###` feature section unless the source clearly says fix/enhancement. |

**Fixes section rule:** Do not add bullets to **Fixes and enhancements** unless the source is explicitly labeled as a fix or enhancement.

## Archive previous latest

When introducing a new `## YYYY.MM {#latest}`:

1. Cut the entire previous `## YYYY.MM {#latest}` section (from its heading through the end of that release’s content, before the next `##` or **Earlier release notes**).
2. Paste it into **Earlier release notes**, inside a **new** collapsible block.
3. Replace the old heading with: `+++Notes from YYYY.MM.DD+++` (use the real release date; format as in existing notes in the file).
4. Remove `{#latest}` from the archived heading; the new top section is the only one with `{#latest}`.
5. Keep chronological order inside **Earlier release notes** (newest archived blocks toward the top unless the file already uses a different ordering—**match the existing file**).

Do **not** edit the body of **pre-existing** `+++Notes from …+++` blocks while performing this archive—only insert the newly archived block and preserve older archives as-is.

## Required structure

### Page title and intro

After frontmatter, use:

```markdown
# GenStudio for Performance Marketing release notes

This release information details the latest updates to the GenStudio for Performance Marketing application.
```

If the file already uses a slightly different intro sentence (e.g. “provides” instead of “details”), keep consistency with the rest of the page.

### Latest release heading

- Format: `## YYYY.MM {#latest}` for the newest release block.
- Only one `{#latest}` anchor on the page.

### Feature sections

- Use `###` for major feature categories.
- Present tense, 1–3 sentences, clear what/why and user actions where helpful.
- Product names: `[!DNL Create]`, `[!DNL Content]`, `[!DNL Insights]`, etc.
- UI: `[!UICONTROL Control Name]` where appropriate.
- Emphasis: `_italics_` for UI areas/sections; `**bold**` for key terms sparingly.

### Beta badge

Use exactly:

```markdown
[!BADGE Beta]{type=Informative tooltip="This feature is currently in Beta, so some functionality may be limited or subject to change."}
```

### Documentation links

- Pattern: `[link text](/help/user-guide/section/page.md#anchor)`
- Prefer anchors; link the phrase users care about, not “click here”.

### Fixes and enhancements

- Bullet lines use `*`.
- Only items explicitly labeled fix/enhancement in source material.
- Same link and terminology conventions as features.

## Prohibited content

- Do **not** include Jira keys, internal issue numbers, internal-only URLs, or corporate wiki links in published release notes.
- Do **not** cite Knowledge Transfer documents, tickets, or internal tools as proof—summarize user-facing outcomes only.
- Do **not** duplicate `{#latest}` on multiple sections.

## Quality checks

Before completing the task:

- [ ] **Scope:** Only the `## … {#latest}` block was added to or edited; **Earlier release notes** and older monthly sections were not modified except for the [Archive previous latest](#archive-previous-latest) cut/paste of the former `{#latest}` into a **new** archive block.
- [ ] All new or changed relative links resolve to real paths under `help/` where possible.
- [ ] Beta features include the Beta badge snippet where required.
- [ ] Terminology matches existing release notes (`[!DNL …]`, `[!UICONTROL …]`).
- [ ] Scan the draft for accidental internal IDs (`[A-Z]+-\d+`), wiki URLs, or “see Jira” language; remove them.
- [ ] **Fixes and enhancements** contains only explicitly labeled fixes/enhancements.
- [ ] Previous latest section archived correctly when a new month was added.

## Content sources (summary)

When **Jira/Confluence MCP** is available, start with [consume-release-sources](../consume-release-sources/SKILL.md) (ceremony wiki → KT pages → structured handoff). Otherwise map pasted Knowledge Transfer or release wiki fields as described in [reference.md](reference.md#internal-sources-kt-and-release-wikis). The shipped page must read as standalone user documentation.

## Optional: polish new subsections

After you add new `###` content under `{#latest}`, run [Polish release notes](../polish-release-notes/SKILL.md) for a copyeditor-style pass (benefit-forward tone, **2–3 sentences per paragraph**, no procedural how-to) **only** on those **new** subsections—**not** on Earlier release notes or pre-existing text unless explicitly requested.

## Additional resources

- [examples.md](examples.md) — paste-ready examples (features, fixes, archival block).
- [reference.md](reference.md) — frontmatter notes, doc paths, linking strategy.
- [Polish release notes](../polish-release-notes/SKILL.md) — optional editorial pass on newly added `###` under `{#latest}`.
