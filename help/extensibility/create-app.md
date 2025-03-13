---
title: Create an App Builder app to extend GenStudio for Performance Marketing
description: Start building an app, or add-on.
---
# Create and develop an App Builder app

Developers extending Adobe GenStudio for Performance Marketing's native capabilities use [Adobe App Builder](https://developer.adobe.com/app-builder/) to create, submit, and deploy their extensible apps, or add-ons.

## App structure

Genstudio for Performance Marketing add-ons are App Builder apps containing the same basic components.

### Build and configuration files

App Builder apps contain these build and configuration files:

* `README.md`: Includes general information about the app.

* TS app files:
  
  * `package.json`
  * `package-lock.json`
  * `eslint`
  * `tsconfig`
  * `jest test up`

* App Builder config files: 

  * `app.config.yaml`,  
  * `ext.config.yaml`: configuration file for the add-on
  * `app.config.yaml`: configuration file for the add-on (includes defining your app as a Genstudio for Performance Marketing add-on)
  *  `.aio`
  * `.env`: Do not commit the `.env` file to source control

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

* `ExtensionRegistration.tsx`: Defines the necessary APIs that the host app (Genstudio for Performance Marketing) loads and displays the add-on.

* `App.tsx`: Main app component that defines routing to other components.

* `AdditionalContextDialog.tsx`: Dialog component for displaying additional context add-ons.

* `RightPanel.tsx`: Dialog component for a validation add-on.

* `Helper` components: Include `ClaimsChecker` and `Spinner`.

## Prerequisites
 
* Node.js (version 20.x or higher)

* npm (packaged with Node.js)

* Adobe Developer command-line interface (CLI). To install, enter `npm install -g @adobe/aio-cli`

## Step 1: Create an App Builder app

You can use an example app to jump-start creation of your add-on. 

**To create an App Builder app from an existing app**:

1. Download an example app from the [GenStudio UIX Examples](https://github.com/adobe/genstudio-uix-examples) repository.

1. From the App Builder Project workspace on [Adobe Developer Console](https://developer.adobe.com/console/), select **[!UICONTROL Download All]** to download Project details. Alternatively, [download workspace details](https://github.com/adobe/aio-cli?tab=readme-ov-file#aio-console-workspace-download-destination).

  `aio console workspace download [DESTINATION]`

1. Open your example app locally in your preferred Integrated Development Environment (IDE).

1. Authenticate with the Adobe Developer command-line interface:

  `aio login` 

1. Create your app with the downloaded JSON: 

  `aio app '/path/to/your/downloaded/app-builder/project/details/config.json'`

## Create a new App Builder App from an existing app

**To create a new app from an existing app**:

1. Clone the repository that contains your existing app.

1. Authenticate with the Adobe Developer command-line interface:

   `aio login` 

1. Navigate to the environment of the App Builder Project in which you want to deploy your app:

   `aio app use <path-to-downloaded-project-details>`

1. Install dependencies:

   `npm install`

You are now ready to add your custom code.

## Add custom code to your add-on

You define your add-on code in `AdditionalContextDialog.tsx` and `RightPanel.tsx` files. These two files define pop-up appearance and behavior when users access the add-on.

* `AdditionalContextDialog.tsx`: User clicks on Add-on in the prompt drawer in [!DNL Create]. Define this component if you plan to use the Add Context add-on.

* `RightPanel.tsx`: User clicks on the validation add-on in the right panel in [!DNL Create] in an experience draft. Define this component if you plan to use the Right Panel (experience validation) Add-on.

You are now ready to [Deploy your app](develop-deploy.md).

## Best practices for app development

Maintaining your development environment can help you avoid app development and deployment errors: 

* If you are using an older version of a sample app, upgrade dependencies by re-installing them:

```
rm -rf node_modules package-lock.json && npm i
``` 
* Upgrade the GenStudio UIX SDK. Confirm that you are using the most recent version of the [GenStudio UIX SDK](https://github.com/adobe/genstudio-uix-sdk). Refer to the [Genstudio UIX Example repository](https://github.com/adobe/genstudio-uix-examples) to learn how to use the most recent SDK changes.
