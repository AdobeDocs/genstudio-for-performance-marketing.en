---
title: AI Assistant Tools Reference
description: Learn about the Insights, Create, Activate, and feedback tools an AI assistant can use with [!DNL GenStudio for Performance Marketing].
role: User
---

# AI assistant tools reference

This reference describes the tools that a connected AI assistant can use with [!DNL GenStudio for Performance Marketing]. The available tool list depends on your organization's configuration.

Ask your AI assistant which tools it can access before starting a workflow.

## Capability areas

| Area | Purpose | Behavior |
|---|---|---|
| Insights | Query paid media performance and retrieve creative recommendations. | Read only. |
| Create | Assemble drafts from Express templates or Insights recommendations, then manage review. | Read and write. Creates documents in Creative Cloud. |
| Activate | Resolve a publishing target and publish an approved experience. | Write and destructive. Can publish a live ad and incur ad spend. |
| Feedback | Send product feedback to the [!DNL GenStudio for Performance Marketing] team. | Write. |

Most Insights tools cover `meta`, `linkedin`, and `innovid`. Conversion metric tools cover `meta` and `linkedin`.

Create supports `meta`, `linkedin`, `display`, `tiktok`, and `youtube`. Activate supports `META`, `LINKEDIN`, and `GOOGLECM360`.

## Insights tools

### get_insights_capabilities

Returns the Insights channels, operations, and custom conversion metrics enabled for your organization. Use this tool first when availability is unclear.

This tool returns capability metadata, not campaign, ad, or metric values.

### get_insights_summary

Returns headline performance metrics and trends for one channel over a selected date range.

| Parameter | Required | Description |
|---|---|---|
| `channel` | Yes | `meta`, `linkedin`, or `innovid`. |
| `startDate` | No | Start date in `YYYY-MM-DD` format. The default is 30 days ago. |
| `endDate` | No | End date in `YYYY-MM-DD` format. The default is today. |
| `metrics` | No | Metrics to chart, such as `spend`, `ctr`, `cpc`, `cpm`, `impressions`, `clicks`, or `conversions`. |

### list_insights_campaigns

Returns a sortable table of campaign performance metrics and a totals row.

| Parameter | Required | Description |
|---|---|---|
| `channel` | Yes | `meta`, `linkedin`, or `innovid`. |
| `startDate`, `endDate` | No | Date range in `YYYY-MM-DD` format. The default is the last 30 days. |
| `search` | No | Campaign name filter. |
| `sortBy` | No | Sort field, such as `spend`, `impressions`, `clicks`, `ctr`, `cpc`, `cpm`, or `name`. |
| `limit`, `offset` | No | Page size and paging offset. |

### list_insights_ads

Returns ad-level performance. Use the default browse mode for a sortable table or a tier mode for high- and low-performing ads.

| Parameter | Required | Description |
|---|---|---|
| `channel` | Yes | `meta`, `linkedin`, or `innovid`. |
| `tier` | No | `all`, `high`, or `low`. The default is `all`. |
| `mainMetric` | Conditional | Ranking metric required for `high` or `low` tier mode. |
| `campaigns` | No | Campaign identifiers used to limit the result. |
| `search` | No | Ad name filter. |
| `startDate`, `endDate` | No | Date range in `YYYY-MM-DD` format. |
| `limit`, `offset` | No | Page size and paging offset. |

Tier mode returns the ad identifiers needed by `get_insights_ad_attributes`.

### get_insights_ad_details

Returns creative metadata for one ad, including copy, call to action, assets, and placements. It does not return performance metrics.

| Parameter | Required | Description |
|---|---|---|
| `channel` | Yes | `meta`, `linkedin`, or `innovid`. |
| `accountId` | Yes | Paid media account identifier. |
| `campaignId` | Yes | Campaign identifier. |
| `adId` | Yes | Ad identifier. |
| `adgroupId` | No | Ad group identifier when the channel uses ad groups. |

### get_insights_ad_attributes

Compares creative traits for selected ads with the channel average. Use it after `list_insights_ads` identifies high- or low-performing ads.

