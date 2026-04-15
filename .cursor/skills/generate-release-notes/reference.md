# Reference: release notes authoring

## Frontmatter

The live page [help/user-guide/release-notes.md](../../help/user-guide/release-notes.md) includes Experience League metadata beyond a minimal set (for example `TQID`, `product_v2`, `feature_v2`, taxonomy IDs).

**Rules:**

- When editing release note **body** content, **preserve existing frontmatter** keys and values unless the task explicitly asks to change metadata.
- Do not strip taxonomy or product metadata to match a shorter template.
- Required concepts for ExL pages generally include `title`, `description`, and `role`; follow [Experience League metadata guidance](https://experienceleague.adobe.com/en/docs/authoring-guide/using/authoring/using-metadata) for new pages.

## Internal sources (KT and release wikis)

Use these fields **only while drafting**; the published release notes must not reference internal docs.

### Knowledge Transfer (KT) documents

Extract from:

| Field | Use |
|-------|-----|
| Description | Core feature explanation |
| Elevator Pitch | Value proposition |
| Feature(s) Delivered | Concrete behavior |
| Problem Statement | User pain point |
| Release Type & Date | Timing |

### Release wiki pages

Group and scope by:

| Field | Use |
|-------|-----|
| Release Date (Fix Version) | Same date → same release notes batch |
| Initiative | Context only; do not link internally in public text |
| PM presents the feature using KT | Signals deeper KT detail may exist |

**Scope rule:** Items that share the same Release Date (Fix Version) belong in the same monthly release block.

## Documentation linking

- Link to the **most relevant** phrase (e.g., link “unsupported image and video assets” to the ad formats section).
- Prefer `#anchor` links into the right subsection.
- Overview pages are acceptable when no deeper anchor exists.

## Common documentation paths

| Area | Path prefix |
|------|-------------|
| Create | `/help/user-guide/create/` |
| Content | `/help/user-guide/content/` |
| Activation | `/help/user-guide/activation/` |
| Approvals | `/help/user-guide/approvals/` |
| Insights | `/help/user-guide/insights/` |
| Guidelines | `/help/user-guide/guidelines/` |
| Templates | `/help/user-guide/templates/` |
| Campaigns | `/help/user-guide/campaigns/` |
| Extensibility | `/help/extensibility/` |
