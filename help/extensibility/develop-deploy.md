---
title: Develop and deploy your app
description: Develop and deploy your custom extension.
---

# Develop and deploy your app
 
## Prerequisites
 
* Node.js (version 20.x or higher)

* npm (packaged with Node.js)

* Adobe I/O CLI. To install, enter `npm install -g @adobe/aio-cli`
 
## Create a new App Builder App from a reference app

**To create a new app from a reference app**:

1. Clone the repository that contains your reference app.

1. Authenticate with Adobe I/O. Enter:

   `aio login` 

1. Navigate to the environment of the App Builder Project you want to deploy your app to. Enter:

   `aio app use <path-to-downloaded-project-details>`

1. Install dependencies. Enter:

   `npm install`

You are now ready to add your custom code.

## Guidelines on writing extension code

You define your extension code in the `AdditionalContextDialog.tsx` and `RightPanel.tsx` files. Use these two files to define the appearance and behavior of the dialog that is triggered by the specified action.

* `AdditionalContextDialog.tsx`: User clicks on the Add-On extension in the prompt drawer in [!DNL Create].

* `RightPanel.tsx`: User clicks on the validation extension in the right panel in [!DNL Create] in an experience draft.

## Step 1: Run and deploy the app

Running your app can provide valuable debugging information. 

**To run the app**:

To run your app, enter `aio app run`.

This command runs the app in `localhost`. It does not produce significant output because this app is successfully issues. To see the your app in GenStudio for Performance Marketing, you must deploy the product.

**To deploy the app**:

1. To deploy in this app in production, first enter this command to change to the workspace you want to deploy in:

   `aio app use -w Production`

1. Enter: 

   `aio app deploy`

add sample output

**To force re-deployment**:

You can force build and deployment of a deployed your app without re-submitting it for approval.

Enter:

`aio app build --force-build`
`aio app deploy --force-deploy`

After deploying the app, you can view it in your instance of GenStudio for Performance Marketing by adding this query parameter to the GenStudio for Performance Marketing URL:

`https://experience.adobe.com/? ext=<deployed-url>#/@my-org/genstudio/create`

## Step 2: Package your extension

Package your extension so that other organizations can install it. If this is a private extension, you can skip this step and directly run and deploy your extension.   

**To create a package**:

1. Enter this command

   `aio app pack`

1. Save the command output in a location that you can easily access when publishing the app publicly. See [Distribute your extension](distribute.md).

You can now distribute your app. See [Distribute your extension](distribute.md).
