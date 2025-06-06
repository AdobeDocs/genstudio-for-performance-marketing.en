---
title: Create an App Builder app to extend GenStudio for Performance Marketing
description: Start building an app, or Add-on.
feature: Extensibility
exl-id: 4e757dd4-a02d-472c-bc13-6f27dffa48f2
---
# Develop an App Builder app

Developers extending GenStudio for Performance Marketing's native capabilities use [Adobe App Builder](https://developer.adobe.com/app-builder/) to create, submit, and deploy their extensible apps, or Add-ons.

>[!BEGINSHADEBOX]

**Prerequisites**:

* Node.js (version 20.x or higher)

* npm (packaged with Node.js)

* Adobe Developer command-line interface (CLI). To install: `npm install -g @adobe/aio-cli`

>[!ENDSHADEBOX] 

## App structure

GenStudio for Performance Marketing Add-ons are App Builder apps and contain the same basic components as other App Builder apps.

### Build and configuration files

Key components of App Builder apps include these build and configuration files. This list in not inclusive of all build and configuration files.

* `README.md`: Includes general information about the app.

* TS app files:
  
  * `package.json`
  * `package-lock.json`
  * `eslint`
  * `tsconfig`
  * `jest test up`

* App Builder config files: 

  * `app.config.yaml`  
  * `ext.config.yaml`: configuration file for the Add-on
  * `app.config.yaml`: configuration file for the Add-on (includes defining your app as a GenStudio for Performance Marketing Add-on)
  * `.aio`
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
 
### Source code components

* `ExtensionRegistration.tsx`: Defines the necessary APIs that the host app (GenStudio for Performance Marketing) needs to load and display the Add-on.

* `App.tsx`: Main app component that defines routing to other components.

* `AdditionalContextDialog.tsx`: Dialog component for displaying additional context Add-ons.

* `RightPanel.tsx`: Dialog component for a validation Add-on.

* `Helper` components: Includes `ClaimsChecker`.

## Create an App Builder app from an existing app

You can use an example app to jump-start creation of your Add-on. 

**To create an App Builder app from an existing app**:

1. Download an example app from the [GenStudio UIX Examples](https://github.com/adobe/genstudio-uix-examples) repository.

1. From the App Builder Project workspace on [Adobe Developer Console](https://developer.adobe.com/console/), select **[!UICONTROL Download All]** to download Project details.

1. Open your example app locally in your preferred Integrated Development Environment (IDE).

1. Authenticate with the Adobe Developer command-line interface:

   ```bash
   aio login
   ```

1. Download your JSON file, then create your app:

   ```bash
   aio app use '/path/to/your/downloaded/app-builder/project/details/config.json'
   ```

## Add custom code to your Add-on

You define your Add-on code in `AdditionalContextDialog.tsx` and `RightPanel.tsx` files. These two files define pop-up appearance and behavior when users access the Add-on.

* `AdditionalContextDialog.tsx`: Define this component if you plan to use the _Add Context_ Add-on. Users interact with this component when clicking on _Add-ons_ in the prompt drawer in [!DNL Create].

* `RightPanel.tsx`: Define this component if you plan to use the _Right Panel_ Add-on (experience validation). Users interact with this component when clicking on the validation Add-on in the right panel in a [!DNL Create] experience draft.

You are now ready to [Deploy your app](deploy-app.md)

## Best practices for app development

Maintaining your development environment can help you avoid app development and deployment errors: 

* If you are using an older version of a sample app, upgrade the dependencies by re-installing them:

   ```bash
   rm -rf node_modules package-lock.json && npm i
   ```

* Upgrade the GenStudio UIX SDK. Confirm that you are using the most recent version of the [GenStudio UIX SDK](https://github.com/adobe/genstudio-uix-sdk). Refer to the [GenStudio UIX Example repository](https://github.com/adobe/genstudio-uix-examples) to learn how to use the most recent SDK changes.
