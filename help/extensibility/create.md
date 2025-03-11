---
title: Create an App Builder app to extend GenStudio for Performance Marketing
description: Start building extensible applications for GenStudio for Performance Marketing.
---
# Create an App builder Project and and App Builder app

Developers extending Adobe GenStudio for Performance Marketing's native capabilities use Adobe App Builder to create, submit, and deploy their extensible apps.

## App Builder app structure

Genstudio for Performance Marketing extensible applications are App Builder apps. App Builder apps and consequently, Genstudio for Performance Marketing apps, contain the same basic components.

### Build and configuration files

* `README.md`: Includes general information about the app.

* TS app files: Includes `package.json`, `package-lock.json`, `eslint`, `tsconfig`, `jest test up`.

* App Builder config files: 

  * `app.config.yaml`, `ext.config.yaml`, `.aio`, `.env`. (Do not commit the `.env` file to source control.)
  * `ext.config.yaml`: config file for the extension
  * `app.config.yaml`: config file for the app (includes defining your app as a Genstudio for Performance Marketing extension)

### Source code

```
- src/
    - genstudiopem/
        - web-src/
            - src/
                - components/
                - utils/
                - Constants.ts
                - index.tsx
                - index.css
                - utils.ts
        - index.html
```
 
### Additional components

* `ExtensionRegistration.tsx`: Defines the necessary APIs that the host app (Genstudio for Performance Marketing) loads and shows the extension.

* `App.tsx`: Main app component that defines routing to other components.

* `AdditionalContextDialog.tsx`: Dialog component for displaying additional context add-ons.

* `RightPanel.tsx`: Dialog component for a validation extension.

* `Helper` components: Include `ClaimsChecker` and `Spinner`.

## Step 1: Create an App Builder Project

Creating your Project relies on access to App Builder and the [Adobe Developer Console](https://developer.adobe.com/developer-console/). See [Create a new Project on Developer Console](https://developer.adobe.com/app-builder/docs/getting_started/first_app/#2-create-a-new-project-on-developer-console) for a more expansive discussion. 

### Prerequisites

* Provision GenStudio for Performance Marketing in the IMS org in which you are developing the custom extension. 

* Install AIO CLI  globally. Use this command: ` npm install -g @adobe/aio-cli`

* Install Nodejs v20

**To create a new Project**:

1. Log in to [Adobe Developer Console](https://developer.adobe.com/developer-console/).

1. Use the IMS org switcher on the Console landing page upper right corner to select your IMS organization.

1. From _Quick Start_, click **[!UICONTROL Create new project]**, then select **[!UICONTROL Create project from template]**. The _Create a New Project from Template_ panel opens. 

   If you do not see the **[!UICONTROL Create project from template]** option, confirm that you have selected the correct IMS org. If the org is correct, you do not yet have access to App Builder. Confirm that you have followed the process in How to Get Access to App Builder.

## Step 2: Create an App Builder app

You can use a sample extension to jump-start your extension creation. See the [GenStudio UIX Examples](https://git.corp.adobe.com/GenStudio/genstudio-uix-examples) repository to view and select example extensions.

**To create an App Builder app from an existing app**

1. Download a sample extension from the [GenStudio UIX Examples](https://git.corp.adobe.com/GenStudio/genstudio-uix-examples) repository.

1. From the AIO environment of your App Builder project, select **[!UICONTROL Download All]** to download your project details.

1. Open your sample extension locally in your preferred IDE.

1. Run this command with the downloaded JSON: 

   `aio app use '/Users/your_name/Downloads/206CornsilkCrow-257324-Production.json'`

You are now ready to [develop and deploy your app](develop-deploy.md).
