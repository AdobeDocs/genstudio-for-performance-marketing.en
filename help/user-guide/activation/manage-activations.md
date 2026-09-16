---
title: Manage Activations
description: Learn how to manage activated experiences with Adobe GenStudio for Performance Marketing.
feature: Ad Activation
exl-id: 7cf340d4-37ab-4906-9aad-088a26db0818
TQID: https://experienceleague.adobe.com/ird0IiW8L5Axjj2FmEjlUcD1sPaNCNfxj9XNqGfQWiI
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
    internal-label: GenStudio for Performance Marketing
feature_v2:
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
    internal-label: Create
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
    internal-label: Metadata
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
---
# Manage activations

Your activation tables appear on the [!DNL Activate] landing page. Each table lists its ads, along with their status:

| Status | Meaning |
|---|---|
| [!UICONTROL Needs Attention] | At least one ad in the activation table has a missing or invalid field, such as an incompatible call to action, or a duplicate tracking ID. |
| [!UICONTROL Ready to Activate] | All ads in the activation table pass validation and are ready to publish. |
| [!UICONTROL Pending] | The entire activation table was submitted and is being processed by the destination platform. |
| [!UICONTROL Published] | The entire activation table published successfully. |
| [!UICONTROL Failed] | The destination platform rejected at least one of the ads in the table. Hover over the status tooltip to see the platform's error message. |

You can automatically retry failed activations by clicking **[!UICONTROL Try again]** in the top right.

Published rows are locked from resubmission and include a deep link to the ad in the destination platform's native ad manager, so you can jump directly to it to review or launch it.

## Details view

Click on an ad row to open a focused view of its activation details. The read-only details view captures the defining details of an activated ad, including failed activations, with information derived from both GenStudio for Performance Marketing and the destination platform:

* **Publication time and date**: Time and date of publication from the destination platform
* **Ad ID**: ID assigned by the destination platform and used for tracking, with a deep link to the published ad in the platform's native ad manager
* **Ad details**: The approved assets, copy, and metadata used for the ad
* **Platform setup**: The account, campaign, and other platform setup fields used to activate the ad

A failed activation's details view includes the reason for failure.
