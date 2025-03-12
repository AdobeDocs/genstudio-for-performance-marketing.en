---
title: Manage assets and experiences
description: Simplify and enhance the management of brand-approved assets for use and reuse in your digital marketing journey.
feature: Content, Assets, Experiences
exl-id: e2ce8797-6d3b-46d4-b12f-f5f80e26c669
---
# Manage assets and experiences

Adobe GenStudio for Performance Marketing [!DNL Content] simplifies and enhances the management of brand-approved assets for use and reuse in your digital marketing journey.

## [!DNL Content] gallery

The gallery shows an inventory of approved assets, experiences, or templates depending on the selected view. The filter (funnel) icon above the left side of the table opens the **[!UICONTROL Filter]** menu, where you can select from many categories to filter the content shown in the gallery. In the _[!UICONTROL Assets]_ view, click the search (magnifying glass) icon to use a keyword to find an asset.

The following shows a search on the term `dog` in the [!UICONTROL Assets] gallery:

![Assets view with search on dog](/help/assets/content-assets.png)

### Search content

The filter and search interface is quick and responsive, and provides a productive search-first experience. Each [!DNL Content] view provides filter options to narrow your search for the ideal asset, experience, or template. For assets and experiences, you can select a campaign and specific guidelines, such as content made for a specific product.

