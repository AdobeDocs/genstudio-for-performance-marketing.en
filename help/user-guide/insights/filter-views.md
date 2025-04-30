---
title: Filter Insights views
description: Learn how to use the enhanced filter capabilities with Insights.
level: Intermediate
feature: Reporting and Insights
---
# Filter for Insights views

The [!DNL Insights] dashboard provides a comprehensive set of filters for an efficient data exploration experience. When analyzing channels, ads, media, or specific attributes, the filtering options allow you to customize your view and streamline your workflow. Use keyword filters for precise targeting or explore predefined lists to refine your search and focus on the data that matters most.

## Filter basics 

Each view in [!DNL Insights] offers a list of filter options. The filter (funnel) icon above the left side of the table opens the **[!UICONTROL Filter]** menu. Whether you are viewing the table or the gallery, applied filters appear in the **[!UICONTROL Filter by]** list above the table or gallery. By default, a channel and an account are selected.

![Filter by](/help/assets/insights-filter-by.png "Filter by"){width=400 zoomable="yes"}

Applied filters persist across all views. Select **[!UICONTROL Clear all]** above the table or gallery to remove all selected filters.

### Keyword filters

With _[!UICONTROL Campaigns]_ and _[!UICONTROL Ads]_ filters, you can leverage precise keywords to refine the list. Keyword filters are particularly useful for filtering campaigns or ads that use a complex naming convention with multiple unique identifiers. For example, a campaign name may include the following:

- Specific region name or code: `NA`, `EMEA`
- Content type acronyms: `EB`, `CHT`, or `DSP`
- Offer codes or acronyms: `OFFER2023`, `PROMO`

Over time, the list of campaigns and ads grow exponentially. Consider the following scenario to use the _[!UICONTROL Campaigns]_ filter to refine the [!UICONTROL Ads] table.

**To refine the Ads table using the Campaigns filter**:

1. In _[!DNL Insights]_, select the **[!UICONTROL Ads]** view.

   ![Ads filter and table](/help/assets/insights-ads-filter.png "Ads view with filter list"){zoomable="yes"}

1. Click the filter (funnel) icon above the left side of the table to open the **[!UICONTROL Filter]** menu.

1. Verify the correct `Filter by` channel and account is selected.

1. Expand the **[!UICONTROL Campaigns]** filter and click **[!UICONTROL Select]**.

   ![Filter campaigns](/help/assets/insights-filter-campaigns-expand.png "Expand campaigns filter"){width=200}

1. In the _[!UICONTROL Select campaigns]_ search field, enter keywords separated by commas.

   Use as many keywords as needed to refine the list. This example looks for campaigns that are `evergreen`, `ROI`, and `Meta`:

   ![Select campaigns](/help/assets/insights-select-campaigns-keywords.png "Enter keywords to search campaign names"){width=400}

1. Select one or more campaigns from the resulting search and click **[!UICONTROL Apply]**.

   ![List of campaigns](/help/assets/insights-select-campaigns-list.png)

Your selected campaigns are now displayed in the _[!UICONTROL Filter by]_ list above the ads table or gallery. You can focus exclusively on the ads linked to the chosen campaigns. In this example, the filtered results include 28 ads, providing a more targeted view for analysis.

![Table filtered by campaigns](/help/assets/insights-filter-by-campaigns.png "Table with campaigns filter"){zoomable="yes"}

You can further filter the [!UICONTROL Media] table in a similar way for ad names. Expand the **[!UICONTROL Ads]** filter and click **[!UICONTROL Select]** and you can perform a similar keyword filter to refine your media table or gallery view.

## Download table results

You can download the filtered results from the table view for further analysis or sharing. Click the download (arrow pointing down) icon above the right side of the table to download a CSV file based on the viewable table. The download automatically begins and places the CSV file in your default download location.

Some tables may have multiple pages, which you can see below the right side of the table. The CSV file includes data from _all_ pages of the table.