| Parameter | Required | Description |
|---|---|---|
| `ads` | Yes | Ads to explain, including the identifiers returned by `list_insights_ads`. |
| `mainMetric` | Yes | The metric used to rank the ads. |
| `campaigns` | No | Campaign identifiers used to define the comparison population. |
| `startDate`, `endDate` | No | Date range in `YYYY-MM-DD` format. |

### get_insights_tag_categories

Returns the tag categories available for your organization during the requested period. It returns category names, not performance metrics.

| Parameter | Required | Description |
|---|---|---|
| `channels` | Yes | One or more supported channels. |
| `startDate`, `endDate` | No | Date range in `YYYY-MM-DD` format. |

### get_insights_ad_tags

Returns performance by tag value within one category, such as product, region, or creative theme.

| Parameter | Required | Description |
|---|---|---|
| `channel` | Yes | `meta`, `linkedin`, or `innovid`. |
| `tagCategory` | Yes | A category returned by `get_insights_tag_categories`. |
| `tagSource` | No | `ad_tags` or `campaign_tags`. |
| `sortBy` | No | Metric used to sort the result. |
| `search` | No | Tag value filter. |
| `startDate`, `endDate` | No | Date range in `YYYY-MM-DD` format. |

### get_insights_custom_metrics

Returns the custom conversion metrics configured for your organization. Use it before `get_insights_conversion_metrics`.

This tool returns metric identifiers, not metric values.

### get_insights_conversion_metrics

Returns configured conversion metric values and trends for Meta and LinkedIn.

| Parameter | Required | Description |
|---|---|---|
| `channels` | No | Supported conversion channel. The default is `meta`. |
| `metrics` | No | Metric identifiers returned by `get_insights_custom_metrics`. |
| `campaigns` | No | Campaign identifiers used to limit the result. |
| `startDate`, `endDate` | No | Date range in `YYYY-MM-DD` format. |

### get_insights_recommendations

Returns proposed creative changes grounded in your organization's performance data. A request can return no recommendations when the selected scope contains no eligible ads.

| Parameter | Required | Description |
|---|---|---|
| `channels` | Yes | One or more supported channels. |
| `campaigns` | No | Campaign identifiers used to limit the result. |
| `search` | No | Campaign name filter. |
| `recommendationId` | No | Identifier used to retrieve one recommendation in detail. |
| `limit`, `offset` | No | Page size and paging offset. |

## Create tools

Create tools assemble drafts from Adobe Express templates and manage review before an experience is ready to activate.

### list_express_templates

Lists available Express templates with filtering and facet counts.

| Parameter | Required | Description |
|---|---|---|
| `channel` | No | `meta`, `display`, `linkedin`, `tiktok`, `youtube`, or `__unspecified__`. |
| `query` | No | Search term for templates. |
| `aspectRatios`, `keywords`, `languages`, `mediaFormat`, `regions`, `timeframes` | No | Template facet filters. |
| `sortBy`, `order` | No | Sort field and order. |
| `limit`, `offset` | No | Page size and paging offset. |

### describe_express_template

Returns the editable text fields and image placements in a template.

| Parameter | Required | Description |
|---|---|---|
| `templateId` | Yes | Express template identifier. |

### list_cta_options

Returns the allowed call-to-action values for a channel.

| Parameter | Required | Description |
|---|---|---|
| `channel` | Yes | `linkedin`, `meta`, `display`, `tiktok`, or `youtube`. |

### create_draft

Creates an editable draft from an Express template with one or more experiences.

| Parameter | Required | Description |
|---|---|---|
| `templateId` | Yes | Express template identifier. |
| `prompt` | Yes | Creative brief and copy instructions stored with the draft. |
| `experiences` | Yes | Channel, content fields, and optional template field overrides for each experience. |
| `name` | No | Document name. |

Use `list_cta_options` before creating a draft for a channel with fixed call-to-action values.

### create_draft_from_recommendation

Creates an editable draft from a specific Insights recommendation.

| Parameter | Required | Description |
|---|---|---|
| `channel` | Yes | `meta` or `linkedin`. |
| `adUid` | Yes | Recommendation identifier returned by `get_insights_recommendations`. |
| `prompt` | Yes | Creative brief based on the recommendation. |
| `name` | No | Document name. |

### list_recent_drafts

Lists recent Express template drafts with their status and links.

