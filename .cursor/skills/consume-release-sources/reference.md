# Reference: consume release sources (MCP)

## Ceremony page discovery

| Pattern | Example |
|---------|---------|
| Title | `YYYY/MM Release Ceremony` in **GenStudio** space |
| From Jira | Wiki link in ticket `description` (preferred) |
| CQL fallback | `title ~ "2026/06 Release Ceremony" AND space = GenStudio` |

## Ceremony feature groups

Release ceremony wikis contain up to **two** feature tables. Parse both from **storage** HTML.

### GA Release Features

- Section heading: `GA Release Features` (`<h2>`)
- Subheading: `Feature Group:` with optional Floodgate link
- Table columns include **Type** (`GA`, `Limited`, `EA`, `Beta`, or empty)
- **KT Documentation** column: `<ac:link><ri:page ri:content-title="..."/></ac:link>`

Per row extract:

| Field | Source |
|-------|--------|
| `featureDescription` | First `<td>` in data row |
| `type` | Type column cell text |
| `ktPageTitle` | `ri:content-title` in KT column |
| `jiraKeys` | `ac:macro ac:name="jira"` → `key` parameter (internal only) |
| `releaseTier` | `ga` when Type is `GA`; inherit Type for other GA-table values |

### Beta Release Features

- Section heading: `Beta Release Features` (may be **absent** on some months)
- Second table; **no Type column** — every row is Beta
- Same KT and Jira extraction as GA table
- Set `releaseTier: beta` and `requiresBetaBadge: true` on every Beta-section row

If the Beta section is missing, log zero Beta rows and continue.

### Storage HTML patterns

```html
<ac:link><ri:page ri:content-title="Translation on HZ Canvas" /></ac:link>
<ac:structured-macro ac:name="jira" ...><ac:parameter ac:name="key">GS-23218</ac:parameter></ac:structured-macro>
```

## MCP tool usage

| Step | Tool | Parameters |
|------|------|------------|
| Ticket | `jira_getIssue` | `issueKey`, optional `expand: renderedFields` |
| Ceremony | `confluence_getContent` | `contentId`, `bodyMode: storage` |
| KT lookup | `confluence_searchContent` | `cql: title = "<KT title>" AND space = GenStudio` |
| KT body | `confluence_getContent` | `contentId`, `bodyMode: text`, `maxBodyChars: 50000` |

**Do not** use `bodyMode: text` for ceremony pages when parsing KT links.

## KT field mapping (drafting inputs)

Map into generate-release-notes; do not paste into public release notes verbatim.

| KT section | Use |
|------------|-----|
| Description | Core capability |
| Elevator pitch | Value proposition |
| Feature(s) delivered | Concrete behavior |
| Problem statement | User pain (context only) |
| Release Type & Date | GA / Beta / Limited (internal); drives badge decision |

## Inclusion filters

Confirm scope with the user when unclear. Common presets:

| Preset | Includes |
|--------|----------|
| `ga_only` | GA table rows where Type = `GA` |
| `ga_and_beta` | **Recommended default for future months** — GA rows where Type = `GA` **plus all** Beta Release Features table rows |
| `ga_plus_empty` | GA table: Type = `GA` or empty Type |
| `all_except_pilot` | GA table rows except `Limited`; plus Beta section when using `ga_and_beta` |
| `all_with_badges` | All GA-table rows; Beta section rows always get Beta badge |

## Beta badge handoff

| Condition | `requiresBetaBadge` |
|-----------|---------------------|
| Row from **Beta Release Features** table | `true` |
| GA table row with Type = `Beta` | `true` |
| GA table row with Type = `GA` | `false` |

Downstream: [generate-release-notes Decision rules](../generate-release-notes/SKILL.md#decision-rules) and [Beta badge snippet](../generate-release-notes/SKILL.md#beta-badge).

## Handoff payload (informal)

Pass to generate-release-notes as a list of items:

```yaml
- featureDescription: "YouTube Shorts"
  releaseTier: ga
  requiresBetaBadge: false
  ktPageTitle: "YouTube Shorts (Create + Activate)"
  # extracted KT fields: description, elevatorPitch, featuresDelivered, ...
```
