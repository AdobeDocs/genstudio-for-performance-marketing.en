---
title: Develop and deploy your app
description: Develop and deploy your custom add-on.
---

# Develop and deploy your app
 
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

You define your add-on code in the `AdditionalContextDialog.tsx` and `RightPanel.tsx` files. These two files define pop-up appearance and behavior when users access the add-on.

* `AdditionalContextDialog.tsx`: User clicks on Add-on in the prompt drawer in [!DNL Create].

* `RightPanel.tsx`: User clicks on the validation add-on in the right panel in [!DNL Create] in an experience draft.

## Step 1: Run and deploy the app

Running your app can provide valuable debugging information. 

**To run the app**:

To run your app, enter `aio app run`.

This command runs the app in `localhost`. It does not produce significant output because this app is successfully issues. To see the app in GenStudio for Performance Marketing, you must deploy the product.

**To deploy the app**:

1. To deploy this app in production, first navigate to the deployment workspace. Enter:

   `aio app use -w Production`

1. Enter: 

   `aio app deploy`

**To force re-deployment**:

You can force build and deployment of a deployed your app without re-submitting it for approval.

Enter:

`aio app build --force-build`
`aio app deploy --force-deploy`

To build and deploy at the same time, enter:

`aio app deploy --force-build --force-deploy` 

After deploying the app, you can view it in your instance of GenStudio for Performance Marketing by adding this query parameter to the GenStudio for Performance Marketing URL:

`https://experience.adobe.com/? ext=<deployed-url>#/@my-org/genstudio/create`

## Step 2: Package the add-on

Package your add-on so that other organizations can install it. If you are creating a private add-on, skip this step and directly run and deploy your add-on.   

**To create a package**:

1. Enter this command

   `aio app pack`

1. Save the command output in a location that you can easily access when publishing the app publicly. See [Distribute your app](distribute.md).

You can now distribute your add-on. See [Distribute your app](distribute.md).
