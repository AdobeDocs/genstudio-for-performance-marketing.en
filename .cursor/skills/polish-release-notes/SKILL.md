---
name: polish-release-notes
description: >-
  Editorial polish pass for Adobe GenStudio for Performance Marketing release
  notes: refines only newly added ### subsections under the current
  ## YYYY.MM {#latest} block in help/user-guide/release-notes.md. Copywriter
  tone (benefit-forward, energetic but accurate), 2–3 sentences per paragraph,
  no procedural how-to. Preserves ExL shortcodes and doc links.
---

# Polish GenStudio release notes

**Canonical target file:** [help/user-guide/release-notes.md](../../../help/user-guide/release-notes.md)

**Examples:** [examples.md](examples.md)

**Drafting workflow (upstream):** [generate-release-notes](../generate-release-notes/SKILL.md)

## Scope (required)

Polish **only** content the user identifies as **newly added** this round:

- **In file:** `###` subsections under the single heading `## YYYY.MM {#latest}` in `help/user-guide/release-notes.md`.
- **Do not** edit the page title, intro paragraph, frontmatter, or any text under **Earlier release notes** (collapsible `+++` blocks).
- **Do not** edit prior `##` monthly blocks or pre-existing `###` in the same `{#latest}` section unless the user **explicitly** asks.
- If it is unclear which `###` are new, **ask** or use **git diff** / edit context before changing prose.
- **Pasted content:** only polish markdown the user pastes when they confirm it matches those **same** new subsections (do not treat unrelated paste as in-scope).

Keep diffs **minimal**: wording and paragraph breaks only—no drive-by refactors elsewhere in the file.

## Voice and tone

- Write as a **copywriter** for product release notes: **concise**, **scannable**, and **energized** about **new value**—lead with outcomes and “what’s in it for you,” use strong verbs and crisp benefit language.
- **Stay accurate:** no claims beyond what the feature delivers; match Experience League / Adobe tone (confident and clear, not sensationalist).
- **Generate excitement** with **specific** benefits and deltas (what marketers can do now, what friction is removed)—not empty hype or unsubstantiated superlatives.

## Paragraph rules

- Each paragraph: **2–3 sentences**. **Never more than three sentences** in one paragraph—if you need more, start a **new paragraph**.
- Optional: if a paragraph still runs longer than **~3 lines** in rendered docs at typical line length, split further.

## Do not add

- **Procedural “how to”** content: numbered steps, “click **[!UICONTROL …]** then…”, full UI walkthroughs, or tutorial phrasing. Release notes summarize **what shipped** and **why it matters**, not hands-on lessons.
- Content that violates [Prohibited content](../generate-release-notes/SKILL.md#prohibited-content) on the generate skill (no Jira keys, internal-only URLs, wiki-as-proof, etc.).

## Preserve (do not strip or rewrite structurally)

- `[!DNL …]`, `[!UICONTROL …]`, `[!BADGE …]`, and other ExL shortcodes.
- Existing **relative** documentation links and anchor patterns: `[phrase](/help/...)` on meaningful anchor text.
- Beta badge blocks exactly as used in [generate-release-notes examples](../generate-release-notes/examples.md).

## Workflow checklist

1. [ ] Confirm **which** `###` under `## … {#latest}` are in scope (new this round).
2. [ ] For each in-scope `###`, tighten copy per [Voice and tone](#voice-and-tone) and [Paragraph rules](#paragraph-rules).
3. [ ] Remove or shorten any **how-to** instructions; keep **user outcomes**.
4. [ ] Verify links and shortcodes still valid; run a quick scan for internal IDs or banned patterns per [Quality checks](#quality-checks).

## Quality checks

- [ ] Only the agreed **new** `###` blocks under `{#latest}` changed; archives and older months untouched.
- [ ] No new Jira-style IDs, internal wiki URLs, or “see ticket” language.
- [ ] Paragraphs are **2–3 sentences** each (max three sentences per paragraph).
- [ ] Copy stays **factual** and aligned with the described capability.

## Additional resources

- [examples.md](examples.md) — before/after patterns.
- [generate-release-notes](../generate-release-notes/SKILL.md) — drafting, archival, Beta badges, linking.
