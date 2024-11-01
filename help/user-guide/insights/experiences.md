---
title: Experiences overview
description: See an overview of customer engagement, budget, and expenditures for experiences and ad placement performance in Adobe GenStudio for Performance Marketing.
feature: Insights, Experiences
---
# Experiences overview

The [!DNL Insights] _[!UICONTROL Experiences]_ view shows a list of experiences for the connected channel ad account. For Facebook, the experiences are Meta ad names.

The _[!UICONTROL Experiences]_ table is organized using [!UICONTROL Ad names]. Click the settings (cog) icon above the right side of the table to toggle the viewable columns. The filter (funnel) icon above the left side of the table opens the **[!UICONTROL Filter]** menu where you can select from the [!UICONTROL Account] and [!UICONTROL Campaign] lists to filter the ad names in the table.

![Experiences filter and table](/help/assets/insights-experiences-filter.png){zoomable="yes"}

## Experience details

An _experience_ is a promotional asset that includes visual and interactive content intended for distribution to a specific audience as part of a marketing campaign.

Select an experience (ad name) and view the performance metrics, text attributes, and placements associated with each ad. In the details view, you can analyze an experience's metrics based on its ad placement and marketing efforts within a specified date range.

The details view includes a metrics overall ad `click-through rate`, `cost per action`, and `spend`—how much of the budget has been on the ad. Since ads can have multiple placements, such as a feed or a banner, you can see a breakdown of the same metrics for each ad placement. Use the left and right arrows under **[!UICONTROL Performance by ad placement]** to cycle through the placement metrics.

![Ad details with metrics and ad placements](/help/assets/insights-experience-details.png){zoomable="yes"}

### Text attributes

Below the experience preview is a list of [!UICONTROL Text attributes] associated with the ad. When assets and experiences are approved and stored in [!DNL Content], GenStudio for Performance Marketing generates tags based on their inherent features. See [Asset details](../content/asset-details.md#system-metadata) for details about system metadata.

### Ad placements

At the time that you created a campaign with Meta ads, you may have selected where to run your ads based on the campaign [objective](channels.md#objectives). Ad placements broaden the audience reach for your ad.

GenStudio for Performance Marketing supports ad formats, such as asset feeds, link ads, and single image or video. The following is a list of ad formats by platform:

| Instagram    | Facebook/Meta    | Messenger    | Audience Network |
| ------------ | ---------------- | ------------ | ---------------- |
| Explore<br>Explore home<br>Explore grid Home<br>Feed<br>Reels<br>Profile feed<br>Search<br>Shop<br>Stories | Business Explore<br>Feed<br>In-stream video<br>Marketplace<br>Reels<br>Reels overlay<br>Right column<br>Search results<br>Stories<br>Video feeds<br>Ads on Facebook reels | Inbox<br>Stories | Native, banner, and interstitial<br>Rewarded video |

#### Unsupported placements

GenStudio for Performance Metrics does not support the following ad placements:

- Collaborative
- Catalog/Advantage+ catalogue
- Instance Experience
- Carousel

## Experiences metrics

Insights metrics can help you evaluate which experiences contribute to the success of a campaign and which ad placements are most effective.

<!-- For example, -->

### Metrics detail

The following table provides definitions and insights for key digital marketing metrics in the [!UICONTROL Experiences] table view. Each metric includes a brief definition as it relates to ad names, how the metric is calculated, and one or more insights to help understand its significance and impact on an experience.

| Metric                 | Definition                    | Insight                          |
| ---------------------- | ----------------------------- | -------------------------------- |
| **[!UICONTROL Experience name]** | A list of experiences for the connected channel account. Filter ads by selecting a campaign. | Sort the experience list by clicking on any of the key metrics. |
| **[!UICONTROL Campaign]**  | A campaign is a set of experiences designed to achieve a specific objective. | |
| **[!UICONTROL Placements]** | A count of ad [placements](#ad-placements), locations where an experience appeared in the campaign. | Placements increase audience reach. |
| **[!UICONTROL Assets]** | A count of assets used in the ad or experience. | |
| **[!UICONTROL Impressions]** | A count of each time the ad placement or experience loads in the channel, regardless of interaction or viewing. | A high impression count can indicate broad visibility, but for true performance insight, consider with other engagement metrics. |
| **[!UICONTROL Clicks]**      | Number of times users interact with a clickable element, such as a link or a call-to-action button, in an experience placement. | A high click count indicates strong interest and engagement with the content, which may be effective and reaching the right audience. |
| **[!UICONTROL CTR]**<br>_Click-through rate_ | Percentage (%) of impressions that resulted in clicks on the experience placement within a campaign.<br>**Calculation**: `clicks` divided by `impressions` | A high click-through rate indicates that the content is highly relevant and motivating to the audience in the messaging and design, and is effectively targeting the audience's interests. |
| **[!UICONTROL CPM]**<br>_Cost per thousand_ | Cost for every one thousand ad impressions for the experience placement.<br>**Calculation**: total amount `spent` divided by reach, then multiplied by 1000 | A low value may indicate cost-effective visibility, especially when paired with a high click-through rate. |
| **[!UICONTROL CPA]**<br>_Cost per Action_ | Average cost spent to achieve a specific customer action, such as a purchase or subscription.<br>**Calculation**: total amount `spent` divided by the number of customer actions completed | Use to monitor spending on experiences that result in valuable customer actions. |
| **[!UICONTROL CPC]**<br>_Cost per click_ | Average cost associated with each click in an experience placement.<br>**Calculation**: total amount `spent` divided by `clicks` | Lower average costs may indicate cost-efficient ad spend, especially when compared with a rise in conversions. |
| **[!UICONTROL Spend]**       | The amount spent from the budget over a given period of time. | A high spend amount in a short period may indicate rapid usage, which could lead to early depletion of resources. Track the spend amount against key performance metrics to help monitor the overall return on investment. |
