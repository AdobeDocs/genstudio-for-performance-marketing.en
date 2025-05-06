---
title: Meta Ads connect
description: Connect a Meta Ads account to activate and monitor your ads and media with Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Admin, Data Engineer
feature: Reporting and Insights
---
# Meta Ads connect

Connect your _Meta Business_ profile to GenStudio for Performance Marketing to manage campaigns, export content, and access advertising data for your Meta Ads and media.

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
