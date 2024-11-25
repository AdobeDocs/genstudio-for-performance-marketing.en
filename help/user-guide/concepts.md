---
title: Adobe GenStudio for Performance Marketing concepts
description: Learn Adobe GenStudio for Performance Marketing concepts and terminology.
feature: Workflow, Generative AI
exl-id: 7dd00b4c-f429-499b-851d-3606c82c09dc
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

## Large language models

GenStudio for Performance Marketing leverages Adobe's generative AI platform, which offers foundational AI and machine learning (ML) services. This platform simplifies the use of large language models (LLMs), powering Adobe's GenAI capabilities to create engaging experiences.

GenStudio for Performance Marketing uses the GPT series of third-party LLMs through Azure OpenAI.<!-- Claude, and Gemini models. -->

## Generative credits

Generative credits allow the use of generative AI features powered by GenStudio for Performance Marketing. Each generative action, such as generating a set of email variants, incurs a computational cost comprised of the processing power required to generate the content, the complexity of the task, and the amount of data processed. These generative actions are calculated and debited against your allotted generative credits.

See your Adbe account management to review your generative credit allocation and usage. Usage rates may vary. Plans are subject to change.

## Generative credits rate info

Features that consume GenActions

| SN  | PRODUCT FUNCTION  | RATE | USAGE MODEL  | Notes |
| --- | ------------------------- | ----------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------- |
| 1   | Create Email              | 5 GenActions per Prompt | Mo will work on 1 email campaign per week. It will take 5 generations (aka Prompts) to get to good outputs. So Mo will use 5 Prompts per week, 20 a month. At the rate of 5 GenActions - this will be 100 GenActions / month.                            | Each generation will create 4 draft emails.                                                                           |
| 2   | Create Paid Media Ads     | 5 GenActions per Prompt | Mo will work on 3 Ads per week, or 12 Ads per month. It will take 5 generations (aka Prompts) to get to good outputs. So Mo will use 60 Prompts per month. At the rate of 5 GenActions per Prompt - this will be 300 GenActions / month.                 | Each generation will create 4 draft paid media ads. We expect Mo to create multiple size renditions per the use case. |
| 3   | Create Display Ads        | 5 GenActions per Prompt | Mo will work on 3 Display Ads per week, or 12 Display Ads per month. It will take 5 generations (aka Prompts) to get to good outputs. So Mo will use 60 Prompts per month. At the rate of 5 GenActions per Prompt - this will be 300 GenActions / month. | Each generation will create 4 draft emails. We expect Mo to create multiple size renditions per the use case.         |
| 4   | Fragment Regeneration     | 1 GenAction per Prompt  | Users can use generative capabilities to regenerate specific fragments or sections of their digital experiences. As this is not a holistic experience generation, the rate per Prompt is lower at 1 GenAction per prompt.                                |                                                                                                                       |
| 5   | On-Brand Image Generation | 1 GenAction per Prompt  | Mo will generate 4 Images per week, or 16 Images per month. It will take 5 generations (aka Prompts) to get to good outputs. So Mo will use 80 Prompts per month. At the rate of 1 GenActions per Prompt - this will be 80 GenActions / month.           | Not in GA Scope. Each generation will create 4 draft images.                                                          |

#### GenAI-powered functions that do not consume GenAction credits

| SN  | PRODUCT FUNCTION                  | USAGE                                                                                                                                                                                                                           |
|-----|-----------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 1   | Brand Validation on Generate click | Brand Validation is invoked after each generation (Prompt) on the entire generated content. For GA, only Marketing Copy is validated if a Brand is selected in the Create menu. Selecting a Brand is optional. Mo might choose to not select a Brand and there will be no validation conducted. While these operations incur COGS, for now, we will meter these actions, but not allocate GenActions. After GA, brand validation will also be performed on Images generated in GenStudio. All generated variants (for example, 4 for email) are sent separately (async) to the Brand Validation service. |
| 2   | Brand Validation on Manual Recheck | If a Brand is selected, Mo can initiate a manual Brand Validation of an edited / regenerated fragment. In the current implementation, the entire single variant (all text fragments + media) are sent to the Brand Validation service. |

## Data governance

When working with AI to generate content, it is essential to ensure the output is safe and inclusive for all users. This requires evaluation of the content for potential harmful biases, hate speech, offensive material, or profanity. Adobe thoroughly tests content generation technology from multiple perspectives, performs comprehensive ethics reviews, and implements effective mitigation plans to prevent harmful content from emerging in outputs.

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
