---
title: Create Accessible Templates
description: Build templates in Adobe GenStudio for Performance Marketing that are capable of reaching more of your audience and providing an optimal experience.
feature: Media Templates
exl-id: eaaa5d9f-ad45-4fd0-826d-c250deb6d238
TQID: https://experienceleague.adobe.com/b56YHJsOAunGenV-F3u7Y2mo56f6CnnX4qPXyzczPJY
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
    internal-label: GenStudio for Performance Marketing
feature_v2:
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
    internal-label: Create
  - id: f71bd2fc-e9ca-4cb6-8088-82e250211e32
    internal-label: Guidelines
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: cc72dcf1-72e1-48cc-b434-e7c27d62d67c
    internal-label: Accessibility
---
# Create accessible templates

Adobe is committed to providing an optimal experience for all audiences. See [Accessibility Initiatives at Adobe](https://www.adobe.com/trust/accessibility/initiatives.html) for further reading.

In GenStudio for Performance Marketing, you can upload assets and templates that enable content creation for a variety of experiences. Adhering to accessibility standards helps your content reach your maximum intended audience.

Use the following recommendations to prepare your templates using optimal accessibility standards.

## Alternative text

Provide text alternatives for non-textual content, such as images.

```html
<img alt="Collage of ideas, books, man holding giant pencil, computer" src="card-create-assets.png">
```

![Collage of ideas, books, man holding giant pencil, computer](/help/assets/card-create-assets.png){width="400"}

When customizing your template, use content placeholders for the `alt` and `aria-label` attributes:

- [Alternative text](/help/user-guide/templates/customize-template.md#alternative-text)
- [Accessibility label](/help/user-guide/templates/customize-template.md#accessibility-label)

## Fonts

Use fonts that are easy to read. For example, Sans Serif fonts have a clean, block-like appearance, which contributes to a higher readability.

Provide an appropriate contrast between text and background. Avoid using font colors that produce dark text on a dark background and light text on a light background. Consider the contrast guidelines for an optimal ratio:

- Text and images of text: contrast ratio of at least 4.5:1
- Large text and images of large-scale text: contrast ratio of at least 3:1

## Link Purpose (Link Only)

Create clear link text that describes the purpose and location of the link.

For example, using link text such as "Click here" or "Read more" does not clearly describe the purpose of the link:

```html
<a href="product-site.html">Click here</a>
```

As a best practice, you should use text that clearly describes where the link goes. A better example might use the title of the link source and the purpose:

```html
<a href="product-site.html">Explore Product Site</a>
```

## Language

Many products and services use language in a creative or unique way. Avoid jargon, long sentences, and complex phrases. Use clear, concise, easy-to-read language compatible with your target audience.

- Use clear descriptions, inline definitions, or relatable examples when possible. It can be difficult to translate a unique vernacular.

- Spell out or link to a definition for the first instances of an acronym or abbreviation. It can be difficult to translate abbreviations.

- Use visual elements to supplement text or complex ideas when possible.
