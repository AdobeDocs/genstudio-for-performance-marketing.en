---
title: Distribute your app
description: Distribute your extensible applications.
---
# Distribute your app

_Distribution_ of an add-on in the Adobe ecosystem is the process of making your add-on available as an application on [Adobe Exchange](https://exchange.adobe.com/) for either public or private distribution.

Your distribution workflow depends on whether your add-on is intended for public or private distribution. Private distribution restricts the deployment of your add-on to the organization identified by the IMS org for which you developed your add-on. Public distribution makes the add-on available as an app on the Adobe Exchange.

The application distribution process is described extensively in [App Builder app](https://developer.adobe.com/developer-distribution/experience-cloud/docs/guides/submission/app_builder_submission/).

>[!NOTE]
>
>Create an App Builder Project and App Builder App before creating a listing for public distribution. Public distribution requires both a deployed app and a packaged version, but private distribution requires only a deployed app.

## Private distribution

Before distributing your private add-on, confirm that your App Builder app is deployed in an App Builder Project.

You also need: 

* Developer permissions in the org from which you submit the app for approval

* System Administrator permissions in the org to approve the app

**To distribute your app privately**:

1. From [Adobe Developer Console](https://developer.adobe.com/console/), select the org and Project where the app is deployed.

1. Select **[!UICONTROL Approval]** from the _Workspace overview_ area. The _App Approval_ pane opens. 

1. In the _App Submissions Details_ area, add informative details about your add-on. Details include app name, description, and contact email. 

1. When you have completed all fields, click **[!UICONTROL Submit]**. 

1. Log in to [Adobe Exchange](exchange.adobe.com) using the same Adobe ID that you used to log into Developer Console. If you do not have system administrator permissions in this org, request approval from an org system administrator. 

1. Select **[!UICONTROL Manage]** > **[!UICONTROL App Builder applications]** to access a request to review the app. 

1. After reviewing the app, select **[!UICONTROL Approve]**. Optionally, add notes.

Your add-on is now visible in your deployment of GenStudio for Performance Marketing.

## Public distribution

Public distribution requires more steps than distributing your add-on privately. 

* **Create a listing on Adobe Developer Distribution for your app**. [Adobe Developer Distribution](https://developer.adobe.com/developer-distribution/) is a self-service submission portal for developers to publish their listings on Adobe Exchange. Creating a listing includes assigning informative public details about your add-on, including name, payment, and support information.

* **Submit the application listing for approval**. After you have added listing details for your application, you can upload the package and submit the listing for approval. If you change your application listing details after submitting the application for review, you must re-submit for approval.

Once your application has been approved, users outside your organization can download and install your add-on.

## Create a listing

**To create a listing**

1. From [Adobe Developer Console](https://developer-stage.adobe.com/console), select your add-on name in the _Product & services_ area.

1. Click **[!UICONTROL Create a new listing]**. The _New listing_ page for your add-on opens.

1. In the _Application information_ area, enter informative details about your application. Details include the public name of your application, descriptive text, and payment and support information.

1. Add a new version number for your application.

Once you have completed adding relevant details, you can upload your add-on package and submit it for approval.

## Submit the add-on for approval
 
1. From the _New listing_ page, upload an `app.zip` file of the packaged AIO code to the listing. See Package the AIO app.

1. Click **[!UICONTROL Preview and submit]**. The console displays either a success message or an informative message that identifies needed action.

After an Adobe administrator reviews and approves your add-on, the app is available for [installation](install.md).
