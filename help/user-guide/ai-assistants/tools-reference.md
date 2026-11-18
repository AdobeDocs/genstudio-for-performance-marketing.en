---
title: AI Assistant Tools Reference
description: Learn about the Insights, Create, Plan, Activate, and feedback tools an AI assistant can use with [!DNL GenStudio for Performance Marketing].
role: User
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
    internal-label: GenStudio for Performance Marketing
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
---

# AI assistant tools reference

This reference describes the tools that a connected AI assistant can use with [!DNL GenStudio for Performance Marketing]. The available tool list depends on your organization's configuration.

Ask your AI assistant which tools it can access before starting a workflow.

## Capability areas

| Area | Purpose | Behavior |
|---|---|---|
| Insights | Query paid media and email performance and retrieve creative recommendations. | Read only. |
| Create | Find assets, assemble drafts from Express templates or Insights recommendations, then manage review. | Read and write. Creates documents in Creative Cloud. |
| Plan | Extract campaign details from a brief and save them to Workfront Planning. | Extracting is read only. Saving creates records in Workfront Planning and cannot be rolled back automatically. |
| Activate | Resolve a publishing target and send an approved experience to the platform. | Write. Ads are sent to the platform and published in an off state. You turn them on separately. Not reversible through these tools. |
| Feedback | Send product feedback to the [!DNL GenStudio for Performance Marketing] team. | Write. |

Most Insights tools cover `meta`, `linkedin`, and `innovid`. Metric value tools cover `meta` and `linkedin`. Email campaign reporting covers Adobe Journey Optimizer (`ajo`) and Adobe Campaign (`acc`).

Create supports `meta`, `linkedin`, `display`, `tiktok`, and `youtube`. Activate supports `META`, `LINKEDIN`, and `GOOGLECM360`.

## Insights tools

### get_insights_capabilities

Returns the Insights channels and reporting operations enabled for your organization. Use this tool first when availability is unclear. The supported channels are `meta`, `linkedin`, `innovid`, `ajo`, and `acc`.

This tool returns capability metadata, not campaign, ad, or metric values. To find your organization's custom metric keys, use `list_connected_channels_and_metrics`.

### list_connected_channels_and_metrics

Returns your organization's active Meta, LinkedIn, and Google Campaign Manager 360 connections, the supported Insights channels and operations, and the configured custom conversion metrics. Use it to find metric keys before calling `get_insights_metric_values`.

This tool returns metric keys, labels, and formats, not metric values. A connection does not guarantee that historical reporting data is available.

| Parameter | Required | Description |
|---|---|---|
| `limit`, `offset` | No | Page size and paging offset. Omit both to return the complete catalog. |

### get_insights_summary

Returns headline performance metrics and trends for one channel over a selected date range.

| Parameter | Required | Description |
|---|---|---|
| `channel` | Yes | `meta`, `linkedin`, or `innovid`. |
| `startDate` | No | Start date in `YYYY-MM-DD` format. The default is 30 days ago. |
| `endDate` | No | End date in `YYYY-MM-DD` format. The default is today. |
| `metrics` | No | Metrics to chart: `spend`, `ctr`, `cpc`, `cpm`, `cpa`, `impressions`, `clicks`, `conversions`, `videoPlays`, `engagement`, `likes`, `comments`, or `shares`. The default is `spend`, `ctr`, `cpc`, and `cpm`. |

### list_insights_campaigns

Returns a sortable table of campaign performance metrics and a totals row.

| Parameter | Required | Description |
|---|---|---|
| `channel` | Yes | `meta`, `linkedin`, or `innovid`. |
| `startDate`, `endDate` | No | Date range in `YYYY-MM-DD` format. The default is the last 30 days. |
| `search` | No | Campaign name filter. |
| `sortBy` | No | Sort field: `spend`, `impressions`, `clicks`, `ctr`, `cpc`, `cpm`, or `name`. The default is `spend`. Results are always sorted in descending order. |
| `limit`, `offset` | No | Page size and paging offset. The default page size is 20. |

### list_insights_email_campaigns

Returns a sortable table of email campaigns with delivery and engagement metrics for Adobe Journey Optimizer and Adobe Campaign. For advertising campaigns, use `list_insights_campaigns`.

