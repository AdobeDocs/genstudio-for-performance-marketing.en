---
title: Provisioning the Adobe GenStudio for Performance Marketing product
description: Learn about provisioning the GenStudio for Performance Marketing product.
level: Beginner
feature: Prompt, Brands Service, Personas Service, Products Service, Generative AI, Guidelines
---

# Provisioning the Adobe GenStudio for Performance Marketing product and users

Creating and deploying modern marketing campaigns requires collaboration among stakeholders with varying responsibilities and skill sets. _User roles_ control stakeholder access to Adobe GenStudio for Performance Marketing's many capabilities. Your assigned user role determines the tasks that you can perform within the product. An [Adobe system administrator](https://helpx.adobe.com/enterprise/using/admin-roles.html) assigns you to a role in the GenStudio product profile in the Adobe Admin Console (adminconsole.adobe.com). Your welcome email identifies your assigned role.

GenStudio product profiles and user roles are managed through the Adobe Admin Console. This console is the central location for managing entitlements for licensed Adobe products across organizations, including user roles and licenses. The GenStudio product profile additionally defines rules and user profiles that are unique to brand and campaign creation and management within GenStudio for Performance Marketing.

>[!NOTE]
>Before any users are provisioned into these roles, an Adobe system administrator must be designated in the Adobe Admin Console to perform one-time setup tasks plus handle ongoing user account management tasks. This Adobe admin role operates only in the context of the Adobe Admin Console. It has no role in the GenStudio for Performance Marketing platform interface. An Adobe system administrator who needs system manager entitlements in GenStudio must provision themselves as a GenStudio system manager in the Adobe Admin Console. For more information about administrative roles in the Adobe Admin Console, see [Administrative roles](https://helpx.adobe.com/enterprise/using/admin-roles.html).

## Overview

The designated Adobe system administrator enables the GenStudio for Performance Marketing product for their organization. This basic product enablement includes the initial provisioning, or onboarding, of users into the organization's GenStudio instance and assignment of user roles to individual organization members.

An _Adobe IMS org_ defines the entitlements of a group of users to one or more Adobe products or integrations. each user of an Adobe product is assigned an organization ID for that product, and this ID is an essential component of Adobe product authentication protocols. Adobe system admins can log into the [Adobe Admin Console](https://helpx.adobe.com/enterprise/using/admin-console.html) and view their organization ID in the URL.

### About the Adobe Admin Console

The Adobe Admin Console provides a central location from which admin users can view and manage users of all Adobe products, including GenStudio for Performance Marketing. See [Accessing the Admin Console](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/onboarding/journey/admin-console) for an introduction to Adobe IDs, Console features, and how to review your admin user privileges.

Once one or more privileged admin users are onboarded for GenStudio for Performance Marketing, they can log into the Admin Console and set up the hierarchy of access privileges that best suits your organization's needs for asset protection and user empowerment. These admin users can delegate select administrative tasks to other users while still maintaining control over the larger structure of organizational entitlements.

Administrators are onboarded to GenStudio for Performance Marketing the same way that admins are onboarded for other Adobe products. Enterprise customers must be assigned the System Administrator or Developer role in the Adobe Admin Console to access the product profile and assign users in the organization privileges within GenStudio for Performance Marketing.

### About Adobe IMS orgs

All users of GenStudio for Performance Marketing must belong to the Adobe IMS organization where GenStudio for Performance Marketing is provisioned. The product has a unique IMS organization that is defined in the GenStudio product profile, and user of the platform must belong to this IMS org.

## Provision GenStudio for Performance Marketing

* Access the GenStudio product profile in the Adobe Admin Console

* Provision users

Only Adobe system admins can carry out these enablement tasks, which occur in the Adobe Admin Console.

### Access the GenStudio product profile in the Adobe Admin Console

If you have access to multiple Adobe organizations, ensure that you log into the correct organization.

**To access the GenStudio product profile**

1. Click the **Get started** link in your welcome email to navigate to the [Adobe Admin Console](https://helpx.adobe.com/enterprise/using/admin-console.html#Overview).

1. Log in to the Admin Console using your Adobe ID.

   Upon successful login, you see the _Overview_ tab of the Adobe Admin Console.

1. Navigate to the _Products_ tab. This tab displays all the Adobe products your organization has purchased.

1. Select **[!UICONTROL GenStudio]** from the list of products. The Console displays the GenStudio product profile, which displays key information about the product licenses your organization has purchased. It also provides options to manage these licenses.

You are now ready to assign licenses to, or provision, users to GenStudio for Performance Marketing. If you have logged into the wrong organization, switch to the correct organixation before trying to assign entitlements to users. To change your organization, click the organization name from the top right corner and choose the **GenStudio** organization.

### Provision users

Provisioning users in the Admin Console is the process of assigning product licenses to users. You can provision users to your GenStudio for Performance Marketing organization in the same way you provision users to other Adobe products. You can add users manually or import users in bulk.

>[!NOTE]
>If you are going to perform tasks in GenStudio that require GenStudio system management permissions, make sure to add yourself as a GenStudio system manager.

**Prerequisites**:

Prepare for provisioning by first identifying this basic information about the users you want to add:

* First and last name
* Corporate email address
* Types of entitlements you want the user to have within GenStudio for Performance Marketing. See [Adobe GenStudio for Performance Marketing user roles](user-roles.md) to better understand the three available user roles.

**To manually assign users to your GenStudio organization**

1. From the GenStudio product profile, click the **[!UICONTROL Assign Users]** button.

   The Console displays the _Add user_ dialog, which you can use from which you can search for and select individual users.

1. Select the name of the user you want to add.

1. Select **[!UICONTROL Save]**. The user is added and displayed in the _Users_ list.

See [Manage user individually](https://helpx.adobe.com/enterprise/using/manage-users-individually.html#add-users) for complete details on assigning entitlements to users individually.

**To add users by importing a CSV file**

You can upload a CSV file (a comma-separated or semi-colon-separated list) to add multiple users to your organization.

1. Select **[!UICONTROL Add Users by CSV]** on the Adobe Admin Console _Users_ tab.

1. Select **[!UICONTROL Download CSV template]** and choose **[!UICONTROL Current users]** or **[!UICONTROL Standard template]**.

See [Manage multiple users/ bulk CSV upload](https://helpx.adobe.com/enterprise/using/bulk-upload-users.html) for complete details on importing multiple users by CSV file.























