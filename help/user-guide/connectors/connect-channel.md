---
title: Connect paid media
description: Connect a channel account to activate and monitor your ads and media with Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Admin, Data Engineer
feature: Reporting and Insights
exl-id: e699041e-b462-45b3-8c4c-4de0d52cf0e6
---
# Connect paid media accounts

_[!DNL Data connectors]_ enable seamless integration between GenStudio for Performance Marketing and your paid media network accounts. By connecting to third-party channel accounts, you can exchange critical data, such as campaign performance metrics in [[!DNL Insights]](/help/user-guide/insights/overview.md), and you can deliver fresh ad placements with [[!DNL Activate]](/help/user-guide/activation/overview.md). This integration allows GenStudio for Performance Marketing to manage your media and ads while receiving valuable insights, including impressions, clicks, and conversions, from your active campaigns.

**To connect to a paid media account**:

1. Click the ellipsis **[!UICONTROL ... More]** in the lower left navigation.

1. Select **[!UICONTROL Settings]** with the cog icon.

1. In _[!UICONTROL Settings]_, choose a connector type from the _[!UICONTROL Data connectors]_ section, and click **[!UICONTROL Connect]**.

   Optionally, if there are connected accounts, you can click on _connected accounts_ to view a list of account names, details, and status.

1. See the [connector type](#connector-types) you selected, review the prerequisites, and continue with the connection steps.

## Paid media connections

GenStudio for Performance Marketing supports various connector types to integrate with your preferred marketing platforms. Each connector type has specific prerequisites and set-up steps to complete for a successful connection.

### Google Campaign Manager 360 connect

>[!BEGINSHADEBOX]

**Prerequisites**:

- Google Campaign Manager 360 account
- Remove any pop-up blockers in your browser

>[!ENDSHADEBOX]

**To connect a Google Campaign Manager 360 account**:

1. In the _Data connectors_ section, click **[!UICONTROL Connect]** on the _Google Campaign Manager 360_ card.

1. Log in to your Google Campaign Manager 360 account.

   You may have to remove the pop-up blockers, and then use **[!UICONTROL Refresh]** to try again.

1. Read the terms and conditions and click **[!UICONTROL Allow]** to grant access.

1. In the _[!UICONTROL Google Campaign Manager 360]_ view, select one or more advertisers and click **[!UICONTROL Select]**.

The _[!UICONTROL Google Campaign Manager 360 accounts]_ view lists the `Account name`, `Added by`, `Date added`, and `Status`. Use **[!UICONTROL Add account]** to add more accounts to the list.

### Meta ads connect

When you connect your _Meta Business_ profile to GenStudio for Performance Marketing, it ensures seamless access to advertising data for your business Pages, Meta Ads accounts, and other Meta assets.

>[!BEGINSHADEBOX]

**Prerequisites**:

- Facebook/Meta login that can access all Meta services, such as Meta Ads account and Facebook Business Profile
- Access to Meta ads account with `View performance` permission level for accessing reports and viewing ads, including the following
   - Permissions required for use with [!DNL Insights]:

      - `pages_show_list`
      - `ads_read`
      - `ads_management`
      - `pages_read_engagement`

   - Permissions required for use with [!DNL Activate]:

      - `ads_management`
      - `ads_read`
      - `business_management`
      - `instagram_basic`
      - `instagram_content_publish`
      - `pages_manage_ads`
      - `pages_manage_posts`
      - `pages_show_list`

- Remove any pop-up blockers in your browser

>[!ENDSHADEBOX]

**To connect a Meta ads account**:

1. In the _Data connectors_ section, click **[!UICONTROL Connect]** on the _Meta Ads_ card.

1. Log in to your Facebook account.

   You may have to remove the pop-up blockers, and then use **[!UICONTROL Refresh]** to try again.

1. Follow the Facebook authentication instructions, verify the account information, and click **[!UICONTROL Continue as ...]**

1. In _[!UICONTROL Facebook Login for Business]_ (Meta to Adobe symbol), step through the following selections to grant GenStudio for Performance Marketing access:

   - Select one or more Meta Business profiles and click **[!UICONTROL Continue]**
   - Select one or more Meta Pages and click **[!UICONTROL Continue]**
   - Select one or more Instagram accounts and click **[!UICONTROL Continue]**
   - Review selections and click **[!UICONTROL Save]**

1. Once you receive verification that your account is connected, click **[!UICONTROL Got it]**.

   This step ensures that GenStudio for Performance Marketing gains access to all ads, metadata, and metrics for optimal performance.

1. In _[!UICONTROL Meta Ads]_, select one or more accounts to include in [!DNL Insights] and click **[!UICONTROL Select]**.

1. Once you receive a _Platform connected_ confirmation, click **[!UICONTROL View accounts]**.

   The _[!UICONTROL Meta Ads accounts]_ view lists the `Account name`, `Added by`, `Date added`, and `Status`. 

Use **[!UICONTROL Add account]** to add more accounts to the list. The authorization flow may differ slightly when you add accounts linked to the same Meta Business profile. You select only the new Meta Ads accounts during the connection process.

## Data ingestion

Initially, GenStudio for Performance Marketing imports the most recent six months of historical data. This practice ensures you have immediate access to relevant insights for analyzing trends, evaluating performance, and making informed decisions. The ingestion process may take one to five days depending on the volume of data in your account.

>[!BEGINSHADEBOX]

**Data Ingestion and Retention Policy**

GenStudio for Performance Marketing retains channel data for 13 months. This retention policy includes the 6 months of data ingested during the initial connection, ensuring comprehensive historical data analysis and reporting.

>[!ENDSHADEBOX]
