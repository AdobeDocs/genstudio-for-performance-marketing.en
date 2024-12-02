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

## Generative actions

Generative actions allow the use of generative AI features powered by GenStudio for Performance Marketing. Each generative action, such as generating a set of email variants, incurs a computational cost comprised of the processing power required to generate the content, the complexity of the task, and the amount of data processed. These are calculated and debited against your allotted generative actions.

See your [Adobe account](https://account.adobe.com/) to review your generative action allocation and usage. Usage rates may vary. Plans are subject to change.

<!-- Add example about usage mode?
Where users check how many generative actions they have left
How many genactions are available by default
How they re-up their genactions
If genactions roll over month to month or not -->

### Rates

The following functions consume generative actions.

| Function                 | Generative actions rate |
| -----------------------  | ------------------ |
| Create email             | 5 per prompt  |
| Create paid media ads    | 5 per prompt  |
| Create display ads       | 5 per prompt  |
| Regenerate sections      | 1 per prompt  |
<!-- | Generate on-brand images | 1 per prompt  |
| Translation              | 1 per prompt  |
| Video: ADLS              | 1 per prompt  |
| Video: TTS + Avatar      | 1 per prompt  | -->

Generative credits _are not_ consumed when using brand validation during variant generation or while manually re-checking variants.

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
