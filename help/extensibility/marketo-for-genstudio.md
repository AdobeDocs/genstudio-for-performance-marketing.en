---
title: Marketo for GenStudio
description: Install and configure the Marketo for GenStudio Adobe Exchange app so your organization can use Marketo Engage templates in GenStudio for Performance Marketing.
feature: Extensibility
---
# Marketo for GenStudio

Organizations that use [!DNL Marketo Engage] and [!DNL GenStudio for Performance Marketing] in the same [!DNL IMS] organization can install the **Marketo for GenStudio** app from [!DNL Adobe Exchange]. After a system administrator approves the app and completes deployment, authors can choose Marketo templates while creating email experiences in GenStudio, next to templates uploaded directly to [!DNL Content].

This topic is for **administrators** who install the app, gather credentials from Marketo, and deploy the app in Exchange. For how AJO and Marketo template syntax works with GenStudio, see [Templates from AJO and Marketo](/help/user-guide/templates/use-templates.md#templates-from-ajo-and-marketo).

## Prerequisites

* [!DNL Marketo Engage] must be provisioned in the organization where you deploy the extension.
* Users who deploy the application need **Marketo credentials**. To create and retrieve those credentials, you must have **Marketo Product Admin** access (the **[!UICONTROL Admin]** area must be available when you open Marketo).

## Install the app from Adobe Exchange

>[!VIDEO](https://video.tv.adobe.com/v/3483299?learn=on)

1. Open [Adobe Exchange](https://exchange.adobe.com) and go to **[!UICONTROL Experience Cloud]**.
1. Open the [Marketo for GenStudio](https://exchange.adobe.com/apps/ec/ab6p21vo8r/marketo-for-genstudio) listing.
![Marketo for GenStudio listing on Adobe Exchange](/help/extensibility/marketo-adobe-exchange.png){width="75%"}
1. Select **[!UICONTROL Free]** to request the app for your organization.
1. After your organization **reviews and approves** the request, continue with [Get Marketo credentials](#get-marketo-credentials) and [Deploy the application from Exchange](#deploy-the-application-from-exchange).

## Get Marketo credentials

You use credentials from your **Marketo** instance (not the Adobe Developer Console). Collect the following credentials using the steps below before you deploy in Exchange.

>[!NOTE]
>
>To generate and retrieve Marketo credentials, you need to have Marketo Product Admin access, otherwise the Admin tab is not visible in Marketo.

### Create an API-only user (optional if you reuse an existing API user)

1. In Marketo, go to **[!UICONTROL Admin]**.
![Marketo Admin tab](/help/extensibility/marketo-admin-global.png){width="80%"}
1. Under **[!UICONTROL Security]**, open **[!UICONTROL Users & Roles]**  and go to the **[!UICONTROL Roles]** tab.
1. Create a new role or edit an existing role, with the following permissions added: _Access API_ and _Access Design Studio_.
1. For a new API user, click **[!UICONTROL Create API Only User]** (use a unique email for each API user).
1. Select the checkbox for Roles and assign the new role you created. If you already have an API user you want to use, skip to [Create or select a LaunchPoint service](#create-or-select-a-launchpoint-service).

![Users & Roles with API Only User and API roles](/help/extensibility/marketo-users-roles-api-user.png){width="80%"}

### Create or select a LaunchPoint service

1. In **[!UICONTROL Admin]**, under **[!UICONTROL Integration]**, open **[!UICONTROL LaunchPoint]**.
1. Click **[!UICONTROL Create]** to create a new Service (or use an existing custom service).
![LaunchPoint custom service](/help/extensibility/marketo-launchpoint-custom-service.png){width="80%"}
1. For your service, click **[!UICONTROL View Details]** and copy the **[!UICONTROL Client ID]** and **[!UICONTROL Client Secret]**. You will enter these in Adobe Exchange **[!UICONTROL Configuration]**.

### Note your Marketo REST API base URL

1. In **[!UICONTROL Admin]**, under **[!UICONTROL Integration]**, open **[!UICONTROL Web Services]**.
1. Find the **[!UICONTROL REST API]** endpoint. Copy only the **base URL** (host), in the form `https://###-XXX-###.mktorest.com`. Do **not** include path segments such as `/rest` or `/identity`. This value is unique per Marketo instance.

![Web Services REST API endpoint base URL](/help/extensibility/marketo-web-services-rest-endpoint.png){width="80%"}

You will also need the **[!UICONTROL Marketo Engage Identity URL]** that your Exchange deployment screen requests, alongside the REST base URL and the Client ID and Client Secret from LaunchPoint.

## Deploy the application from Exchange

To make the extension available in GenStudio, deploy the app from Adobe Exchange.

1. Return to [Adobe Exchange](https://exchange.adobe.com).
1. Select **[!UICONTROL Manage]** and open the **Marketo for GenStudio** app (for example under **[!UICONTROL App Builder applications]** or your organization's managed apps).
1. Under **[!UICONTROL Environments]**, choose an existing environment from the dropdown or select **[!UICONTROL Add Environment]** to create one.
1. Open **[!UICONTROL Configuration]** for the selected environment.
1. Enter the **[!UICONTROL Client ID]** and **[!UICONTROL Client Secret]** from [LaunchPoint](#create-or-select-a-launchpoint-service), the **[!UICONTROL Marketo Engage Identity URL]**, and the **[!UICONTROL Marketo Engage REST API Base URL]** (the base host from [Web Services](#note-your-marketo-rest-api-base-url)).
1. Click **[!UICONTROL Deploy]**. When deployment succeeds, the action changes to **[!UICONTROL Undeploy]**.

### Update configuration

To change configuration values for an environment, **[!UICONTROL Undeploy]** first, update the fields, then **[!UICONTROL Deploy]** again.

### Workspace configuration (optional)

You may skip this step if you intend to use the default workspace. By default, the **Workspace ID** and **Template List Page Size** fields are preconfigured.

However, if you need to fetch templates from a different workspace:

1. In Marketo, navigate to **[!UICONTROL Admin]** → **[!UICONTROL Security]** → **[!UICONTROL Workspaces & Partitions]**.
1. The **Workspace ID** column is hidden by default. To enable it, r1.ight-click on the header row (where column names are displayed).
1. Select **[!UICONTROL Columns]**.
1. Enable **[!UICONTROL ID]** from the list.
![Workspaces & Partitions with Workspace ID column enabled](/help/extensibility/marketo-workspace-id.png){width="80%"}

Once visible, use the appropriate **Workspace ID** for your configuration.

## Access Marketo templates in GenStudio

After Marketo for GenStudio is installed and configured, a **[!UICONTROL Marketo Templates]** tab appears when you create an **Email** experience in GenStudio. Use that tab to browse templates from Marketo Engage.

>[!IMPORTANT]
>
>Create emails under the **standard Email** experience flow in GenStudio for Performance Marketing. This integration does NOT support emails created with the new email editor experience.

![Exchange Configuration with Marketo credentials](/help/extensibility/marketo-exchange-configuration.png){width="80%"}

## Troubleshooting

### Marketo Templates tab is not visible

* Confirm the app is **Approved** in Exchange and the environment is **deployed** with valid Client ID, Client Secret, and Marketo base URLs.
* Ask your administrator to verify **Marketo Product Admin** access was used when creating credentials.

### Templates do not load

* Reload the page or sign out and back in to GenStudio.
* In the browser developer tools **[!UICONTROL Network]** panel, look for failed API calls to your Marketo instance and verify the REST base URL matches **[!UICONTROL Web Services]** in Marketo (no extra path after the host).
