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

**To connect a Google Campaign Manager account**:

1. In the _Data connectors_ section, click **[!UICONTROL Connect]** on the _Google Campaign Manager 360_ card.

1. Log in to your Google Campaign Manager 360 account.

   You may have to remove the pop-up blockers, and then use **[!UICONTROL Refresh]** to try again.

1. Read the terms and conditions and click **[!UICONTROL Allow]** to grant access.

1. In the _[!UICONTROL Google Campaign Manager 360]_ view, select one or more advertisers and click **[!UICONTROL Select]**.

The _[!UICONTROL Google Campaign Manager 360 accounts]_ view lists the `Account name`, `Added by`, `Date added`, and `Status`. Use **[!UICONTROL Add account]** to add more accounts to the list.

### Meta ads connect

>[!BEGINSHADEBOX]

**Prerequisites**:

- Facebook/Meta ads account
- Access to Meta ads account with `View performance` permission level for accessing reports and viewing ads
- Remove any pop-up blockers in your browser

>[!ENDSHADEBOX]

**To connect a Meta ads account**:

1. In the _Data connectors_ section, click **[!UICONTROL Connect]** on the _Meta Ads_ card.

1. Log in to your Facebook account.

   You may have to remove the pop-up blockers, and then use **[!UICONTROL Refresh]** to try again.

1. Follow the Facebook authentication instructions.

1. In the _[!UICONTROL Facebook Login for Business]_ pop-up (Meta to Adobe symbol), step through the following selections.

   - Verify the account information and click **[!UICONTROL Continue as]**
   - Grant access to select Pages and click **[!UICONTROL Continue]**
   - Grant access to select Businesses and click **[!UICONTROL Continue]**
   - Opt in to one or more Instagram accounts and click **[!UICONTROL Continue]**
   - Review selections and click **[!UICONTROL Save]**

1. In the _[!UICONTROL Meta Ads]_ view, select one or more accounts and click **[!UICONTROL Select]**.

The _[!UICONTROL Meta Ads accounts]_ view lists the `Account name`, `Added by`, `Date added`, and `Status`. Use **[!UICONTROL Add account]** to add more accounts to the list.

## Data ingestion

Initially, GenStudio for Performance Marketing imports the most recent six months of historical data. This practice ensures you have immediate access to relevant insights for analyzing trends, evaluating performance, and making informed decisions. The ingestion process may take one to five days depending on the volume of data in your account.

>[!BEGINSHADEBOX]

**Data Ingestion and Retention Policy**

GenStudio for Performance Marketing retains channel data for 13 months. This retention policy includes the 6 months of data ingested during the initial connection, ensuring comprehensive historical data analysis and reporting.

>[!ENDSHADEBOX]
