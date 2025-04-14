---
title: Attributes overview
description: Learn how to evaluate the performance of specific attributes in Adobe GenStudio for Performance Marketing.
level: Intermediate
feature: Reporting and Insights, Content Attributes, Content Performance
exl-id: 9d05c128-50d5-415a-ae60-7023c36c06ad
---
# Attributes overview

The [!DNL Insights] _[!UICONTROL Attributes]_ view shows a list of attributes used in ad campaigns for the selected channel account.

{{connect-insights}}

The _[!UICONTROL Attributes]_ table is organized using the [!UICONTROL Attribute] name. You can toggle between the list types using the **[!UICONTROL Images]** button and the **[!UICONTROL Video]** button. Click the settings (cog) icon above the right side of the table to toggle the viewable columns.

The filter (funnel) icon above the left side of the table opens the **[!UICONTROL Filter]** menu where you can select from multiple lists. Select **[!UICONTROL Clear all]** above the table to remove all filters.

![Attributes filter and table](/help/assets/insights-attributes-filter.png){zoomable="yes"}

{{$include /help/_includes/download-insights.md}}

## Attribute details

Attributes help to identify [ads](ads.md#ad-details) and [media](media.md#media-details) by their inherent details, such as color, composition, visual elements, and other properties.

In the attribute details view, you can see which ads use the selected attribute. Details include total attribute performance and a breakdown of the performance metrics related to each ad.

![Attribute performance metrics](/help/assets/insights-attribute-details.png){zoomable="yes"}

GenStudio for Performance Marketing detects certain features and applies the appropriate attribute to media content or ad as a tag. See [Categories](#categories) for examples of these tags. To see all the attributes associated with an ad, click the settings (cog) icon above the right side of the table to select the **[!UICONTROL Attributes]** column.

## Categories

An attribute _category_ is a classification group that organizes related attributes that share a common characteristic. These categories help streamline the discovery, identification, and understanding of specific attributes by providing greater context and facilitating their application and use.

GenStudio for Performance Marketing uses Adobe's AI and machine learning capabilities to study [images](image-features.md), [videos](video-features.md), and [text](text-features.md) and apply attributes to ads and media based on a probability of correctness.

The detected attributes list for ads and media content is not exhaustive. Content that contains a rich set of features may be limited to the three most dominant features identified by the AI. For example, the following illustration contains several detected image attributes, including multiple objects, foreground and background colors:

![image attributes](/help/assets/category/asset-attributes.png "Image of Toucan includes multiple detected attributes"){width="300" zoomable="yes"}

>[!INFO]
>
>You cannot edit tags that are detected and automatically applied.

## Attribute performance

Insights metrics can help you evaluate which attributes inspire more customer engagement.

The following table provides definitions and insights for key digital marketing metrics in the [!UICONTROL Attributes] table view. Each metric includes a brief definition as it relates to attributes, how the metric is calculated, and one or more insights to help understand its significance and impact on an ad campaign.

| Metric                 | Definition                    | Insight                          |
| ---------------------- | ----------------------------- | -------------------------------- |
| **[!UICONTROL Attribute]**   | The attribute name. | Sort the table by clicking on the column heading for any of the key metrics. |
| **[!UICONTROL Category]**    | The [category](#categories) that represents the inherent quality of an attribute. |  |
| **[!UICONTROL # of images]** | The number of images that have this attribute. | The count in the Attributes table may be different than the count in the Attribute details view. This discrepancy can occur if the channel source, such as Meta, and GenStudio use slightly different summary calculations. |
| **[!UICONTROL # of videos]** | The number of videos that have this attribute. | The count in the Attributes table may be different than the count in the Attribute details view. This discrepancy can occur if the channel source, such as Meta, and GenStudio use slightly different summary calculations. |
| **[!UICONTROL Impressions]** | A count of each time an image or videos with this attribute loads in the channel, regardless of interaction or viewing. | A high impression count can indicate broad visibility, but for true performance insight, consider it in relation with other engagement metrics. |
| **[!UICONTROL Clicks]**      | The number of times users interact with an image or video with this attribute. | A high click count indicates strong interest and engagement with the content, which may be effective and reaching the right audience. |
| **[!UICONTROL CTR]**<br>_Click-through rate_ | Percentage (%) of impressions that resulted in clicks on images or videos with this attribute.<br>**Calculation**: `clicks` divided by `impressions` | A high click-through rate indicates that the content is highly relevant and motivating to the audience in the messaging and design, and is effectively targeting the audience's interests. |
| **[!UICONTROL CPM]**<br>_Cost per thousand_ | Cost for every one-thousand ad impressions of an image or video with this attribute.<br>**Calculation**: total amount `spent` divided by reach, then multiplied by 1000 | A low value may indicate cost-effective visibility, especially when paired with a high click-through rate. |
| **[!UICONTROL CPA]**<br>_Cost per Action_ | Average cost spent to achieve a specific customer action, such as a purchase or subscription.<br>**Calculation**: total amount `spent` divided by the number of customer actions completed | Helps to identify attributes that result in valuable customer actions. |
| **[!UICONTROL CPC]**<br>_Cost per click_ | Average cost associated with each click on images or videos with this attribute.<br>**Calculation**: total amount `spent` divided by `clicks` | Lower average costs may indicate cost-efficient ad spend, especially when compared with a rise in conversions. |
| **[!UICONTROL Spend]**       | The amount spent from the budget as it relates to attributes over a given period of time. | A high spend amount in a short period may indicate rapid usage, which could lead to early depletion of resources. Track the amount spent against key performance metrics to help monitor the overall return on investment. |
