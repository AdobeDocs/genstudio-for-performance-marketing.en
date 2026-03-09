---
title: Meta Ad Template Guidelines
description: Follow best practices when using Meta ad templates with Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Developer, User
feature: Media Templates
exl-id: e69039b0-272d-4f39-b0e4-916be710fd5f
TQID: https://experienceleague.adobe.com/-WHH1xjWFaizXTKjuF-K9UtaR12V3QpMezSqRfwbMIU
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
    internal-label: GenStudio for Performance Marketing
feature_v2:
  - id: bffd9bc2-7f41-4bf6-9f08-f14cbd37afd7
    internal-label: Campaigns
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
    internal-label: Create
  - id: f71bd2fc-e9ca-4cb6-8088-82e250211e32
    internal-label: Guidelines
subfeature_v2:
  - id: e3878dde-4b87-4290-9e81-ed7ee6eb83fe
    internal-label: Experiences
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
    internal-label: Developer
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
    internal-label: Intermediate
---
# Meta ad template guidelines

Meta ad templates help you to create visually consistent and effective ads across Meta platforms. By following recommended design practices and using supported fields, you can ensure that your templates are optimized for GenStudio for Performance Marketing. This guide explains how to structure, customize, and prepare Meta ad templates for seamless integration and high-impact results.

Follow these design best practices when customizing Meta ad templates to work with GenStudio for Performance Marketing:

- Use 360 pixel width for column layouts
- Use a minimum resolution of 1080 x 1080 pixels for images
- Exactly one image field is required
- Do **not** use relative font size
- Do **not** define viewport
- Do **not** use JavaScript
- Do **not** override an HTML element in the CSS
- Use the `<img>` tag instead of `background-image`
- Use masking to improve text readability over background images
- Only one section can be used, generating a single set of template elements

## Recognized field names

When customizing your Meta ads template, apply content placeholders for these required fields:

- `image` (required, selected from Content JPEG, PNG, or GIF)
- `on_image_text` (text that appears over the image)

GenStudio for Performance Marketing automatically generates the following fields. You do not have to apply content placeholders for:

- `headline`
- `body`
- `cta`

See [Content placeholders](/help/user-guide/templates/customize-template.md#content-placeholders) to understand more about using field names in templates.

## Supported aspect ratios

| Aspect Ratio     | Dimensions (pixels)        | Notes                                                                 |
|------------------|----------------------------|-----------------------------------------------------------------------|
| Square 1:1       | 1080 x 1080                | Standard for most Meta placements; recommended for broad compatibility.|
| Portrait 4:5     | 1080 x 1350                | Optimized for mobile feeds; provides more vertical space.             |
| Story 9:16       | 1080 x 1920                | Ideal for Stories and Reels; fills the entire mobile screen.          |
| Landscape 1.91:1 | 1080 x 566                 | Best for link ads and News Feed placements; wide format.              |
| Custom           | Minimum 50 x 50 (width)    | Use only if required; may result in cropping or scaling.              |

If the ad is not designed in one of these aspect ratios, GenStudio for Performance Marketing automatically crops the image into the appropriate size.

## Template example

+++Example: Meta ad template

<!-- Does this need to be a precise size? -->

The following is a basic example of a Meta ad template. The head contains inline CSS for styling. The body uses [content placeholders](#content-placeholders), such as `image` and `on_image_text`, to indicate where GenStudio for Performance Marketing can generate content.

```html {line-numbers="true" highlight="33"}
<!DOCTYPE html>
<html>
    <head>
        <meta charset="UTF-8" />
        <meta name="viewport" content="width=device-width, initial-scale=1.0" />
        <title>Adobe</title>
        <style>
            .ad-container {
            font-family: Helvetica, sans-serif;
            position: relative;
            text-align: center;
            height: 100%;
            }
            .ad-image {
            width: 100%;
            height: 100%;
            object-fit: cover;
            }
            .ad-text {
            position: absolute;
            top: 0;
            left: 0;
            margin: 1em;
            background-color: rgba(0, 0, 0, 0.5);
            color: white;
            padding: 1em;
            font-size: 75px;
            }
        </style>
    </head>
    <body>
        <div class="ad-container">
            <img src="{{image}}" alt="Ad Image" class="ad-image" />
            <div class="ad-text">{{on_image_text}}</div>
        </div>
    </body>
</html>
```

+++
