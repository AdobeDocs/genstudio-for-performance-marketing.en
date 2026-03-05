---
title: LinkedIn Template Guidelines
description: Follow best practices when using LinkedIn templates with Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Developer, User
feature: Media Templates
exl-id: 85432185-8311-411b-b57b-f482c3d45854
---
# LinkedIn template guidelines

LinkedIn templates provide a structured way to create and customize ad creatives for LinkedIn campaigns. These guidelines ensure that your ads meet LinkedIn's specifications while streamlining the creative process in GenStudio for Performance Marketing. This guide helps you prepare for consistent branding and effective performance across LinkedIn's desktop and mobile platforms.

Follow these design best practices when customizing LinkedIn ad templates to work with GenStudio for Performance Marketing:

- Exactly one image field is required
- Maximum image size of 5 MB
- Maximum headline 70 characters
- Maximum introductory text 150 characters
- Only one section can be used, generating a single set of template elements

## Recognized field names

When customizing your LinkedIn template, apply content placeholders for these required fields:

- `image` (required, selected from Content JPEG, PNG, or GIF)
- `on_image_text` (text that appears over the image)

GenStudio for Performance Marketing automatically generates the following fields. You do not have to apply content placeholders for:

- `headline`
- `introductory_text`
- `cta` (Call to Action)

See [Content placeholders](/help/user-guide/templates/customize-template.md#content-placeholders) to understand more about using field names in templates.

## Supported aspect ratios

All LinkedIn template widths are hardcoded at 1200 pixels.

| Aspect Ratio      | Platform        | Dimensions (px) | Notes                                                                  |
|-------------------|-----------------|------------|-------------------------------------------------------------------------------------|
| Square 1:1        | Desktop, Mobile | 1200 x 1200     | Most versatile. Ideal for consistent appearance across devices and placements.       |
| Horizontal 1.91:1 | Desktop         | 1200 x 628     | Standard landscape format. Commonly used for sponsored content and news feed ads.    |
| Vertical 1:1.91   | Mobile          | 1200 x 2292    | Tall vertical format. Optimized for mobile viewing, offering more screen presence.   |
| Vertical 2:3      | Mobile          | 1200 x 1800    | Slightly less tall than 1:1.91. Good for mobile-first campaigns.                     |
| Vertical 4:5      | Mobile          | 1200 x 1500   | Recommended for mobile. Balances visibility and content, which often yields higher impact. |

<!-- Potentially add an example

## Template example

+++Example: LinkedIn template

+++

-->
