---
title: Experiences overview
description: See an overview of customer engagement, budget, and expenditures for experiences and ad placement performance in Adobe GenStudio for Performance Marketing.
feature: Insights, Experiences, Attributes
exl-id: e3827b1a-53d0-465c-8125-15b0e298ef3a
---
# Experiences overview

The [!DNL Insights] _[!UICONTROL Experiences]_ view shows a list of experiences for the connected channel ad account. For Facebook, the experiences are Meta ad names.

{{connect-insights}}

The _[!UICONTROL Experiences]_ table is organized using [!UICONTROL Ad names]. Click the settings (cog) icon above the right side of the table to toggle the viewable columns. The filter (funnel) icon above the left side of the table opens the **[!UICONTROL Filter]** menu where you can select from the [!UICONTROL Account] and [!UICONTROL Campaign] lists to filter the ad names in the table. Click **Reset** to clear all filter selections.

![Experiences filter and table](/help/assets/insights-experiences-filter.png){zoomable="yes"}

{{$include /help/_includes/download-insights.md}}

## Experience details

An _experience_ is a promotional asset that includes visual and interactive content intended for distribution to a specific audience as part of a marketing campaign.

Select an experience and view the performance metrics, text attributes, and placements associated with each ad. In the details view, you can analyze an experience's metrics based on its ad placement and marketing efforts within a specified date range.

The details view includes a metrics overall ad `click-through rate`, `cost per action`, and `spend`—how much of the budget has been on the ad. Since ads can have multiple placements, such as a feed or a banner, you can see a breakdown of the same metrics for each ad placement. Use the left and right arrows under **[!UICONTROL Performance by ad placement]** to cycle through the placement metrics.

![Ad details with metrics and ad placements](/help/assets/insights-experience-details.png){zoomable="yes"}

### Text attributes

