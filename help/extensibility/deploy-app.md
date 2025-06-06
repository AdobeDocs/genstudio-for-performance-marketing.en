---
title: Deploy your App Builder app
description: Deploy your App Builder app, or Add-on, for GenStudio for Performance Marketing.
feature: Extensibility
exl-id: 51888ab7-7772-4ac8-838d-26db3019e9b0
---
# Deploy your app

Running your app provides a preliminary snapshot of your Add-on behavior before deploying it. This information can facilitate debugging. You can force build and deployment of a deployed your app without re-submitting it for approval.

**To run the app**:

Run the app in `https://localhost:9080`:

```bash
aio app run
```

**To deploy the app**:

1. Navigate to your Deployment workspace. For example, to navigate to the Production workspace:

   ```bash
   aio app use -w Production
   ```

1. Deploy the app:

   ```bash
   aio app deploy
   ```

**To force re-deployment**:

>[!NOTE]
>
>Forcing build and deployment overwrites your existing deployment. Thoroughly test your app in a test environment first.

   ```bash
   aio app build --force-build
   ```

   ```bash
   aio app deploy --force-deploy
   ```

**To build and deploy at the same time**: 

   ```bash
   aio app deploy --force-build --force-deploy
   ```

**To view the app**:

After deployment, you can view the app in GenStudio for Performance Marketing by adding a `query` parameter to the GenStudio for Performance Marketing URL:

`https://experience.adobe.com/?ext=https://<my-deployed-add-on>.adobeio-static.net/index.html#/@<ims-org>/genstudio/create`

If you are satisfied with your Add-on, you are ready to distribute it without the `query` parameter.

You can now [distribute your app](distribute-app.md).