| Parameter | Required | Description |
|---|---|---|
| `limit`, `offset` | No | Page size and paging offset. |

### get_draft_metadata

Returns a draft's name, channels, approval status, reviewer outcomes, and collaborator access.

| Parameter | Required | Description |
|---|---|---|
| `draftId` | Yes | Draft asset identifier. |

### share_draft

Gives collaborators view or edit access to a draft without requesting approval.

| Parameter | Required | Description |
|---|---|---|
| `draftId` | Yes | Draft asset identifier. |
| `emails` | Yes | One or more collaborator email addresses. |
| `role` | Yes | `editor` or `viewer`. |
| `message` | No | Invitation message. |

### request_draft_approval

Sends a draft to one or more people for approval.

| Parameter | Required | Description |
|---|---|---|
| `draftId` | Yes | Draft asset identifier. |
| `emails` | Yes | One or more reviewer email addresses. |

### list_experiences

Returns approved, published experiences that are ready to activate. Drafts are not included.

| Parameter | Required | Description |
|---|---|---|
| `channel` | No | Experience channel filter. |
| `createdByMe` | No | Limits results to experiences created by the current user. |
| `campaignNames` | No | Exact campaign name filters. |
| `creatorEmail` | No | Creator email filter. |
| `createdAtFrom`, `createdAtTo` | No | Creation date bounds. |
| `language` | No | BCP 47 language tag. |
| `limit`, `cursor` | No | Page size and pagination cursor. |

## Activate tools

Activate tools resolve a paid media target and publish an approved experience. Publishing is not reversible through these tools and might incur ad spend.

### configure_activation_target

Resolves and validates the paid media account, campaign, ad set, and Facebook Page when required.

| Parameter | Required | Description |
|---|---|---|
| `platform` | Yes | `META`, `LINKEDIN`, or `GOOGLECM360`. |
| `platformAccountId` | No | Paid media account identifier. Omit it to discover accounts. |
| `campaignId` | No | Campaign identifier for Meta or LinkedIn. |
| `adsetId` | No | Meta ad set or LinkedIn campaign identifier. |
| `pageId` | No | Facebook Page identifier for Meta. |

### create_activation

Publishes a live, single-image ad from an approved experience and validated target.

| Parameter | Required | Description |
|---|---|---|
| `platform` | Yes | `META`, `LINKEDIN`, or `GOOGLECM360`. |
| `targetId` | Yes | Validated target returned by `configure_activation_target`. |
| `experienceId` | Yes | Approved experience identifier returned by `list_experiences`. |
| `assetId` | No | Variant identifier for an experience with multiple eligible variants. |
| `name` | No | Ad placement display name. |

Calling `create_activation` twice creates two separate ads instead of updating the first ad.

## Feedback tool

### submit_mcp_feedback

Sends feedback about a tool or workflow to the [!DNL GenStudio for Performance Marketing] team.

| Parameter | Required | Description |
|---|---|---|
| `category` | Yes | `bug`, `feature_request`, or `workflow_friction`. |
| `comment` | Yes | A concise description of the feedback. |
| `tags` | No | Tags used to categorize the feedback. |
| `tool_name` | No | The tool associated with the feedback. |

## Common workflows

Use these sequences when one tool supplies identifiers or configuration for another:

- **Diagnose an ad:** Call `list_insights_ads` in `high` or `low` tier mode, then call `get_insights_ad_attributes` with the same ranking metric.
- **Analyze by tag:** Call `get_insights_tag_categories`, then call `get_insights_ad_tags` with a returned category.
- **Review conversion metrics:** Call `get_insights_custom_metrics`, then call `get_insights_conversion_metrics` with returned metric identifiers.
- **Turn a recommendation into a draft:** Call `get_insights_recommendations`, then call `create_draft_from_recommendation`.
- **Build from a template:** Call `list_express_templates`, `describe_express_template`, and `list_cta_options`, then call `create_draft`.
- **Publish an approved experience:** Call `list_experiences`, then call `configure_activation_target` and `create_activation`.

## Related capabilities

- [AI assistants overview](overview.md)
- [Connect an AI assistant](connect-ai-assistants.md)
- [Use AI assistants](use-ai-assistants.md)