Below the experience preview is a list of [!UICONTROL Text attributes] associated with the ad. When assets and experiences are approved and stored in [!DNL Content], GenStudio for Performance Marketing generates tags based on their inherent features. See [Asset details](/help/user-guide/content/asset-details.md#system-metadata) for details about system metadata.

### Ad placements

At the time that you created a campaign with Meta ads, you may have selected where to run your ads based on the campaign [objective](channels.md#objectives). Ad placements broaden the audience reach for your ad.

GenStudio for Performance Marketing supports ad formats, such as asset feeds, link ads, and single image or video. The following is a list of ad formats by platform:

| Instagram    | Facebook/Meta    | Messenger    | Audience Network |
| ------------ | ---------------- | ------------ | ---------------- |
| Explore<br>Explore home<br>Explore grid Home<br>Feed<br>Reels<br>Profile feed<br>Search<br>Shop<br>Stories | Business Explore<br>Feed<br>In-stream video<br>Marketplace<br>Reels<br>Reels overlay<br>Right column<br>Search results<br>Stories<br>Video feeds<br>Ads on Facebook reels | Inbox<br>Stories | Native, banner, and interstitial<br>Rewarded video |

#### Unsupported placements

GenStudio for Performance Marketing does not support the following ad placements:

- Collaborative
- Catalog/Advantage+ catalog
- Instance Experience
- Carousel

## Experience performance

Insights metrics can help you evaluate which experiences contribute to the success of a campaign and which ad placements are most effective.

The following table provides definitions and insights for key digital marketing metrics in the [!UICONTROL Experiences] table view. Each metric includes a brief definition as it relates to ad names, how the metric is calculated, and one or more insights to help understand its significance and impact on an experience.

| Metric                 | Definition                    | Insight                          |
| ---------------------- | ----------------------------- | -------------------------------- |
| **[!UICONTROL Experience name]** | A list of experiences for the connected channel account. Filter ads by selecting a campaign. | Sort the experience list by clicking on any of the key metrics. |
| **[!UICONTROL Campaign]**  | A campaign is a set of experiences designed to achieve a specific objective. | When you filter the Experiences table by campaign, the summary metrics of all experiences for the campaign may be different than the campaign's summary row in the [!UICONTROL Channels] view. This discrepancy can occur if the channel source, such as Meta, and GenStudio use slightly different summary calculations. |
| **[!UICONTROL Placements]** | A count of ad [placements](#ad-placements), locations where an experience appeared in the campaign. | Placements increase audience reach.<p>Ads that show zero placements and zero assets may indicate an [unsupported ad type](#unsupported-placements).</p> |
| **[!UICONTROL Assets]** | The number of assets used in the ad or experience. | The count in the Experiences table may be different than the count in the Experience details view. This discrepancy can occur if the channel source, such as Meta, and GenStudio use slightly different summary calculations. |
| **[!UICONTROL Impressions]** | A count of each time the ad placement or experience loads in the channel, regardless of interaction or viewing. | A high impression count can indicate broad visibility, but for true performance insight, consider it in relation with other engagement metrics. |
| **[!UICONTROL Clicks]**      | The number of times users interact with a clickable element, such as a link or a call-to-action button, in an experience placement. | A high click count indicates strong interest and engagement with the content, which may be effective and reaching the right audience. |
| **[!UICONTROL CTR]**<br>_Click-through rate_ | Percentage (%) of impressions that resulted in clicks on the experience placement within a campaign.<br>**Calculation**: `clicks` divided by `impressions` | A high click-through rate indicates that the content is highly relevant and motivating to the audience in the messaging and design, and is effectively targeting the audience's interests. |
| **[!UICONTROL CPM]**<br>_Cost per thousand_ | Cost for every one thousand ad impressions for the experience placement.<br>**Calculation**: total amount `spent` divided by reach, then multiplied by 1000 | A low value may indicate cost-effective visibility, especially when paired with a high click-through rate. |
| **[!UICONTROL CPA]**<br>_Cost per Action_ | Average cost spent to achieve a specific customer action, such as a purchase or subscription.<br>**Calculation**: total amount `spent` divided by the number of customer actions completed | Use to monitor spending on experiences that result in valuable customer actions. |
| **[!UICONTROL CPC]**<br>_Cost per click_ | Average cost associated with each click in an experience placement.<br>**Calculation**: total amount `spent` divided by `clicks` | Lower average costs may indicate cost-efficient ad spend, especially when compared with a rise in conversions. |
| **[!UICONTROL Spend]**       | The amount spent from the Campaign budget over a given period of time to place this ad Experience. | A high spend amount in a short period may indicate rapid usage, which could lead to early depletion of resources. Track the amount spent against key performance metrics to help monitor the overall return on investment. |

## Placement performance

In the _Experience details_ view, the top three metrics reflect the overall performance of the selected experience. However, the _Performance by placement_ section shows the detailed metrics for each ad placement. Use the right and left arrows to navigate through the different ad placements.

The following table provides definitions for ad placement performance metrics:

| Metric                 | Definition                    | Insight     |
| ---------------------- | ----------------------------- | ----------- |
| **[!UICONTROL CTR]**<br>_Click-through rate_ | The percentage (%) of impressions for a single ad placement that resulted in clicks.<p>**Calculation**:`clicks` divided by `impressions`<p>This metric helps determine the effectiveness of the ad placement in engaging the audience. | A high CTR indicates that the ad placement is relevant and compelling to the audience, leading to more interactions. |
| **[!UICONTROL CPA]**<br>_Cost per Action_ | The average cost spent on a single ad placement to achieve a desired customer action, such as a purchase or subscription.<p>**Calculation**: total amount `spent` divided by the number of customer actions completed<p>This metric helps evaluate the cost-efficiency of the ad placement in driving valuable actions. | A lower CPA suggests that the ad placement is effective in converting audience interactions into desired actions at a lower cost. |
| **[!UICONTROL CPC]**<br>_Cost per click_ | The average cost associated with each click in a single ad placement.<p>**Calculation**: total amount `spent` divided by `clicks`<p>This metric helps assess the cost-effectiveness of the ad placement in generating clicks. | A lower CPC indicates that the ad placement is generating clicks at a lower cost, which can be beneficial for maximizing the return on investment. |
| **[!UICONTROL Spend]** | The amount spent on a single ad placement, representing a fraction of the total amount spent on the entire experience. This metric helps track the budget allocation and spending efficiency for each ad placement. | Monitoring spend can help ensure that resources are being used effectively across different placements. |
