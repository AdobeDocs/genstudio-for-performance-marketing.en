---
title: Adobe GenStudio for Performance Marketing Concepts
description: Learn Adobe GenStudio for Performance Marketing concepts and terminology.
feature: Generative AI
role: User
exl-id: 7dd00b4c-f429-499b-851d-3606c82c09dc
TQID: https://experienceleague.adobe.com/i3VF7S-ndAMDoF1akF3l20tStW-IPS--MSysxD-MArc
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
    internal-label: GenStudio for Performance Marketing
feature_v2:
  - id: bffd9bc2-7f41-4bf6-9f08-f14cbd37afd7
    internal-label: Campaigns
  - id: c5a86ad9-9158-4ab1-a7ea-9e29985087b8
    internal-label: Content lifecycle
  - id: c7c3a4ab-6b96-4f2f-8931-4d2b360c3d12
    internal-label: Generative AI
  - id: c95c94c1-727b-457a-9184-a4dda4c95ab2
    internal-label: Insights
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
    internal-label: Create
  - id: f71bd2fc-e9ca-4cb6-8088-82e250211e32
    internal-label: Guidelines
  - id: f912fa8d-7beb-4468-9ea7-1c0f198b59ef
    internal-label: Data governance
subfeature_v2:
  - id: a98e0185-3180-4e8c-8f31-f72af4cc21a2
    internal-label: Assets
  - id: be495d08-ecd1-455f-951e-c22de504e667
    internal-label: Content generation
  - id: dd48f9df-f2e2-49fe-a918-332a8e240ffe
    internal-label: Channels
  - id: e3878dde-4b87-4290-9e81-ed7ee6eb83fe
    internal-label: Experiences
  - id: ec92a2bc-afe3-4ff0-a985-0c8ef22b4da0
    internal-label: Content management
  - id: f54ee13b-9545-4d68-9842-a12026e60aaf
    internal-label: Variant generation
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: c7d04a2c-412a-4c9d-9d7a-4456eaa5adeb
    internal-label: Governance
  - id: cdd65e7e-8839-44a2-bc21-0e03623b5dd1
    internal-label: Optimization
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
    internal-label: Insights
  - id: eb30f47f-d87a-400f-8f78-63ce7979ff56
    internal-label: Machine learning
---
# Concepts

GenStudio for Performance Marketing is a standalone enterprise product that embodies Adobe's content supply chain to streamline marketing campaigns. It is challenging to build personalized, brand-approved content at scale, monitor effectiveness, and adapt quickly to the ever-changing market. GenStudio for Performance Marketing brings Creative Cloud and Experience Cloud together in one application that leverages generative AI as a performance multiplier for enterprise marketing teams.

With GenStudio for Performance Marketing you can:

* Create on-brand content using natural language prompts for your top-priority digital channels, such as paid media, email, and display ads

* Collaborate with stakeholders to review and approve generated content
* Save generated and approved content to access for future marketing campaigns
* Assess content effectiveness by analyzing asset performance and identifying key attributes of top-performing content

## Generative AI technology

GenStudio for Performance Marketing harnesses the power of generative AI to accelerate the content creation process and ensure high-quality content generation. The iterative lifecycle of your creative assets results in increasingly accurate and brand-aligned content that resonates with your target audience.

Begin by ingesting your organization's branding, customer personas, and product descriptions through the powerful brand guidelines feature. See the [Guidelines overview](../user-guide/guidelines/overview.md) to learn how to prepare and upload these guidelines.

{{in-academy}}

### Large language models

GenStudio for Performance Marketing leverages Adobe's generative AI platform, which offers foundational AI and machine learning (ML) services. This platform simplifies the use of large language models (LLMs), powering Adobe's GenAI capabilities to create engaging experiences.

GenStudio for Performance Marketing uses the GPT series of third-party LLMs through Azure OpenAI.<!-- Claude, and Gemini models. -->

## [!DNL Generative Actions]

