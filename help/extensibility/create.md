---
title: Create an App Builder Project to extend GenStudio for Performance Marketing
description: Create an App Builder Project for your app, or add-on.
---
# Create an App Builder Project

Developers extending Adobe GenStudio for Performance Marketing's native capabilities use Adobe App Builder to create, submit, and deploy their extensible apps, or _add-ons_.

## App Builder app structure

Genstudio for Performance Marketing add-ons are App Builder apps. App Builder apps and add-ons contain the same basic components.

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

## Step 1: Create an App Builder Project

Creating your Project relies on access to App Builder and the [Adobe Developer Console](https://developer.adobe.com/developer-console/). See [Create a new Project on Developer Console](https://developer.adobe.com/app-builder/docs/getting_started/first_app/#2-create-a-new-project-on-developer-console) for a more expansive discussion. 

### Prerequisites

* Provision GenStudio for Performance Marketing in the IMS org in which you are developing the custom add-on. 

* Install the App Builder command-line interface globally. Use this command: ` npm install -g @adobe/aio-cli`

* Install Nodejs (version 20 or higher)

**To create a new Project**:

1. Log in to [Adobe Developer Console](https://developer.adobe.com/developer-console/).

1. Use the IMS org switcher on the Console landing page upper right corner to select your IMS organization.

1. From _Quick Start_, click **[!UICONTROL Create new project]**, then select **[!UICONTROL Create project from template]**. The _Create a New Project from Template_ panel opens. 

If you do not see the **[!UICONTROL Create project from template]** option, confirm that you have selected the correct IMS org. If the org is correct, you do not yet have access to App Builder. Confirm that you have followed the process in How to Get Access to App Builder.

You are now ready to [create and develop your app](create-app.md).
