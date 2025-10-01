---
title: Connect to Meta Ads
description: Connect a Meta Ads account to activate and monitor your ads and media with Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Admin, Data Engineer
recommendations: noDisplay
feature: Reporting and Insights
exl-id: 78110edf-947b-4e05-a3f1-de4b1eabda44
---
# Connect to Meta Ads

This page explains how to connect and manage your Meta Ads profile account to GenStudio for Performance Marketing to manage campaigns, export content, and access advertising data for your active campaigns.

>[!BEGINSHADEBOX]

**Prerequisites**:

- Facebook/Meta login that can access all Meta services

- _Full control_ over Meta Business Portfolio and Ad Accounts, including:

  - Manage campaigns
  - View performance
  - Manage Creative Hub mockups
  - Advanced analytics

- Disable any pop-up blockers in your browser

>[!ENDSHADEBOX]

## Connect a Meta ads account

1. Click **[!UICONTROL More]** > **[!UICONTROL Settings]**.

1. In the _Data connectors_ section, click **[!UICONTROL Connect]** on the _Meta Ads_ card.

1. Log in to your Facebook account.

   You may have to remove the pop-up blockers, and then use **[!UICONTROL Refresh]** to try again.

1. Follow the Facebook authentication instructions, verify the account information, and click **[!UICONTROL Continue as ...]**

1. In _[!UICONTROL Facebook Login for Business]_ (Meta to Adobe symbol), step through the following selections to grant GenStudio for Performance Marketing access:

   - Select one or more Meta Business profiles and click **[!UICONTROL Continue]**
   - Select one or more Meta Pages and click **[!UICONTROL Continue]**
   - Select one or more Instagram accounts and click **[!UICONTROL Continue]**
   - Review selections and click **[!UICONTROL Save]**

     ![Review selections](/help/assets/meta/meta-review-selections.png "Review selections"){width="400" zoomable="yes"}

1. Once you receive verification that your account is connected, click **[!UICONTROL Got it]**.

   This step ensures that GenStudio for Performance Marketing gains access to all ads, metadata, and metrics for optimal performance.

1. In _[!UICONTROL Meta Ads]_, select one or more accounts to include in [!DNL Insights] and click **[!UICONTROL Select]**.

1. Once you receive a _Platform connected_ confirmation, click **[!UICONTROL View accounts]**.

   The _[!UICONTROL Meta Ads accounts]_ view lists the `Account name`, `Added by`, `Date added`, and `Status`.

   ![Meta accounts list](/help/assets/meta/meta-accounts-list.png "List of connected Meta accounts"){zoomable="yes"}

Use **[!UICONTROL Add account]** to add more accounts to the list. The authorization flow may differ slightly when you add accounts linked to the same Meta Business profile. You select only the new Meta Ads accounts during the connection process.

## Disconnecting and troubleshooting a Meta Ads integration

Sometimes a GenStudio for Performance Marketing instance is connected to a Meta Ads Account incorrectly. Common setups that can cause issues include:

- An Instagram account is selected without selecting its associated Facebook page
- Revoked permissions for a user that performed the initial connection

In these situations, it's best to reconnect the Meta Ad Account to the GenStudio for Performance Marketing instance. First, the user must remove the app integration directly from their Meta Business Manager, creating a clean slate for resetting permissions. This requires admin access to the Meta Business Manager. 

These steps clear cached permissions and reset the integration flow:

1. Access [Meta Business Manager](https://business.facebook.com) by visiting the Facebook website.
1. Log in with your account. The account must have admin access to the Business Manager.
1. Click the **[!UICONTROL Settings]** cog icon in the lower left to navigate to your Business Portfolio settings.
1. In the left-hand menu, click **[!UICONTROL Integrations]**.
1. Select **[!UICONTROL Connected Apps]**. You'll see Adobe GenStudio in the list of Connected apps. 
![Meta Business Manager Connected Apps](./meta-connected-apps.png "Meta Business Manager Connected Apps pane")
1. Click the app name.
1. Click **[!UICONTROL Remove]**.
1. Confirm the removal when prompted.

You can now reconnect your Meta ad accounts, Instagram profiles, and Facebook pages.
