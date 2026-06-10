---
title: Email Experiences
description: Learn about email experiences in Adobe GenStudio for Performance Marketing, including Canvas behavior and content fragment swap from approved libraries.
feature: Create Canvas, Media Templates
role: User
level: Beginner
exl-id: e2bddd02-914e-43a8-92b6-fdcbced94a6a
TQID: https://experienceleague.adobe.com/-lwSfvc0TnVd8byNT-5OfoEsXz7yaeIifcHOJtp-n4c
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
    internal-label: GenStudio for Performance Marketing
feature_v2:
  - id: c7c3a4ab-6b96-4f2f-8931-4d2b360c3d12
    internal-label: Generative AI
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
    internal-label: Create
  - id: f71bd2fc-e9ca-4cb6-8088-82e250211e32
    internal-label: Guidelines
subfeature_v2:
  - id: a8b28c00-da6e-4d27-8667-80f790ad8972
    internal-label: Email experiences
  - id: be495d08-ecd1-455f-951e-c22de504e667
    internal-label: Content generation
  - id: dee4e9a9-78d1-4953-8179-f8da6117027d
    internal-label: Create canvas
  - id: ee4b6e5f-5b7a-421b-9859-0f964841a866
    internal-label: Meta experiences
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
    internal-label: Beginner
---
# Email experiences

With Adobe GenStudio for Performance Marketing, you can use generative AI to streamline the [creation of high-impact email experiences](/help/user-guide/create/create-email-experience.md).

[!DNL Create] enables modern marketers to use [guidelines](/help/user-guide/guidelines/overview.md), image assets, and a [well-crafted prompt](/help/user-guide/effective-prompts.md) to quickly [create brand-aligned email experiences](/help/user-guide/create/create-email-experience.md).

When generating email experiences four variations are created and shown in the Canvas.

Editable sections of an email experience include:

* Pre-header
* Headline
* Sub-headline
* Body
* Call to action (CTA)
* Image

See [Template elements](/help/user-guide/templates/use-templates.md#template-elements).

<!-- 
## Email capabilities

Content creators and marketers can produce brand-consistent email experiences in GenStudio for Performance Marketing. 
-->

## Multi-section emails

Email experiences can feature multiple sections, allowing full customization to align with your brand and goals. [Select [!DNL Products] and visual assets for each section](/help/user-guide/create/create-email-experience.md#add-parameters) and use [structured prompts](/help/user-guide/effective-prompts.md#structured-prompts) to craft unique content. Each section supports one visual asset.

See [customizing templates with sections](/help/user-guide/templates/customize-template.md#sections-or-groups) to learn how to create a multi-section template.

## Progressive loading

When the content generation process starts, each section of generated content in email variants progressively loads in the Canvas. Experiences, assets, and fields and sections within experiences, appear individually in the Canvas as they are generated.

When you click **[!UICONTROL Generate]**, a loading indicator appears at the bottom of the Canvas updating you on the progress of generation.

Each field and section of email experiences are progressively loaded in this sequence:

1. Variant names
1. Subject lines for all variations
1. Pre-headers
1. Headlines, email body (for single section emails), and calls-to-action
1. Email body for subsequent sections (for multi-section emails)
1. Brand validation

   Brand validation and content check process occurs and the [_Content check_ summary](/help/user-guide/guidelines/brand-validation.md#content-check-summary) populates for each variant.

## Character counts

After you generate a set of email variants, you can see the character count displayed for each section. Hover over or click into a generated section, such as the subject line or the body, and see the section name and character count for that section.

![Character count](/help/assets/character-count.png){width="500" zoomable="yes"}

## Content fragment swap {#content-fragment-swap}

>[!NOTE]
>
>Content fragment swap is available for **email** experiences on the Canvas today. **Horizon** channel support is coming soon.

Enterprise email content often needs both newly generated copy and approved modular blocks (such as disclaimers, safety language, offers, and regulated claims) alongside content you shape for templates. Teams that store modular content in [!DNL Adobe Experience Manager] can find and swap that content to use in email experiences without leaving [!DNL GenStudio for Performance Marketing]. This can be useful for:

* **Compliance-aware content:** AI can fill creative slots while compliance-approved fragments replace injectable slots; locked legal areas stay unchanged through export.
* **Reusable approved content components:** Approved headlines, regional disclaimers, or product descriptions can remain the system of record in [!DNL Adobe Experience Manager] while authors pull them into variants without copy-paste workarounds.

Creators assemble experiences on the Canvas; brand and compliance teams keep approval workflows in [!DNL Adobe Experience Manager]; IT and integrations teams connect repositories and permissions your organization requires.

![Content fragment swap](./cf-swap.png){width="500" zoomable="yes"}

When your organization enables content fragment swap, you can expect:

* Content fragment fields can be populated from a connected content library instead of only manual typing or AI generation alone.
* Browse, search, and filter fragments using metadata such as campaign, persona, channel, language, and brand.
* A repository picker is available when multiple repositories are configured.
* Preview of a fragment before it replaces field text.
* Propagation of a fragment selection across all variants in one action.

![Content fragments UI pane](./cf-pane.png){width="500" zoomable="yes"}

Your organization chooses which content fragment sources and repositories are available. See [Find content fragment extension](/help/extensibility/deploy-app.md#find-content-fragment-extension) for how administrators configure sources and how authors swap copy from the Canvas with **[!UICONTROL Swap]**.

You can also translate an approved email experience into multiple languages on the HTML canvas. See [Translate and localize experiences](/help/user-guide/create/translate-experiences.md).
