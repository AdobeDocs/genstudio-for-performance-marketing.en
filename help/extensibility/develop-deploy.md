---
title: Deploy your App Builder app
description: Deploy your App Builder app, or add-on, for GenStudio for Performance Marketing.
---

# Deploy your app
 

## Step 1: Run and deploy the app

Running your app can provide valuable debugging information. 

**To run the app**, enter `aio app run`. This command runs the app in `https://localhost:9080`.

**To deploy the app**:

1. To deploy this app, first navigate to the deployment workspace. For example, to navigate to the Production workspace:

   `aio app use -w Production`

1. Deploy the app.

   `aio app deploy`

**To force re-deployment**:

>[!NOTE]
>
>Forcing build and deployment overwrites your existing deployment. Thoroughly test your app in a test environment first.

You can force build and deployment of a deployed your app without re-submitting it for approval.

Enter: 

`aio app build --force-build` 

`aio app deploy --force-deploy`

To build and deploy at the same time: 

`aio app deploy --force-build --force-deploy`

After deploying the app, you can view it in GenStudio for Performance Marketing by adding a `query` parameter to the GenStudio for Performance Marketing URL. If you are satisfied with your Add-on, you are ready to distribute it without the `query` parameter.

## Step 2: Package the add-on

Package your add-on so that other organizations can install it. If you are creating a private add-on, skip this step and directly distribute the add-on after deployment.   

**To create a package**:

1. Create a package.

   `aio app pack`

1. Save the command output in a location that you can easily access when publishing the app publicly.

You can now [distribute your app](distribute.md).
