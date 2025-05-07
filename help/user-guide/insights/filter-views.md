---
title: Filter Insights views
description: Learn how to use the enhanced filter capabilities with Insights.
level: Intermediate
feature: Reporting and Insights
exl-id: fbc53c2a-388c-4b51-94e2-626cd1e18e63
---
# Filter for Insights views

The [!DNL Insights] dashboard provides a comprehensive set of filters for an efficient data exploration experience. When analyzing channels, ads, media, or specific attributes, the filtering options allow you to customize your view and streamline your workflow. Use keyword filters for precise targeting or explore predefined lists to refine your search and focus on the data that matters most.

## Filter basics

Each view in [!DNL Insights] offers a list of filter options. The filter (funnel) toggle above the left side of the table opens the **[!UICONTROL Filter]** menu. Whether you are viewing the table or the gallery, applied filters appear in the **[!UICONTROL Filter by]** list above the table or gallery. By default, a channel and an account are selected.

![Filter by](/help/assets/insights-filter-by.png "Filter by"){width=600 zoomable="yes"}

Applied filters persist across all views. Select **[!UICONTROL Clear all]** above the table or gallery to remove all selected filters.

### Search field

Click the search (magnifying glass) icon to type a search term to locate specific items in the table or gallery. For example, entering the term `Gear` in the [!UICONTROL Ads] table filters the results to display only ads using the term `Gear` in the name.

![Search field example](/help/assets/insights-search.png "Search for ads with Gear in the name"){width=600 zoomable="yes"}

### Date range

The date range selector is a powerful tool to align the displayed data with your analysis objectives. Use the date range selector to adjust the time frame for the data displayed in the table or gallery view. By default, the date range is set to the last 30 days. To include more data or focus on a specific period, expand the date range.

![Date range selector](/help/assets/insights-date-range.png "Select a date range"){width=400}

If no items appear in the table or gallery view, it may be due to the selected date range excluding relevant data. In such cases, increase the date range to ensure that the desired data is included.

### Pages

Some tables may span multiple pages, as indicated below the table on the right side. Use the versatile search and filter options to refine your results. To navigate between pages, use the right (forward) and left (back) pagination controls. Ensure that you apply filters correctly to include all relevant data across pages.

### Slide control

Some filter options include a slide control, which allows you to select a value within a defined range. For example, in _[!UICONTROL Attributes]_, the **[!UICONTROL Media count]** slider lets you filter attributes based on the number of associated images or videos. Drag the slider to specify a range, starting from a minimum of 0 to a maximum that can exceed 100.

## Advanced filtering

With _[!UICONTROL Campaigns]_ and _[!UICONTROL Ads]_ filters, you can leverage precise keywords to refine the list. Keyword filters are particularly useful for filtering campaigns or ads that use a complex naming convention with multiple unique identifiers. For example, a campaign name may include the following:

- Specific region name or code: `NA`, `EMEA`
- Content type acronyms: `EB`, `CHT`, or `DSP`
- Offer codes or acronyms: `OFFER2023`, `PROMO`

Over time, your list of campaigns and ads may grow exponentially. Consider the following scenario to use the _[!UICONTROL Campaigns]_ filter to refine the [!UICONTROL Ads] table.

**To refine the Ads table using the Campaigns filter**:

1. In _[!DNL Insights]_, select the **[!UICONTROL Ads]** view.

   ![Ads filter and table](/help/assets/insights-ads-filter.png "Ads view with filter menu"){zoomable="yes"}

1. Click the filter (funnel) toggle above the left side of the table to open the **[!UICONTROL Filter]** menu.

1. Verify the correct `Filter by` channel and account is selected.

1. Expand the **[!UICONTROL Campaigns]** filter and click **[!UICONTROL Select]**.

   ![Filter campaigns](/help/assets/insights-filter-campaigns-expand.png "Expand campaigns filter"){width=200}

1. In the _[!UICONTROL Select campaigns]_ search field, enter keywords separated by commas.

   Use as many keywords as needed to refine the list.

   - Search for `adventure` **AND** `ready`:

     ![Search all keywords](/help/assets/insights-select-campaigns-and.png "Search for campaign names that contain keywords"){width=400}
   
   - Search for `adventure` **OR** `ready`:

     ![Search either keywords](/help/assets/insights-select-campaigns-or.png "Search for campaign names that contain at least one set of keywords"){width=400}
 
   You can add another set of keywords to broaden your search. Using multiple sets of keywords allows you to include campaigns that match either the first set of keywords or the second set of keywords.
   
   - Search for `adventure` and `apparel` _OR_ `sun` and `gear`:

     ![Search with multiple sets of keywords](/help/assets/insights-advanced-or.png "Search campaign names using multiple sets of keywords"){width=400}

1. Select one or more campaigns from the resulting search and click **[!UICONTROL Apply]**.

   ![List of campaigns](/help/assets/insights-select-campaigns-list.png "Select campaigns to include")

Your selected campaigns now appear in the _[!UICONTROL Filter by]_ list above the ads table or gallery. You can focus exclusively on the ads linked to the chosen campaigns. In this example, the filtered results include 6 ads, providing a more targeted view for analysis.

![Table filtered by campaigns](/help/assets/insights-filter-by-campaigns.png "Table with campaigns filter"){zoomable="yes"}

You can further filter the [!UICONTROL Media] table in a similar way for ad names. Expand the **[!UICONTROL Ads]** filter and click **[!UICONTROL Select]** and you can perform a similar keyword filter to refine your media table or gallery view.

## Download table results

You can download the filtered results from the table view for further analysis or sharing. Click the download (arrow pointing down) icon above the right side of the table to download a CSV file based on the viewable table. The download automatically begins and places the CSV file in your default download location.

Some tables may have multiple pages, which you can see below the right side of the table. The CSV file includes data from _all_ pages of the table.
