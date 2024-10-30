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

GenStudio for Performance Marketing recognizes certain features of images, videos, and text and applies a feature tag to the asset. A _category_ is a set of features that share a specific characteristic. For example, the _image orientation_ category has a `landscape`, `portrait`, or `square` value.

Attributes that are detected and automatically applied cannot be edited.

Select any of the following to open a detailed list of feature categories:

+++**Image features**

The following tables list the image feature categories recognized by the GenStudio for Performance Marketing generative AI.

| Category | Description | Values |
| -------- | ----------- | ------ |
| Camera Position        | The location and angle of the camera relative to the subject. | - `low angle`, `high angle`, `dutch angle`<br>- `overhead view`, `eye level`,`bird's eye view` |
| Camera Proximity       | The distance between the camera and the subject of an image. | `close up`, `mid shot`, `long shot` |
| Camera Setting         | The configuration of the camera's controls to produce the image. | - `fast shutter speed`, `long exposure`, `double exposure`<br>- `normal mode`, `flash`, `macro`, `wide-angle`<br>- `black and white`, `surreal`<br>- `bokeh blur`, `motion blur`, `tilt-shift blur` |
| Colors and tone   | The color of elements in the background or foreground of the image.<br>The overall warmth or coolness of the image colors. | Colors: Returns the color profile from a set of 40 pre-determined colors.<br>Tones: `warm`, `cool`, `neutral` |
| Image Type             | The visual treatment of an image. | `photograph`, `sketch`, `painting`, `digital cartoon`, `infographics`, `graphic design`, `collage`, `screenshot` |
| Lighting Condition     | The type of light in an image. | `golden hour`, `blue hour`, `midday`, `overcast`, `night`, `high-key`, `low-key`, `daylight`, `incandescent`, `fluorescent`, `colorful`, `studio` |
| Objects           | The items, entities, and elements that are visible. | Examples: `lighthouse`, `orchid`, `tunnel` |
| Orientation       | Image alignment, based on its width-to-height ratio. | Examples: `landscape`, `portrait`, `square` |
| People Categories | The kinds of people in an image. | Examples: `person`, `social group`, `people`, `kid` |
| Photography Styles     | The subject and technique used to capture an image. | `aerial`, `architectural`, `astrophotography`, `black and white`, `business`, `cityscape`, `commercial`, `composite`, `creative`, `editorial`, `event`, `family`, `fashion`, `fine art`, `food`, `holiday`, `indoor`, `landscape`, `lifestyle`, `macro`, `minimalist`, `night`, `outdoor`, `pet`, `portrait`, `product`, `real estate`, `seascape`, `sports`, `still-life`, `street`, `travel`, `underwater`, `wildlife` |
| Scenes            | The setting or environment depicted in an image. | Examples: `city`, `island`, `living room` |
| Tags              | Objects, elements, and other image characteristics. | Examples: `gaming`, `law`, `yoga` |
| Visual Attention Spread | The level of viewer attention spread across an image. | `high`, `medium`, `low` |
| Visual Content Density | The amount of information or detail in an image. | `high`, `medium`, `low` |

+++

+++**Video features**

The following table lists the video feature categories recognized by the GenStudio for Performance Marketing generative AI.

| Category | Description | Values |
| -------- | ----------- | ------ |
| Audio Genre  | | |
| Audio Genre Category  | | |
| Audio Mood  | | |
| Audio Types| | |
| Objects  | | |
| Orientation  | | |
| People Categories  | | |
| Scenes  | | |
| Styles  | | |
| Tags   | | |
| Video Category  | | |
| Video Type  | | |

+++

+++**Text features**

The following table lists the text feature categories recognized by the GenStudio for Performance Marketing generative AI.

| Category | Description | Values |
| -------- | ----------- | ------ |
| Emojis Count  | | |
| HashTags Count  | | |
| Keywords  | | |
| Marketing Emotions  | | |
| Narratives  |  | |
| Persuasion Strategies  |  | |
| Readability  | | |
| Sentences Count  | | |
| Stop Words Ratio  | | |
| Text Quotes Count  | | |
| Tones  | | |
| Words Count  | | |
| Words Count Per Sentence  | | |

+++

## Attribute metrics

Insights metrics can help you evaluate which attributes inspire more customer engagement.

### Metrics detail

The following table provides definitions and insights for key digital marketing metrics in the [!UICONTROL Attributes] table view. Each metric includes a brief definition as it relates to an asset, how the metric is calculated, and one or more insights to help understand its significance and impact on an ad campaign.

| Metric                 | Definition                    | Insight                          |
| ---------------------- | ----------------------------- | -------------------------------- |
| **[!UICONTROL Attribute]**   | The attribute name. | Sort the table by clicking on the column heading for any of the key metrics. |
| **[!UICONTROL Category]**    | The [category](#categories) that represents the inherent quality of an attribute. |  |
| **[!UICONTROL # of images]** | A count of images with this attribute. |  |
| **[!UICONTROL # of videos]** | A count of videos with this attribute. |  |
| **[!UICONTROL Impressions]** | A count of each time an image or videos with this attribute loads in the channel, regardless of interaction or viewing. | A high impression count can indicate broad visibility, but for true performance insight, consider with other engagement metrics. |
| **[!UICONTROL Clicks]**      | Number of times users interact with an image or video with this attribute. | A high click count indicates strong interest and engagement with the content, which may be effective and reaching the right audience. |
| **[!UICONTROL CTR]**<br>_Click-through rate_ | Percentage (%) of impressions that resulted in clicks on images or videos with this attribute.<br>**Calculation**: `clicks` divided by `impressions` | A high click-through rate indicates that the content is highly relevant and motivating to the audience in the messaging and design, and is effectively targeting the audience's interests. |
| **[!UICONTROL CPM]**<br>_Cost per thousand_ | Cost ($) for every one-thousand ad impressions of an image or video with this attribute.<br>**Calculation**: total amount `spent` divided by reach, then multiplied by 1000 | A low value may indicate cost-effective visibility, especially when paired with a high click-through rate. |
| **[!UICONTROL CPA]**<br>_Cost per Action_ | Average cost ($) spent to achieve a specific customer action, such as a purchase or subscription.<br>**Calculation**: total amount `spent` divided by the number of customer actions completed | Helps to identify attributes that result in valuable customer actions. |
| **[!UICONTROL CPC]**<br>_Cost per click_ | Average cost ($) associated with each click on images or videos with this attribute.<br>**Calculation**: total amount `spent` divided by `clicks` | Lower average costs may indicate cost-efficient ad spend, especially when compared with a rise in conversions. |
| **[!UICONTROL Spend]**       | The amount ($) spent from the budget as it relates to attributes over a given period of time. | A high spend amount in a short period may indicate rapid usage, which could lead to early depletion of resources. Track the spend amount against key performance metrics to help monitor the overall return on investment. |
