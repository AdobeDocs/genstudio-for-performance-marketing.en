---
title: Create an App Builder Project to extend GenStudio for Performance Marketing
description: Create an App Builder Project for your app, or add-on.
---
# Create an App Builder Project

Developers extending Adobe GenStudio for Performance Marketing's native capabilities use Adobe App Builder to create, submit, and deploy their extensible apps, or _add-ons_.

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