| Parameter | Required | Description |
|---|---|---|
| `channel` | Yes | `ajo` or `acc`. |
| `startDate`, `endDate` | No | Date range in `YYYY-MM-DD` format. The default is the last 30 days before the end date. |
| `search` | No | Campaign name filter. |
| `sortBy` | No | Sort field: `campaignName`, `emailsNumber`, `emailsDelivered`, `totalClicks`, `openRate`, `ctr`, `ctor`, `bounceRate`, `unsubscribeRate`, or `spamComplaintRate`. The default is `emailsDelivered`. Results are always sorted in descending order. |
| `limit`, `offset` | No | Page size and paging offset. |

### list_insights_ads

Returns ad-level performance. Use the default browse mode for a sortable table or a tier mode for high- and low-performing ads.

| Parameter | Required | Description |
|---|---|---|
| `channel` | Yes | `meta`, `linkedin`, or `innovid`. |
| `tier` | No | `all`, `high`, or `low`. The default is `all`. |
| `mainMetric` | No | Ranking metric for `high` or `low` tier mode: `ctr`, `cpc`, `cpm`, `cpa`, `spend`, `impressions`, or `clicks`. Ignored in browse mode. |
| `metrics` | No | Additional metrics to report for each ad in tier mode. |
| `campaigns` | No | Campaigns used to limit the result, up to 50. Each campaign includes `channel`, `accountId`, and `campaignId`. |
| `search` | No | Ad name filter. |
| `sortBy` | No | Browse mode sort field: `spend`, `impressions`, `clicks`, `ctr`, `cpc`, `cpm`, or `name`. The default is `spend`. Results are always sorted in descending order. |
| `spendMin`, `spendMax` | No | Total spend bounds for each ad. Tier mode only. |
| `includeUnsupported` | No | Includes ads whose creative can't be rendered. The default is `false`. |
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
| `ads` | Yes | One to 200 ads to explain. Each ad includes `channel`, `accountId`, `campaignId`, and `adId`, and optionally `adGroupId` and `performanceTier` (`high` or `low`). Use the identifiers returned by `list_insights_ads` in tier mode. |
| `mainMetric` | Yes | The metric used to rank the ads: `ctr`, `cpc`, `cpm`, `cpa`, `spend`, `impressions`, or `clicks`. |
| `campaigns` | No | Campaigns used to define the comparison population, up to 50. Each campaign includes `channel`, `accountId`, and `campaignId`. |
| `spendMin`, `spendMax` | No | Spend bounds for the comparison population. |
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
| `tagSource` | No | `ad_tags` or `campaign_tags`. The default is `ad_tags`. |
| `sortBy` | No | Sort field: `adsCount`, `spend`, `impressions`, `clicks`, `conversionCount`, `ctr`, `cpc`, `cpm`, or `cpa`. The default is `adsCount`. |
| `search` | No | Tag value filter. |
| `startDate`, `endDate` | No | Date range in `YYYY-MM-DD` format. |
| `limit`, `offset` | No | Page size and paging offset. |

### get_insights_metric_values

Returns the values and trends for your organization's tracked metrics, such as prospects, sign-ups, or return on ad spend, for Meta and LinkedIn.

| Parameter | Required | Description |
|---|---|---|
| `channels` | No | `meta`, `linkedin`, or both. |
| `metrics` | No | Up to 20 metric keys returned by `list_connected_channels_and_metrics`. The default is your organization's default visible set. |
| `campaigns` | No | Campaigns used to limit the result, up to 50. Each campaign includes `channel`, `accountId`, and `campaignId`. |
| `startDate`, `endDate` | No | Date range in `YYYY-MM-DD` format. The default is the last 30 days. |

### get_insights_recommendations

Returns proposed creative changes grounded in your organization's performance data. A request can return no recommendations when the selected scope contains no eligible ads.

| Parameter | Required | Description |
|---|---|---|
| `channels` | Yes | One or more of `meta`, `linkedin`, or `innovid`. |
| `campaigns` | No | Campaigns used to limit the result, up to 50. Each campaign includes `channel`, `accountId`, and `campaignId`. |
| `search` | No | Campaign name filter. |
| `recommendationId` | No | The `adUid` of one recommendation, used to retrieve it in detail. |
| `onlyWithPreview` | No | Excludes recommendations that have no example creative preview. The default is `true`. |
| `limit`, `offset` | No | Page size and paging offset. |

## Create tools

Create tools find assets, assemble drafts from Adobe Express templates, and manage review before an experience is ready to activate.

### list_express_templates

Lists available Express templates with filtering and facet counts.

