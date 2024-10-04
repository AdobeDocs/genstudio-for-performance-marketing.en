---
title: Attributes overview
description: Learn how to evaluate the performance of specific attributes in Adobe GenStudio for Performance Marketing.
feature: Insights, Assets
---
# Attributes overview

The [!DNL Insights] _[!UICONTROL Attributes]_ view shows a list of attributes used in ad campaigns for the selected channel account.

The _[!UICONTROL Attributes]_ table is organized using the [!UICONTROL Attribute] name. You can toggle between the list types using the **[!UICONTROL Images]** button and the **[!UICONTROL Video]** button. Click the settings (cog) icon above the right side of the table to toggle the viewable columns.

The filter (funnel) icon above the left side of the table opens the **[!UICONTROL Filter]** menu where you can select from the [!UICONTROL Account] and [!UICONTROL Attribute category] to filter the attributes in the table. The following example shows a list of attributes in the `Lighting Condition` category.

![Attributes filter and table](/help/assets/insights-attributes-filter.png){zoomable="yes"}

## Attribute details

Attributes help to identify assets by their inherent details, such as color, composition, visual elements, and other properties.

In the attribute details view, you can see which experiences use the selected attribute. Details include total attribute performance and a breakdown of the performance metrics related to each experience.

![Attribute performance metrics](/help/assets/insights-attribute-details.png){zoomable="yes"}

GenStudio for Performance Marketing detects certain features and applies the appropriate attribute to an asset or experience as a tag. See [Categories](#categories) to see examples of these tags. To see all the attributes associated with an experience, click the settings (cog) icon above the right side of the table to select the **[!UICONTROL Attributes]** column.

## Categories

GenStudio for Performance Marketing recognizes certain features of images, videos, and text and applies a feature tag to the asset. A _category_ is a set of features that share a specific characteristic. An example value of _image orientation_ is `landscape`.

Attributes that are detected and automatically applied cannot be edited.

<!--
Select any of the following to open a detailed list of feature categories:

+++**Image features**

| Category               | Values                              |
| ---------------------- | ----------------------------------- |
| Background Colors      | 14 colors |
| Camera Position        | - `low angle`, `high angle`, `dutch angle`<br>- `overhead view`, `eye level`,`bird's eye view` |
| Camera Proximity       | `close up`, `mid shot`, `long shot` |
| Camera Setting         | - `fast shutter speed`, `long exposure`, `double exposure`<br>- `normal mode`, `flash`, `macro`, `wide-angle`<br>- `black and white`, `surreal`<br>- `bokeh blur`, `motion blur`, `tilt-shift blur` |
| Foreground Colors      | 14 colors |
| Image Type             | `photograph`, `sketch`, `painting`, `digital cartoon`, `infographics`, `graphic design`, `collage`, `screenshot` |
| Lighting Condition     | golden hour, blue hour, midday, overcast, night, high-key, low-key, daylight, incandescent, fluorescent, colorful, studio |
| Objects                | The items, entities, and elements that are visible, such as `lighthouse`, `orchid`, or `tunnel`. |
| Orientation            | Examples: `landscape`, `portrait`, `square` |
| Overall Tone           | `warm`, `cool`, `neutral` |
| People Categories      | Examples: `person`, `social group`, `people`, `kid` |
| Photography Styles     | `aerial photography`, `aerial photography`, `architectural photography`, `astrophotography`, `black and white photography`, `business photography`, `cityscape photography`, `commercial photography`, `composite photography`, `creative photography`, `editorial photography`, `event photography`, `family photography`, `fashion photography`, `fine art photography`, `food photography`, `holiday photography`, `indoor photography`, `landscape photography`, `lifestyle photography`, `macro photography`, `minimalist photography`, `night photography`, `outdoor photography`, `pet photography`, `portrait photography`, `product photography`, `real estate photography`, `seascape photography`, `sports photography`, `still-life photography`, `street photography`, `travel photography`, `underwater photography`, `wildlife photography` |
| Scenes                 | Examples: `city`, `island`, `living room` |
| Tags                   | Examples: `gaming`, `law`, `yoga` |
| Visual Attention Spread| The level of viewer attention spread across an image: `high`, `low` |
| Visual Content Density | The amount of information or detail in an image: `high`, `low` |

+++

+++**Video features**

| Category               | Values                              |
| ---------------------- | ----------------------------------- |
| Audio Genre  | |
| Audio Genre Category  | |
| Audio Mood  | |
| Audio Types| |
| Objects  | |
| Orientation  | |
| People Categories  | |
| Scenes  | |
| Styles  | |
| Tags   | |
| Video Category  | |
| Video Type  | |

+++

+++**Text features**

| Category               | Values                              |
| ---------------------- | ----------------------------------- |
| Emojis Count  | |
| HashTags Count  | |
| Keywords  | |
| Marketing Emotions  | |
| Narratives  |  |
| Persuasion Strategies  |  |
| Readability  | |
| Sentences Count  | |
| Stop Words Ratio  | |
| Text Quotes Count  | |
| Tones  | |
| Words Count  | |
| Words Count Per Sentence  | |

+++

-->

## Attribute metrics

Insights metrics can help you evaluate which attributes inspire more customer engagement.

### Metrics detail

The following table provides definitions and insights for key digital marketing metrics in the [!UICONTROL Attributes] view. Each metric includes a brief definition as it relates to an asset, how the metric is calculated, and one or more insights to help understand its significance and impact on an ad campaign.

| Metric                 | Definition                    | Insight                          |
| ---------------------- | ----------------------------- | -------------------------------- |
| **[!UICONTROL Attribute]**   | The attribute name. | Sort the table by clicking on the column heading for any of the key metrics. |
| **[!UICONTROL Category]**    | The [category](#categories) that represents the inherent quality of an attribute. |  |
| **[!UICONTROL # of images]** | A count of images with this attribute. |  |
| **[!UICONTROL # of videos]** | A count of videos with this attribute. |  |
| **[!UICONTROL Impressions]** | A count of each time an image or videos with this attribute loads in the channel, regardless of interaction or viewing. | A high impression count can indicate broad visibility, but for true performance insight, consider with other engagement metrics. |
| **[!UICONTROL Clicks]**      | Number of times users interact with an image or video with this attribute. | A high click count indicates strong interest and engagement with the content, which may be effective and reaching the right audience. |
| **[!UICONTROL CTR]**<br>_Click-through rate_ | Percentage (%) of impressions that resulted in clicks on images or videos with this attribute.<br>**Calculation**: `clicks` divided by `impressions` | A high click-through rate indicates that the content is highly relevant and motivating to the audience in the messaging and design, and is effectively targeting the audience's interests. |
| **[!UICONTROL CPM]**<br>_Cost per thousand_ | Cost ($) for every one-thousand ad impressions of an image or video with this attribute.<br>**Calculation**: total amount `spent` divided by reach, then multiplied by 1000  | A low value may indicate cost-effective visibility, especially when paired with a high click-through rate. |
| **[!UICONTROL CPC]**<br>_Cost per click_ | Average cost ($) associated with each click on images or videos with this attribute.<br>**Calculation**: total amount `spent` divided by `clicks` | Lower average costs may indicate cost-efficient ad spend, especially when compared with a rise in conversions. |
| **[!UICONTROL Spend]**       | The amount ($) spent from the budget as it relates to attributes over a given period of time. | A high spend amount in a short period may indicate rapid usage, which could lead to early depletion of resources. Track the spend amount against key performance metrics to help monitor the overall return on investment. |
