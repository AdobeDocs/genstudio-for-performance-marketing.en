---
title: Deploy your App Builder app
description: Deploy your App Builder app, or Add-on, for GenStudio for Performance Marketing.
---

# Deploy your app
 
Running your app can provide valuable information about your app before deploying it. Running provides a preliminary snapshot of how your Add-on works before deploying it. This view can provide valuable information for debugging. 

You can force build and deployment of a deployed your app without re-submitting it for approval.

>[!NOTE]
>
>Forcing build and deployment overwrites your existing deployment. Thoroughly test your app in a test environment first.

**To run the app**:

This command runs the app in `https://localhost:9080`:

`aio app run`. 

**To deploy the app**:

1. To deploy this app, first navigate to the deployment workspace. For example, to navigate to the Production workspace:

   `aio app use -w Production`

1. Deploy the app:

   `aio app deploy`

**To force re-deployment**:

`aio app build --force-build` 

`aio app deploy --force-deploy`

To build and deploy at the same time: 

`aio app deploy --force-build --force-deploy`

**To view the app**:

After deployment, you can view the app in GenStudio for Performance Marketing by adding a `query` parameter to the GenStudio for Performance Marketing URL:

`https://experience.adobe.com/?ext=https://<my-deployed-add-on>.adobeio-static.net/index.html#/@<ims-org>/genstudio/create`

If you are satisfied with your Add-on, you are ready to distribute it without the `query` parameter.

You can now [distribute your app](distribute-app.md)
