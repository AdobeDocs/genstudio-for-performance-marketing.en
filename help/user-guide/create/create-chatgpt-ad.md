---
title: Create a ChatGPT Ad Experience
description: Learn how to create, review, publish, and activate ChatGPT paid media experiences in Adobe GenStudio for Performance Marketing.
feature: Create Canvas, Create Prompt, Generative AI, Variant Generation, Content Generation
role: User
level: Beginner
---

# Create a ChatGPT ad experience

Use [[!DNL Create]](/help/user-guide/create/overview.md) in [!DNL GenStudio for Performance Marketing] to build **ChatGPT ads** as paid media experiences—from guidelines and assets through generation, brand and channel checks, approval, publishing to [!DNL Content], and activation in the same [!DNL Activate] flow used for channels such as Meta and Google Campaign Manager 360.

Before you begin, [add guidelines](/help/user-guide/guidelines/add-guidelines.md) where needed and review [effective prompts](/help/user-guide/effective-prompts.md) so your headline prompts produce strong variants.

## Prerequisites

You'll need to be set up according to these prerequisites before you create or activate ChatGPT ads in [!DNL GenStudio for Performance Marketing].

### Access and roles

* You have an **Editor** role or higher in [!DNL GenStudio for Performance Marketing]. See [User roles and permissions](/help/user-guide/user-roles.md).
* You have an **OpenAI Ad Account** and an **API key** from that account.
* A **ChatGPT Ads** account is connected to [!DNL GenStudio for Performance Marketing].

To create an API key in OpenAI Ads Manager:

1. In OpenAI Ads Manager, go to **[!UICONTROL Settings]** > **[!UICONTROL API Keys]** > **[!UICONTROL Create New Key]**.

To connect your ChatGPT Ads account in [!DNL GenStudio for Performance Marketing]:

1. In the lower-left area, click **[!UICONTROL More]** > **[!UICONTROL Settings]** > **[!UICONTROL ChatGPT]** > **[!UICONTROL Connect]** > **[!UICONTROL Add Account]**.
1. Enter the name of your OpenAI Ad Account, paste your API key, and click **[!UICONTROL Add Account]**.

Your ad account is connected when the flow completes successfully.

### Create configuration

* **[!DNL Brands]**, **[!DNL Products]**, and **[!DNL Personas]** are configured so the app can generate on-brand copy. See [Guidelines overview](/help/user-guide/guidelines/overview.md).
* Images you want to use are available in [[!DNL Content]](/help/user-guide/content/overview.md).

## Generate a ChatGPT ad

You create ChatGPT ads as paid media experiences in the [!DNL Create] workspace.

### Start a ChatGPT experience

To open ChatGPT creation:

1. Go to **[!UICONTROL Create]** > **[!UICONTROL ChatGPT]**. You do not select templates for ChatGPT; a single ad layout is used.
![ChatGPT tile in the Create workflow](./create-chatgpt-clp.png){width="60%"}
1. In the _Canvas_, make selections for **[!DNL Brand]**, **[!DNL Product]**, **[!DNL Persona]**, and **Language**.
1. Select an image from [!DNL Content].
1. Enter a prompt for your ChatGPT headline copy.
1. Click **[!UICONTROL Generate]**.

[!DNL GenStudio for Performance Marketing] **generates four** creative variants.

You can:

* Use **[!UICONTROL Regenerate]** or **[!UICONTROL Refine]** to adjust tone, length, or emphasis.
* Edit text directly in the _Canvas_.
* Use **[!UICONTROL Swap]** to choose an alternative image from [!DNL Content].

See [Manage variants](/help/user-guide/create/manage-variants.md) for more ways to edit generated experiences.

### Run brand and channel checks

Before you save or send the experience for review, validate copy and layout against brand and channel rules.

To run content checks:

1. Click **[!UICONTROL Content check]** (brand and channel checks).
1. Review validation results in the [_Content check_ panel](/help/user-guide/guidelines/brand-validation.md#content-check-panel).
1. Resolve any flagged issues—for example copy length or dense on-screen text—by editing variants or regenerating as needed.

See [Brand validation](/help/user-guide/guidelines/brand-validation.md).

## Save a ChatGPT ad in [!DNL GenStudio for Performance Marketing]

Saving moves your ChatGPT ad experience into [!DNL Content] so it can be reviewed, reused, and activated.

There are two states:

* **Draft experience** — Work in progress and not approved.
* **Published experience** — Approved and available in [!DNL Content] for activation.

### Send for review

1. From the experience header, click **[!UICONTROL Request review]**.
1. Select approvers (for example brand, legal, or performance stakeholders).
1. Optional: Add a note in **[!UICONTROL Settings]**.
1. Click **[!UICONTROL Send for review]**.

Approvers can view the ChatGPT experience, brand and channel check results, and **[!UICONTROL Approve]** or request changes.

See [Request review and approval](/help/user-guide/approvals/request-review.md) and [Reviews and approvals](/help/user-guide/approvals/overview.md).

### Publish to Content

After all required approvals, publish to [!DNL Content]:

1. Click **[!UICONTROL Publish to Content]**.
1. Confirm metadata—for example campaign or activation name, region, language, persona, funnel stage, and **Channel: ChatGPT**.
1. Click **[!UICONTROL Publish]**.

The ChatGPT ad appears in [!DNL Content]—discoverable with filters such as channel or campaign—and is ready for selection in [!DNL Activate].

See [Publish approved content](/help/user-guide/approvals/publish-content.md) and [[!DNL Content] overview](/help/user-guide/content/overview.md).

## Activate a ChatGPT ad

ChatGPT activation uses the same [[!DNL Activate]](/help/user-guide/activation/overview.md) module as Meta and Google Campaign Manager 360. See [Create an activation](/help/user-guide/activation/create-activation.md) for the shared activation workflow.

### Start a ChatGPT activation

You can start from [!DNL Content] or from [!DNL Activate].

**From [!DNL Content]**

* Select one or more **published** ChatGPT experiences.

**From [!DNL Activate]**

* Open the **ChatGPT** card and click **[!UICONTROL + New]**.

Each experience maps to **one** ChatGPT ad.

### Configure experience setup

For each selected experience, confirm:

* **Title**
* **Body**
* **Target URL** — Must use valid `https://` format (for example `https://www.example.com`).

### Configure platform setup

Select ChatGPT Ads Manager details:

* **OpenAI Ads account**
* **ChatGPT Campaign** — Must already exist in OpenAI Ads Manager.
* **ChatGPT Ad group** — Must already exist in OpenAI Ads Manager.
* **ChatGPT Ad name** — One distinct name per ChatGPT ad.

### Review and publish

1. Review all creative and platform details.
1. Click **[!UICONTROL Publish]**.

[!DNL GenStudio for Performance Marketing] pushes ads to ChatGPT Ads Manager in an **inactive** state so your media team controls final launch timing and budget—consistent with other paid channels. See [Activate overview](/help/user-guide/activation/overview.md).

### What happens after you publish

* A **publishing in progress** modal appears and closes automatically.
* You are redirected to the **ChatGPT Activation** table, which lists the latest activations. Status shows **[!UICONTROL Pending]** while processing completes.
* You can navigate away while publishing finishes.

When processing completes:

* A confirmation pop-up shows **success** or **failure**.
* If you click the pop-up—or open the ChatGPT activation in the activation table—you see the **Details** page.
* If activation **[!UICONTROL Failed]**, the table shows that status plus an error message from ChatGPT.

In OpenAI Ads Manager, media teams can run final checks and turn ads or ad groups live when ready.