| Parameter | Required | Description |
|---|---|---|
| `channel` | No | `meta`, `display`, `linkedin`, `tiktok`, `youtube`, or `__unspecified__`. |
| `query` | No | Search term for templates. |
| `activatableMimeType`, `aspectRatios`, `externalTemplateSource`, `isHTML5Template`, `keywords`, `languages`, `mediaFormat`, `regions`, `timeframes` | No | Template facet filters. |
| `sortBy` | No | `modified` or `created`. The default is `modified`. |
| `order` | No | `asc` or `desc`. The default is `desc`. |
| `limit`, `offset` | No | Page size and paging offset. |

### describe_express_template

Returns the editable text fields and image placements in a template.

| Parameter | Required | Description |
|---|---|---|
| `templateId` | Yes | Express template identifier. |

### list_cta_options

Returns the allowed call-to-action values for a channel. Display returns an empty list because it accepts free-form text.

| Parameter | Required | Description |
|---|---|---|
| `channel` | Yes | `linkedin`, `meta`, `display`, `tiktok`, or `youtube`. |
| `limit`, `offset` | No | Page size and paging offset. Omit both to return every option. |

### search_assets

Searches the images and videos in your GenStudio Content. Use it to select existing assets for a draft. Derived, external, and expired assets are excluded. This tool does not upload, edit, delete, or generate assets, and it requires GenStudio Content entitlement.

| Parameter | Required | Description |
|---|---|---|
| `query` | No | Keyword or natural-language search across asset metadata. |
| `mediaTypes` | No | `image`, `video`, or both. The default includes both. |
| `aspectRatios` | No | Aspect ratios such as `1:1` or `16:9`. If a ratio is unavailable, the tool returns the available choices. |
| `brands`, `campaigns`, `products`, `personas`, `channels` | No | Filters by name. |
| `customMetadata` | No | Up to 5 metadata fields, each with one or more values. |
| `uploadedBy` | No | `me` or an uploader email address. |
| `createdAtFrom`, `createdAtTo` | No | Creation time bounds in ISO 8601 format. |
| `aiGenerated` | No | Filters by AI-generation status. |
| `contentCredentials` | No | Filters by Content Credentials status. |
| `limit`, `offset` | No | Page size and paging offset. |

The result includes stable asset references for `create_draft` and short-lived signed URLs.

### create_draft

Creates an editable draft from an Express template with one or more experiences. Each call creates a new draft.

| Parameter | Required | Description |
|---|---|---|
| `templateId` | Yes | Express template identifier. |
| `prompt` | Yes | Creative brief and copy instructions stored with the draft. |
| `experiences` | Yes | One or more experiences. See the following table. |
| `name` | No | Document name. |
| `allowAssetReuse` | No | Allows one selected asset to be reused across multiple experiences. The default is `false`. |

Each experience supports these fields:

| Field | Required | Description |
|---|---|---|
| `channel` | Yes | `linkedin`, `meta`, `display`, `tiktok`, or `youtube`. |
| `title` | No | Experience title. The default is "Concept *n*". |
| `headline` | Meta and LinkedIn | Primary headline. |
| `body` | Meta, LinkedIn, and TikTok | Body copy. For LinkedIn, this is the introductory text. For TikTok, this is the primary text. |
| `description` | YouTube | Ad description. Optional for Meta and LinkedIn. |
| `display_url` | Meta and LinkedIn | Display URL shown in the ad. |
| `destination_url` | No | URL that the ad links to. |
| `cta` | No | Call-to-action text from `list_cta_options`. |
| `templateFields` | No | Overrides for named template elements from `describe_express_template`. Each override sets text, an image URL with dimensions, or a video URL. |
| `assetTemplateFields` | No | Content assets from `search_assets` for image or video fields in the template. |

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
| `emails` | Yes | One to 20 collaborator email addresses. |
| `role` | Yes | `editor` or `viewer`. |
| `message` | No | Invitation message. |

### request_draft_approval

Sends a draft to one or more people for approval.

| Parameter | Required | Description |
|---|---|---|
| `draftId` | Yes | Draft asset identifier. |
| `emails` | Yes | One to 20 reviewer email addresses. |

### list_experiences

Returns approved, published experiences that are ready to activate. Drafts are not included.