_[!DNL Generative Actions]_, as defined in the [Adobe GenStudio for Performance Marketing product description](https://helpx.adobe.com/legal/product-descriptions/adobe-genstudio-for-performance-marketing---product-description.html), are the units quantifying the use of generative AI features within GenStudio for Performance Marketing.

<!-- Add example about usage mode?
Where users check how many generative actions they have left
How they re-up their genactions
If genactions roll over month to month or not -->

### Rates

You receive a default allotment of [!DNL Generative Actions] as outlined in the [GenStudio for Performance Marketing product description](https://helpx.adobe.com/legal/product-descriptions/adobe-genstudio-for-performance-marketing---product-description.html).

>[!NOTE]
>
>Usage rates may vary. Plans are subject to change. See the [Adobe GenStudio for Performance Marketing product description](https://helpx.adobe.com/legal/product-descriptions/adobe-genstudio-for-performance-marketing---product-description.html) for updated rate information.

The following functions consume [!DNL Generative Actions] at the specified rate.

| Function                 | Generative actions rate |
| -----------------------  | ------------------ |
| Create email             | 5 per generation  |
| Create paid media ads    | 5 per generation  |
| Create display ads       | 5 per generation  |
| Regenerate sections      | 1 per generation  |

<!-- | Generate on-brand images | 1 per prompt  |
| Translation              | 1 per prompt  |
| Video: ADLS              | 1 per prompt  |
| Video: TTS + Avatar      | 1 per prompt  | -->

[!DNL Generative Actions] _are not_ consumed when:

* Using [brand validation](/help/user-guide/guidelines/brand-validation.md) during variant generation
* Extracting information from [uploaded guidelines](/help/user-guide/guidelines/add-guidelines.md)
* Manually [re-checking variants](/help/user-guide/guidelines/brand-validation.md#improve-brand-alignment)
* Digital assets are automatically tagged with attributes ([[!DNL Insights]](/help/user-guide/insights/overview.md))

>[!TIP]
>
>If you exceed your entitlement of [!DNL Generative Actions], you may purchase more directly from your account representative.

## Data governance

When working with AI to generate content, it is essential to ensure that the output is safe and inclusive for all users. This requires evaluation of the content for potential harmful biases, hate speech, offensive material, or profanity. Adobe thoroughly tests content generation technology from multiple perspectives, performs comprehensive ethics reviews, and implements effective mitigation plans to prevent harmful content from emerging in outputs.

This approach reinforces social responsibility, minimizes reputational risk, and ensures adherence to [Adobe's Trust & Safety and Ethics policies](https://www.adobe.com/content/dam/cc/en/ai-ethics/pdfs/Adobe-AI-Ethics-Principles.pdf).

GenStudio for Performance Marketing incorporates mitigation plans to prevent the use of identified harmful or biased content per Adobe data governance standards and policies. When such content is detected, you are made aware that asset generation is blocked with a "Can't generate" message.

When this message appears, you can edit the prompt and try again _or_ flag the prompt content for review by GenStudio for Performance Marketing. The prompt data for content that is flagged for review is collected for internal review purposes.

## Content lifecycle

The demand is high for quality experiences in multiple channels at a faster pace. GenStudio for Performance Marketing simplifies the content supply chain into a well-organized workflow for marketers. GenStudio for Performance Marketing leverages Adobe technology at each stage of the lifecycle.

<table style="table-layout:auto">
<tr style="border: 0;">
    <td>
       <p><strong>Workflow & Planning</strong></p>
    </td>
    <td>
        <p>Brainstorm ideas, define guidelines, and build a strategy around content to engage your audience.</p>
    </td>
</tr>
<tr style="border: 0;">
    <td>
        <p><strong>Creation & Production</strong></p>
    </td>
    <td>
        <p>Produce the content based on the plan. Collaborate in real time, receive feedback, make edits, and approve content.</p>
    </td>
</tr>
<tr style="border: 0;">
    <td>
        <p><strong>Content Management</strong></p>
    </td>
    <td>
        <p>Store, share, and find creative assets in the centralized repository. Reuse and revitalize content based on performance.</p>
    </td>
</tr>
<tr style="border: 0;">
    <td>
        <p><strong>Delivery & Activation</strong></p>
    </td>
    <td>
        <p>Activate content and publish across multiple marketing channels.</P>
    </td>
</tr>
<tr style="border: 0;">
    <td>
        <p><strong>Reporting & Insights</strong></p>
    </td>
    <td>
        <p>Collect data and derive insights for asset performance optimization.</p>
    </td>
</tr>
</table>
