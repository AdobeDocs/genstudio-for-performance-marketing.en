---
title: Generate and Refine Content with Stateful Generation
description: Learn how to generate on-brand content and refine it turn by turn in a conversation with voiceprinting and visual cues in [!DNL GenStudio for Performance Marketing].
feature: Create Prompt, Generative AI, Content Generation
role: User
level: Beginner
---
# Generate and refine content with Stateful Generation

[!DNL GenStudio for Performance Marketing] uses Stateful Generation to help you create on-brand content and then refine it turn by turn in a conversation, instead of starting over with a new prompt each time. As you refine, the generation remembers your earlier instructions and the variants you keep, then applies only the change you ask for.

Stateful Generation adds three kinds of context to your generations: voiceprinting keeps copy in your brand voice, visual cues ground copy in an image or video, and a web page URL adds reference context from a page that you choose.

## Generate and refine content

1. In [!DNL GenStudio for Performance Marketing], start a generation for your channel and format. See the [[!DNL Create] overview](/help/user-guide/create/overview.md) to begin a generation for each channel.
1. _Optional_: To ground the copy in your own creative, select **[!UICONTROL Select from Content]**, then choose an image or video to use as a [visual cue](#ground-content-in-an-image-or-video).
1. Select **[!UICONTROL Generate]**. [!DNL GenStudio for Performance Marketing] creates a set of variants and applies your [brand voice](#keep-copy-in-your-brand-voice) automatically on supported channels.
1. Refine the results in the prompt drawer. Type the change that you want, such as `shorten the headline`, `make variant 2 punchier`, or `change the headline`. The generation applies only that change and keeps your earlier instructions.
1. To keep a variant while you continue to refine, type an instruction in the prompt drawer, such as `keep variant 2`.
1. When the content is ready, export it or send it for review.

## Ground content in an image or video

Visual cues let the generation read an image or video that you attach, then write copy that reflects that creative. The **[!UICONTROL Creative options]** toggle controls visual cues, and it is on by default.

To use a visual cue, select **[!UICONTROL Select from Content]** and choose an image or video before you generate. To generate without a visual cue, turn off **[!UICONTROL Creative options]**.

>[!NOTE]
>Visual cues are not available for multi-frame display ads or carousel ads.

## Keep copy in your brand voice

Voiceprinting applies your brand's learned voice to generated copy, so that it sounds on-brand without extra prompting. It is on by default for channels that have [Insights](/help/user-guide/insights/overview.md), such as LinkedIn and Meta.

## Use a web page as context

You can point the generation at a web page and use its content as context. In the prompt drawer, type an instruction that includes the URL, such as `Use this URL to generate an ad for this channel: https://www.example.com`.

>[!NOTE]
>Enter the URL in your prompt. Do not add it through _Parameters_.

## Related capabilities

- [Manage variants](/help/user-guide/create/manage-variants.md): Edit and fine-tune generated variants directly on the Canvas.
- [Write effective prompts](/help/user-guide/effective-prompts.md): Craft prompts that produce better results.