| Parameter | Required | Description |
|---|---|---|
| `channel` | No | `email`, `meta`, `meta_organic`, `display`, `ctv`, `linkedin`, `linkedin_organic`, `tiktok`, `chatgpt`, or `youtube`. |
| `createdByMe` | No | Limits results to experiences created by the current user. |
| `campaignNames` | No | Up to 5 exact campaign name filters. |
| `creatorEmail` | No | Creator email filter. |
| `createdAtFrom`, `createdAtTo` | No | Creation date bounds. |
| `language` | No | BCP 47 language tag. |
| `limit`, `cursor` | No | Page size (1–50, default 20) and pagination cursor. |

## Plan tools

Plan tools turn a campaign brief into a reviewable campaign draft and save it to Workfront Planning.

### extract_campaign_from_brief

Extracts a reviewable campaign draft from one pasted marketing brief. This tool does not save any records. Missing facts and dates are not inferred.

| Parameter | Required | Description |
|---|---|---|
| `briefText` | Yes | The full plain text of one campaign brief, up to 100,000 characters. Files and links are not supported. |

The result includes a campaign draft, findings with supporting quotes, suggested audiences, and warnings.

### create_workfront_campaign

Creates a Workfront Planning campaign with linked products and personas from a draft that you reviewed and approved. This tool is not idempotent, and records can't be rolled back automatically. Inspect Workfront before retrying a write that might have succeeded.

| Parameter | Required | Description |
|---|---|---|
| `campaignDraft` | Yes | The approved draft. Requires `name`. Optional fields are `description`, `objective`, `keyMessaging`, `startDate`, `endDate` (`YYYY-MM-DD`), `status`, `channels`, `products`, and `personas`. |
| `channelSelections` | No | Approved choices for ambiguous channel names. |
| `entitySelections` | No | Approved existing product and persona records. Use `null` to request a new record. |
| `createMissingEntities` | No | Creates the products and personas that you selected as new. The default is `false`. |

If a product, persona, or channel is ambiguous, the tool returns choices to confirm and makes no changes.

## Activate tools

Activate tools resolve a paid media target and send an approved experience to the platform. Ads are published in an off state (Meta paused, LinkedIn draft, Campaign Manager 360 inactive), so you must turn them on separately before they deliver. Sending ads to the platform is not reversible through these tools.

### configure_activation_target

Resolves and validates the paid media account, campaign, ad set, and Facebook Page when required.

| Parameter | Required | Description |
|---|---|---|
| `platform` | Yes | `META`, `LINKEDIN`, or `GOOGLECM360`. |
| `platformAccountId` | No | Paid media account identifier. Omit it to discover accounts. |
| `campaignId` | No | Campaign identifier for Meta or LinkedIn. Not used for Campaign Manager 360. |
| `adsetId` | No | Meta ad set or LinkedIn campaign identifier. Not used for Campaign Manager 360. |
| `pageId` | No | Facebook Page identifier for Meta. |

For Campaign Manager 360, only the ad account is required.

### create_activation

Sends an approved experience to the platform as ads, using a validated target. The ads are published in an off state. Meta creates one ad with the first image for each aspect ratio. LinkedIn and Campaign Manager 360 create one ad for each resolved image.

| Parameter | Required | Description |
|---|---|---|
| `platform` | Yes | `META`, `LINKEDIN`, or `GOOGLECM360`. |
| `targetId` | Yes | Validated target returned by `configure_activation_target`. |
| `experienceId` | Yes | Approved experience identifier returned by `list_experiences`. |
| `name` | No | Ad placement display name. The default is the experience's ad title. |

The result lists the number of ads created, queued, and skipped, with each ad's initial status and a link to it in [!DNL GenStudio for Performance Marketing]. A status of `PENDING` means the job is queued, not that the ad is delivering.

Calling `create_activation` twice creates additional ads instead of updating the first ads.

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
- **Review tracked metrics:** Call `list_connected_channels_and_metrics`, then call `get_insights_metric_values` with returned metric keys.
- **Turn a recommendation into a draft:** Call `get_insights_recommendations`, then call `create_draft_from_recommendation`.
- **Build from a template:** Call `list_express_templates`, `describe_express_template`, and `list_cta_options`, then call `create_draft`.
- **Build from existing assets:** Call `search_assets`, then pass the returned asset references to `create_draft` in `assetTemplateFields`.
- **Save a campaign brief to Workfront:** Call `extract_campaign_from_brief`, review the draft, then call `create_workfront_campaign`.
- **Send an approved experience to a platform:** Call `list_experiences`, then call `configure_activation_target` and `create_activation`.

## Related capabilities

- [AI assistants overview](overview.md)
- [Connect an AI assistant](connect-ai-assistants.md)
- [Use AI assistants](use-ai-assistants.md)
