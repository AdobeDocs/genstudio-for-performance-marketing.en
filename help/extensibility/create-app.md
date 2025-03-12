---
title: Create an App Builder app to extend GenStudio for Performance Marketing
description: Start building an app, or add-on.
---
# Create and develop an App Builder app

Developers extending Adobe GenStudio for Performance Marketing's native capabilities use Adobe App Builder to create, submit, and deploy their extensible apps, or add-ons.

## App Builder app structure

Genstudio for Performance Marketing add-ons are App Builder apps. App Builder apps and consequently, add-ons, contain the same basic components.

### Build and configuration files

* `README.md`: Includes general information about the app.

* TS app files: Includes `package.json`, `package-lock.json`, `eslint`, `tsconfig`, `jest test up`.

* App Builder config files: 

  * `app.config.yaml`, `ext.config.yaml`, `.aio`, `.env`. (Do not commit the `.env` file to source control.)
  * `ext.config.yaml`: configuration file for the add-on
  * `app.config.yaml`: configuration file for the add-on (includes defining your app as a Genstudio for Performance Marketing add-on)

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

* `ExtensionRegistration.tsx`: Defines the necessary APIs that the host app (Genstudio for Performance Marketing) loads and shows the add-on.

* `App.tsx`: Main app component that defines routing to other components.

* `AdditionalContextDialog.tsx`: Dialog component for displaying additional context add-ons.

* `RightPanel.tsx`: Dialog component for a validation add-on.

* `Helper` components: Include `ClaimsChecker` and `Spinner`.

## Step 1: Create an App Builder app

You can use an example app to jump-start your add-on creation. 

**To create an App Builder app from an existing app**

1. Download an example app from the [GenStudio UIX Examples](https://github.com/adobe/genstudio-uix-examples) repository.

1. From the App Builder Project workspace on Developer Console, select **[!UICONTROL Download All]** to download Project details. Alternatively, navigate to 

   https://github.com/adobe/aio-cli?tab=readme-ov-file#aio-console-workspace-download-destination and download workspace details:

  `aio console workspace download [DESTINATION]`

1. Open your example app locally in your preferred IDE.

1. Authenticate with the Adobe Developer command-line interface.

  `aio login` 

1. Create your app with the downloaded JSON: 

  `aio app '/path/to/your/downloaded/app-builder/project/details/config.json'`

  ## Prerequisites
 
* Node.js (version 20.x or higher)

* npm (packaged with Node.js)

* Adobe Developer command-line interface (CLI). To install, enter `npm install -g @adobe/aio-cli`
 
## Create a new App Builder App from a reference app

**To create a new app from a reference app**:

1. Clone the repository that contains your reference app.

1. Authenticate with the Adobe Developer command-line interface. Enter:

   `aio login` 

1. Navigate to the environment of the App Builder Project in which you want to deploy your app. Enter:

   `aio app use <path-to-downloaded-project-details>`

1. Install dependencies. Enter:

   `npm install`

You are now ready to add your custom code.

## Guidelines on writing add-on code

You define your add-on code in either or both `AdditionalContextDialog.tsx` and `RightPanel.tsx` files. These two files define pop-up appearance and behavior when users access the add-on.

* `AdditionalContextDialog.tsx`: User clicks on Add-on in the prompt drawer in [!DNL Create]. Define this component if you plan to use the Add Context add-on.

* `RightPanel.tsx`: User clicks on the validation add-on in the right panel in [!DNL Create] in an experience draft. Define this component if you plan to use the Right Panel (experience validation) Add-on.

You are now ready to [Deploy your app](develop-deploy.md).
