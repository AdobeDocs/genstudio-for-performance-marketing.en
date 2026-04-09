---
title: Journey Optimizer for GenStudio
description: Install and configure the Journey Optimizer for GenStudio Adobe Exchange app so your organization can use Adobe Journey Optimizer templates in GenStudio for Performance Marketing.
feature: Extensibility
---
# Journey Optimizer for GenStudio

Organizations that use [!DNL Adobe Journey Optimizer] (AJO) and [!DNL GenStudio for Performance Marketing] in the same [!DNL IMS] organization can install the **Journey Optimizer for GenStudio** app from [!DNL Adobe Exchange]. After a system administrator approves the app and completes deployment, authors can choose AJO content templates while creating email experiences in GenStudio, next to templates uploaded directly to [!DNL Content].

This topic is for **administrators and developers** who install the app, create OAuth credentials in the [!DNL Adobe Developer Console], and map technical-account permissions in [!DNL Adobe Experience Platform]. For how AJO and Marketo template syntax works with GenStudio, see [Templates from AJO and Marketo](/help/user-guide/templates/use-templates.md#templates-from-ajo-and-marketo).

## Prerequisites

* AJO must be provisioned in the organization where you deploy the extension.
* Users who author templates in AJO need permission to **create and edit** content templates in Journey Optimizer, as your organization defines.
* Email templates in AJO must include field placeholders (handlebars) where generated content should appear. A template can be selected without those fields, but **experience generation fails** if the placeholders [!DNL GenStudio for Performance Marketing] expects are missing. See [Customize a template](/help/user-guide/templates/customize-template.md) and [Recognized field names](/help/user-guide/templates/customize-template.md#recognized-field-names).

## Install the app from Adobe Exchange

1. Open [Adobe Exchange](https://exchange.adobe.com) and go to **[!UICONTROL Experience Cloud]**.
1. Open the [Journey Optimizer for GenStudio](https://exchange.adobe.com/apps/ec/abpopqqr1q/journey-optimizer-for-genstudio) listing.
![Journey Optimizer for GenStudio listing on Adobe Exchange, including requirements and Free install](/help/extensibility/ajo-adobe-exchange.png){width="75%"}
1. Select **[!UICONTROL Free]** to request the app for your organization.
1. After your organization **reviews and approves** the request, continue with [Create OAuth credentials in Adobe Developer Console](#create-oauth-credentials-in-adobe-developer-console) and [Deploy the application from Exchange](#deploy-the-application-from-exchange).

## Create OAuth credentials in Adobe Developer Console

Create a **project** in the [Adobe Developer Console](https://developer.adobe.com/console/) that provides OAuth credentials for the Journey Optimizer API. You will need values such as **Client ID**, **Client Secret**, **Org ID**, and **Scope** when you configure the app in Exchange.

1. Sign in to the Adobe Developer Console and create a **new project**.
1. Add the **Adobe Journey Optimizer (AJO) API** to the project by clicking **[!UICONTROL Add API]** and selecting **[!UICONTROL Adobe Journey Optimizer]** from the **[!DNL Experience Cloud]** product APIs list.
1. Generate credentials in the project workspace and copy **Client ID**, **Client Secret**, **Org ID**, **Scope**, and any other values your deployment flow asks for. Store them securely for the next section.

>[!NOTE]
>
>When you install from Exchange, use the **OAuth Client ID** if both an OAuth Client ID and a Technical Account ID are shown.

## Deploy the application from Exchange

### Open the app in Manage and add an environment

1. Return to [Adobe Exchange](https://exchange.adobe.com).
1. Select **[!UICONTROL Manage]** and open **[!UICONTROL App Builder applications]** (or your organization's path to managed apps).
1. Select **Journey Optimizer for GenStudio** and confirm the app is **Approved**.
1. Under **[!UICONTROL Environments]**, choose an existing environment from the **Environments:** dropdown or select **[!UICONTROL Add Environment]** to create one.
![Application details with Approved status and Add Environment](/help/extensibility/ajo-config-002.png){width="50%"}
1. In the selected environment, select **[!UICONTROL Configuration]**.
1. On the **[!UICONTROL Configuration]** tab, find **[!UICONTROL AJO Credentials]**.
![Configuration with AJO Credentials before deployment (Draft)](/help/extensibility/ajo-config-004.png){width="80%"}
1. Enter the credentials from the Developer Console project that has the Journey Optimizer API added (for example, **[!UICONTROL AJO Client ID]**, **[!UICONTROL AJO Client Secret]**, and **[!UICONTROL AJO Token Endpoint]** and any other required fields).
1. Enter the **sandbox name in all lowercase** (for example, `prod`).
1. Click **[!UICONTROL Deploy]**. When deployment finishes, the status shows as deployed. The button text will change to **[!UICONTROL Undeploy]**.
![Deployed app with Undeploy available on the App Builder applications view](/help/extensibility/ajo-config-005.png){width="80%"}

After deployment, the Adobe Developer Console includes a new auto-generated project named **Journey Optimizer for GenStudio <Your_Environment_Name>** with AJO and Adobe Runtime APIs. This project is read-only and cannot be edited or deleted.
![Read-only auto-generated Developer Console project after deployment](/help/extensibility/ajo-auto-project.png){width="100%"}

### Update configuration

To change configuration variables for an environment, **[!UICONTROL Undeploy]** first, update values, then **[!UICONTROL Deploy]** again so changes take effect.

You can create **multiple environments** in Exchange (for example, one per sandbox). Each deployment can surface as a separate experience in GenStudio when your organization uses multiple sandboxes.

## Map permissions for the technical account

Users can see the AJO extension in GenStudio without full [!DNL Adobe Experience Platform] access. For API calls (for example, loading templates), the technical account tied to the OAuth credentials must be granted Journey Optimizer permissions in **[!DNL Adobe Experience Platform]** > **[!UICONTROL Permissions]**. The exact role names and permission sets depend on your organization.

View the extension under **[!UICONTROL Journey Administrator]** in AJO **[!UICONTROL Permissions]** > **[!UICONTROL Roles]** and add the **API credentials** from the Developer Console project, the same credentials you used when deploying from Exchange.

![API credentials assigned to the AJO Architect role in Adobe Experience Platform Permissions](/help/extensibility/ajo-map-permissions.png){width="80%"}

**See also** (Journey Optimizer access control):

* [Access control](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/access-control/access-control-landing-page)
* [Permissions in Journey Optimizer](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/access-control/permissions)
* [Get started for system administrators](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/get-started/quick-start/administrator)

## Access AJO templates in GenStudio

After deployment and permission mapping:
1. Open **[!UICONTROL Create]** in GenStudio for Performance Marketing and start an **Email** experience.
1. In **[!UICONTROL Select template]**, open the **[!UICONTROL AJO Template]** tab beside **[!UICONTROL Uploaded templates]** to browse templates from Journey Optimizer.

![Select template with AJO Template tab and template gallery](/help/extensibility/ajo-template-tab.png){width="80%"}

## Troubleshooting

### AJO Templates tab is not visible

* Confirm the values entered in Exchange **[!UICONTROL Configuration]** are correct, including **Client ID**, **Client Secret**, **Scope**, and **Sandbox**.
* Ensure the **sandbox name is lowercase** (for example, `prod`).
* When installing from Exchange, use the **Client ID** as described in [Create OAuth credentials](#create-oauth-credentials-in-adobe-developer-console).

### AJO Templates tab is visible but no templates appear

* Reload the page or open the **[!UICONTROL AJO Template]** tab again.
* In the browser **[!UICONTROL Network]** tools, inspect the **`get-templates`** request. If it returns **403 Forbidden**, the technical account is not assigned to a role or group with the required Journey Optimizer permissions. Update mappings in [!DNL Adobe Experience Platform] **[!UICONTROL Permissions]** and in AJO **[!UICONTROL Permissions]** as your organization requires.
