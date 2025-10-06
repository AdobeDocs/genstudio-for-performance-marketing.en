---
title: Deploy your App Builder App
description: Deploy your App Builder app, or Add-on, for GenStudio for Performance Marketing.
feature: Extensibility
exl-id: 51888ab7-7772-4ac8-838d-26db3019e9b0
---
# Deploy your app

Running your app offers a preliminary snapshot of your Add-on's behavior before deploying it. This can help with debugging. 

## Run the app

Run the app in `https://localhost:9080`:

```bash
aio app run
```

## Deploy the app

1. Navigate to your Deployment workspace:

   ```bash
   aio app use -w [deployment_workspace]
   ```

2. Deploy the app:

   ```bash
   aio app deploy
   ```

## Force re-deployment

You can force a build and deployment of your app without re-submitting it for approval.

>[!NOTE]
>
>Forcing a build and deployment overwrites your existing deployment. **Thoroughly test your app** in a test environment first.

   ```bash
   aio app build --force-build
   ```

   ```bash
   aio app deploy --force-deploy
   ```

## Build and deploy at the same time

   ```bash
   aio app deploy --force-build --force-deploy
   ```

## Find your new app

After deployment, you can view the new app in GenStudio for Performance Marketing.

### View with a URL

See the new app by adding a `query` parameter to the GenStudio for Performance Marketing URL:

```txt
https://experience.adobe.com/?ext=https://<my-deployed-add-on>.adobeio-static.net/index.html#/@<ims-org>/genstudio/create
```

### View in the UI

New extensions are found in different locations in the UI, depending on the type of extension you deployed. The currently available extension points are:

* Compliance extension, which includes: 
  * *prompt extension points*, which allow customers to add additional context to LLM generation, and 
  * *validation extension points*, which allow customers to validate the generated content from the LLM. Validation is often paired with Prompt extension to make sure content generated with an extended prompt is complaint with customer requirements (for example, medical drug claims, or legal)
* Digital Asset Management (DAM) extension
* Template extension
* Translation extension

#### Find prompt extensions

Prompt extenstions are found in the **Add-ons** dropdown, in the **parameters section** of a template.

![Prompt extensions](./select-prompt-ext.png){width="600" zoomable="yes"}

The add-on dialog will open, allowing you to select the additional context to add for the LLM generation.

![Prompt extension dropdown](./select-prompt-dropdown.png){width="600" zoomable="yes"}

#### Find validation extensions

Validation extensions can be found after a prompt generation, in the right sidenav displayed with the results.

![Validation extensions](./validation-ext.png){width="600" zoomable="yes"}

Run the extension you selected to validate the generated content.

![Valid Validation](./validation-valid.png){width="600" zoomable="yes"}

#### Find DAM extensions

Digital Asset Management (DAM) extensions are found when selecting content in the **parameters section** of a template. See the bottom of the **Select location** dropdown to see any add-ons.

![DAM extensions](./dam-ext.png){width="600" zoomable="yes"}

#### Find template extensions

Template extensions are found in the **External Template App** tab when selecting a template. This tab appears only when there are template apps to select.

![Template extensions](./template-ext.png){width="600" zoomable="yes"}


#### Find translation extensions

Use Translation Extension Points to bring your own translation service through a proxy instead of using GenStudio default translation.
There's no UI location for these extensions. 

If the extension is registered, the provided translation service is used. Otherwise the default GenStudio translation service is used.



If you're satisfied with your Add-on, you're ready to distribute it without the `query` parameter.

Now, you can [distribute your app](distribute-app.md).
