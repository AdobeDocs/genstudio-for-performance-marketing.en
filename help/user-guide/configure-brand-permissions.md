---
title: Configure an Adobe Admin Console Project for GenStudio Brands
description: Learn about configuring entitlements for GenStudio for Performance Marketing brand creators and editors.
level: Beginner
feature: Prompt, Brands Service, Personas Service, Products Service, Generative AI, Guidelines
---
# Configure an Adobe Admin Console Project for GenStudio [!DNL Brands]

GenStudio system managers by default have permissions that permit them to create and edit [!DNL Brands]. Some GenStudio for Performance Marketing content editors and collaborators might require [!DNL Brands] editing and creation permissions but no other system management entitlements. To grant content editors and collaborators these [!DNL Brand]-related entitlements, an Adobe system administrator must perform some additional configuration tasks in the [Adobe Admin Console](https://helpx.adobe.com/enterprise/using/admin-console.html#Overview).

These additional configuration steps include:

1. Create a new user group in the Adobe Admin Console.
1. Assign a GenStudio system manager product profile to the user group.
1. Create an Adobe GenStudio [!DNL Brands] project from the Console _Storage_ tab.
1. Invite the user group you just created to the [!DNL Brands] project.
1. Add users to the user group.

>[!NOTE]
>
>Only Adobe system administrators can implement enablement tasks that require Adobe Admin Console access.

Adding users and user groups are basic tasks common to all Adobe products whose entitlements are managed through the Admin Console. See [Adobe Admin Console users](https://helpx.adobe.com/enterprise/using/users.html) for an overview of user management and procedures for adding users and user groups.

## Step 1: Create a new user group in the Adobe Admin Console

**To create a new user group**:

1. Log in to the Admin Console and navigate to **[!UICONTROL Users]** > **[!UICONTROL Users Groups]**.

1. Click **[!UICONTROL New User Group]** . The _Create a new user group_ popup opens.

1. Add an informative user group name to the **[!UICONTROL User group name]** field. This name should help identify the purpose of this new group (for example, **GenStudio Brand Managers**).

1. (_Optional_). Add a description of the group and its purpose.

1. Click **[!UICONTROL Save]**.  The Admin Console opens the _New group_ popup, with the name of the group you just created.

## Step 2: Assign a GenStudio System Manager profile to the user group

Once you have created a new user group and added users, you can assign the Adobe GenStudio system managers profile to this group. The entitelments associated to the profile you assign gives all users in this group GenStudio [!DNL Brands] permissions (create, update, and delete brands).

**To assign a profile to the user group**:

1. Navigate to the newly created user group and click the _Assigned product profiles_ tab.

1. From the _Assigned product profiles_ tab, click **[!UICONTROL Assign profile]**. The _Assign products and profiles_ pop up opens.

1. Select `Adobe GenStudio` from the _Select products_ list.

1. Click **[!UICONTROL Apply]**. The _Select product profiles_ pop-up opens, displaying the product profiles associated with Adobe GenStudio.

1. Select the `Adobe GenStudio system manager`.
   
1. Click **[!UICONTROL Apply]**. The Admin Console opens the _New group_ popup, with the name of the group you just created.
   
   The _Assign products and profiles_ pop up opens, displaying the product profile for the user group you just created.

## Step 3: Create a [!DNL Brands] project from the Storage tab

A _project_ provides a storage location where select users can save assets -- in this case, [!DNL Brands] assets.

**To create a [!DNL Brands] project**:

1. Navigate to the _Storage_ tab in the Admin Console.

1. Click on **[!UICONTROL Projects]** in the side navigation. The _Projects_ tab opens.

1. Click **[!UICONTROL Create Project]**. The _New Project_ popup opens.

1. Enter `Adobe GenStudio Brands` into the project name field. Enter this project name exactly as displayed here. Do not include extra spaces or change the lettercase.

1. Click **[!UICONTROL Create]**. The  _Invite to project_ popup opens.
 
See [Manage projects](https://helpx.adobe.com/enterprise/using/projects-in-business-storage.html).

## Step 4: Invite the user group to the [!DNL Brands] project

You are now ready to add the user group you just created to the `Adobe GenStudio [!DNL Brands]` project.

**To invite the user group to the project**:

1. From the _Invite to project_ popup, add the user group you just created to this project.

1. Choose the **Can edit** permissions option.

1. Click **[!UICONTROL Invite]**.

<!-- Need info on what happens when you click Invite -->

## Step 5: Add users to the user group

To assign users permission create, edit, and publish [!DNL Brands], add them to the user group you just created.

**To add users to the user group**:

1. From the Admin Console, navigate to **[!UICONTROL Users]** > **[!UICONTROL User Groups]**.

1. Select the name of the user group you created earlier. The _Add users to this user group_ popup opens.

1. Add a new or existing user by either username or email address. Learn about managing user groups in [Manage user groups](https://helpx.adobe.com/enterprise/using/user-groups.html).

After a user is added to this group, they are granted the [!DNL Brands] create, edit, and publish permissions of Adobe GenStudio system managers. Users also receive an automated email invitation to edit the Adobe GenStudio [!DNL Brands] project.