There are filters based on [keywords](asset-details.md#user-defined-metadata) and [attribute categories](/help/user-guide/insights/attributes.md#categories) to narrow search results. For example, you may want to find an asset of a particular file type or subject matter to help you build a new experience for your campaign. Or you can filter content based on your username or the name of a team member:

- **[!UICONTROL Uploaded by]** filter limits the _[!UICONTROL Assets]_ list to show only the assets uploaded by you or a specific person.
- **[!UICONTROL Created by]** filter limits the _[!UICONTROL Experiences]_ list to show only the experiences created by you or a specific person.

**To search for content to reuse**:

1. In _[!DNL Content]_, select the **[!UICONTROL Assets]** section.

1. Select an asset repository from the **[!UICONTROL Location]** list, or verify that you are looking at the correct asset repository. `GenStudio assets` is the default repository.

   >[!IMPORTANT]
   >
   >The _Location_ list is available only when you [connect to an AEM repository](connect-aem-repo.md).

1. Click **[!UICONTROL Search]** (magnifying glass) to enter a keyword or description.

1. Narrow your search by selecting a category from the _[!UICONTROL Filter]_ list. For example, if you are looking for a PNG file, click **[!UICONTROL File format]** and choose **PNG**.

   The more you narrow your search, the fewer filter options available. Click **[!UICONTROL Clear all]** to remove all filters.

1. Select an asset for a full view and a list of details.

   Click **[!UICONTROL Download]** (down arrow) to use the asset in your local workstation.

### Location

By default, assets that you add to [!DNL Content] through the [!DNL Create] process or through upload are stored in the `GenStudio assets` repository. The `GenStudio assets` repository is a read-write repository in GenStudio for Performance Marketing. This means that you can save, edit, and delete assets in the `GenStudio assets` repository.

The **[!UICONTROL Location]** list above the _[!UICONTROL Assets]_ gallery on the right side allows you to select from connected Adobe Experience Manager (AEM) [!DNL Assets Content Hub] repositories.

![Location list of repositories](../../assets/content-location-selection.png){width="350"}

When you select an AEM repository, the gallery shows an inventory of assets from that repository, allowing you to leverage approved assets from these repositories as inputs for content creation. The filter options change to reflect the categories configured in [!DNL AEM Assets Content Hub].

See [Connect an AEM repository](connect-aem-repo.md) for guidance on adding your [!DNL AEM Assets Content Hub] repository to GenStudio for Performance Marketing.

The AEM repository is read-only, which means that you can access the content but you cannot save drafts, new assets, or metadata to the AEM repository. All drafts and final updates for assets, experiences, and templates save to the `GenStudio assets` repository with new [system metadata](asset-details.md#system-metadata).

{{note-aem-assets}}

An AEM repository may enforce certain licensing requirements, such as asset expiration. These assets may not be available for use in [!DNL Create] workflows. Expired assets may need to be renewed or replaced to maintain the continuity of your projects. Consult your [!DNL AEM Assets Content Hub] administrator for assistance with these assets.

## Assets management

In [!UICONTROL Content], you can easily store, retrieve, and manage your digital assets. By leveraging both the `GenStudio assets` repository and AEM repositories, you can ensure that your assets are well-organized and accessible for various marketing campaigns. This multi-repository approach provides flexibility and control over asset usage across environments, ensuring that only approved and up-to-date assets are used in marketing efforts.

The following table lists the management tasks available for assets, experiences, and templates:

| Tasks                                                     | Assets | Experiences | Templates |
| --------------------------------------------------------- | :----: | :---------: | :-------: |
| [View details](/help/user-guide/content/asset-details.md) |   ✓    |     ✓       |     ✓     |
| [Create experience](/help/user-guide/create/overview.md)  |        |             |     ✓     |
| [Edit in Adobe Express](#edit-in-express)                 |   ✓    |             |           |
| [Export for Activation](#export-for-activation)           |        |     ✓       |           |
| [Refresh](/help/user-guide/content/use-templates.md#refresh-template) |   |      |     ✓     |
| [Download](#download-assets)                              |   ✓    |             |     ✓     |
| [Delete](#delete-assets)                                  |   ✓    |     ✓       |     ✓     |

### Add assets

When adding assets to [!DNL Content], they are by default stored in the `GenStudio assets` repository. The _[!UICONTROL Add assets]_ button is available only when the _[!UICONTROL Location]_ is the `GenStudio assets` repository.

![Location field](../../assets/content-location.png){width="350"}

**To add one or more assets**:

1. In _[!DNL Content]_, click **[!UICONTROL Add assets]**.

1. In the _Add your approved assets_ view, drop a file or files in the drop space. Optionally, you can select from local files using **[!UICONTROL Browse]** or import files from Dropbox or Microsoft OneDrive.

1. In the _Add details_ section, select a **[!UICONTROL Campaign name]** or enter a new name.

1. To improve discoverability, add optional details such as _Brand name_, _Personas_, _Region_ and _Keywords_ in the **More details** section.

   The more details that you provide, the more you experience the robust capabilities of GenStudio for Performance Marketing. Select one or more details from the list, or enter a new one where applicable, such as with keywords. Each detail you add appears below the list. Click **`x`** to remove a detail.

   Any details you add apply to all the assets added in this action.

   See [Metadata details](/help/user-guide/content/asset-details.md#system-metadata).

1. Click **[!UICONTROL Add assets]**.

1. When the asset upload is completed, click **Done**.

1. To view your new uploaded assets, click **[!UICONTROL Refresh]** from the _New assets available_ notification at the bottom of the Canvas.

### Download assets

**To download an asset**:

1. In _[!DNL Content]_, select an asset or template. Clicking on an asset opens a focused view of the asset.

1. In the asset view, click the **[!UICONTROL Download]** icon (arrow pointing down) in the upper right.

1. The download begins placing a copy of the asset in your default download location.

### Delete assets

**To delete an asset**:

1. In _[!DNL Content]_, select an asset, experience, or template. Clicking on an asset opens a focused view of the asset.

1. In the asset view, click **[!UICONTROL Delete]** (trash can) in the upper right.

1. In the _Delete asset_ popup, verify the asset and click **[!UICONTROL Delete]**.

## Export for activation

You can export an approved experience for activation in a format compatible with your target channel.

**To export an experience**:

1. In _[!DNL Content]_, select an experience. Clicking on an experience opens the details view or click the shortcut menu (`...`).

1. Click **[!UICONTROL Export for activation]** (box with arrow pointing out).

1. In the _Export for activation_ popup, select one of the available formats:

   - Email: `HTML`, `CSV`
   - Meta and display ads: `HTML`, `JPEG`, `PNG`

See [Activation](/help/user-guide/activation/overview.md).

## Edit in Express

You can edit image assets (JPG or PNG) directly within GenStudio for Performance Marketing using Adobe Express. The _[!UICONTROL Powered by Adobe Express]_ Canvas provides convenient features to enhance your images without leaving the GenStudio application. You can easily remove backgrounds, apply generative fills, adjust effects, and crop images.

>[!BEGINSHADEBOX]

Criteria for enhancing images with the [!DNL Edit in Adobe Express] feature:

- Supported MIME types include `image/png` and `image/jpeg`
- The minimum image dimensions are 50x50 pixels
- The maximum image dimensions are 8000x8000 pixels
- The maximum size is 40MB (40,000,000 bytes)

>[!ENDSHADEBOX]

**To edit an asset with Express**:

1. In _[!DNL Content]_, select an image asset. Clicking on an asset opens a focused view of the asset.

1. In the asset view, click the **[!UICONTROL Edit in Adobe Express]** icon in the upper right.

1. In the _[!UICONTROL Powered by Adobe Express]_ Canvas, use the Express controls on the left panel to enhance your image.

1. When you are happy with the updated image, click **[!UICONTROL Save a copy]** in the upper right.

1. Select the file format—JPG or PNG—and click **[!UICONTROL Save a copy]**.

1. In the _[!UICONTROL Save a copy of asset]_ popup, update the **[!UICONTROL Asset name]**.

   - Select **[!UICONTROL Same details as original asset]** to carry over the asset details to the new image.

   - Expand the **[!UICONTROL More details]** section to update the guidelines and other metadata.

   >[!TIP]
   >
   >The more details that you provide, the more you experience the robust capabilities of GenStudio for Performance Marketing. Select one or more details from the list, or enter a new one where applicable, such as with keywords. Each detail you add appears below the list. Click **`x`** to remove a detail.

1. Click **[!UICONTROL Save]**.
