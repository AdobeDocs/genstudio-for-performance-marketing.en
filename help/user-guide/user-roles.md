---
title: Adobe GenStudio for Performance Marketing user roles and permissions
description: Learn about GenStudio for Performance Marketing user roles and permissions.
level: Beginner
feature: Prompt, Brands Service, Personas Service, Products Service, Generative AI, Guidelines
exl-id: 33ebcf9c-e5f8-4011-b449-5f73d151f221
---
# User roles and permissions

Creating and deploying modern marketing campaigns requires collaboration among stakeholders with varying responsibilities and skill sets. _User roles_ control stakeholder access to GenStudio for Performance Marketing's many capabilities. Your assigned user role determines the tasks that you can perform using this platform. An Adobe system administrator assigns you to a role in the GenStudio product profile in the Adobe Admin Console. Your welcome email identifies your assigned role.

>[!NOTE]
>
>Before any users are provisioned into these roles, an Adobe system administrator must be designated in the Adobe Admin Console to perform one-time setup tasks. This Adobe admin role operates only in the context of the Adobe Admin Console. It has no role in the GenStudio for Performance Marketing platform interface. An Adobe system administrator who needs system manager entitlements must provision themselves as a GenStudio system manager in the Adobe Admin Console. See [Provision GenStudio for Performance Marketing](product-provisioning.md).

## Adobe system administrator vs GenStudio system manager

These user role titles might seem similar, but they identify unique roles that provide entitlements in different environments.

**Adobe system administrators** have power user privileges in the Adobe Admin Console and perform all user management tasks, such as adding or deleting users. This system administrator role provides no privileges in the GenStudio for Performance Marketing application, which explains why Adobe system admins do not require a license for GenStudio. Adobe system administrators typically use the Admin Console to add and delete user accounts from GenStudio deployments and assign or remove entitlements, or permissions, from individual users or user groups.

**GenStudio system managers** are power users within GenStudio for Performance Marketing but have no permission to perform tasks in the Adobe Admin Console. This system manager role requires a GenStudio product license and it corresponds to a Power User in the [Adobe GenStudio for Performance Marketing Product description](https://helpx.adobe.com/legal/product-descriptions/adobe-genstudio-for-performance-marketing---product-description.html). GenStudio system managers have full entitlement to GenStudio for Performance Marketing capabilities, including [!DNL Brands], [!DNL Persona], and [!DNL Product] creation, deletion, updating, and publishing. [Adobe GenStudio for Performance Marketing Product Description](https://helpx.adobe.com/legal/product-descriptions/adobe-genstudio-for-performance-marketing---product-description.html) explains how GenStudio user roles relate to product licenses.

See [Administrative roles](https://helpx.adobe.com/enterprise/using/admin-roles.html#enterprise) in _Enterprise and Teams administration guide_.

## Entitlements

_Entitlements_ grant permission to perform specific tasks and access protected resources. Entitlements, or permissions, are defined in the user role within the product profile, and users receive these entitlements when assigned to that role.

>[!IMPORTANT]
>
>Do not add new, or edit or delete, existing product profiles. Altering the default product profiles can seriously disrupt your GenStudio for Performance Marketing deployment.

## User roles

Three types of GenStudio for Performance Marketing user roles support this diversity of organizational roles. Entitlements are tailored to each of these user types and support each user's responsibilities in the marketing organization. These three user role types are:

* **GenStudio editors** use GenStudio for Performance Marketing's generative AI capabilities to create marketing campaign assets, request content review and approval, and publish approved drafts of this content. All GenStudio for Performance Marketing users can access and use an asset once its editor has saved it to [!DNL Content]. GenStudio editors are power users in GenStudio for Performance Marketing.

* **GenStudio collaborators** are the widest range of GenStudio for Performance Marketing users. Collaborators can view and approve content and are an essential part of the workflow that ensures that the content you generate matches your organization's needs and standards. GenStudio collaborators are _collaborator users_ in GenStudio for Performance Marketing.

* **GenStudio system managers** have the broadest set of entitlements, or permissions, within GenStudio for Performance Marketing. System managers perform the essential onboarding task of establishing the fundamental guardrails for campaign asset creation and deployment. System managers implement these guardrails by uploading brand and organizational-specific information such as [brand guidelines](./guidelines/overview.md). System managers have permission to create and publish [!DNL Brands], but have no user administration privileges. GenStudio system managers are power users in GenStudio for Performance Marketing.

### GenStudio editors

_Editors_, or content creators, have the core permissions needed to create GenStudio for Performance Marketing [!DNL Brands], [!DNL Campaigns], and [!DNL Content] assets. These power users can also edit and delete assets they have created. GenStudio for Performance Marketing supports the quick creation of hundreds of pieces of content. These users can generate content fragments or whole experiences that orchestrate discrete pieces of approved content to meet the needs of specific marketing campaigns.

Editors interact with GenStudio for Performance Marketing generative AI technologies through _prompting_. The prompt drawer in the Canvas provides tools to place prompts in the context of a specific campaign's guidelines. As a result, the quality and success of generated content partially depend on the quality of the brand guidelines your organization has uploaded and the specificity of your prompt. See [Write effective prompts](effective-prompts.md).

The following table displays the default editor permissions:

| Feature | Create  | Update | Delete | View |
|-----------|----------------|----------------|----------------|----------------|
|   [!DNL Brands]| no  | no | no |  yes |
|   [!DNL Campaigns] | yes    |   yes      |  yes       |    yes       |
|   [!DNL Content] |     yes  |   yes     |    yes   |   yes      |
|   [!DNL Create] |     yes  |   yes     |    yes   |   yes      |
|   [!DNL Insights] |  can configure connectors only  |    |     |   yes  |
|   [!DNL Personas] | yes    |   yes*      |  yes*       |    yes       |
|   [!DNL Products] | yes    |   yes*      |  yes*       |    yes       |
|   [!DNL Reviews and approvals]  |   yes     |  yes   |    yes     |    yes     |
|   [!DNL Templates]| no  | no | no |  yes |

Editors can edit and delete [!DNL Personas] and [!DNL Products] that they have created.

GenStudio system managers can give editors permission to edit and delete a [!DNL Brand].

### GenStudio collaborators

_Collaborators_ can view assets in GenStudio for Performance Marketing but not create, edit, or delete these assets. Collaborators see a "*You don't have access to this content*" message when they attempt to access [[!DNL Create]](/help/user-guide/create/overview.md).

Collaborators include stakeholders who are essential to the success of the review and approval process for content but who do not need to create or directly edit content. Legal experts and managers of creatives are examples of potential collaborators. GenStudio for Performance Marketing collaborators might have permission to create and view assets in other Creative Cloud products.

The following table displays the default collaborator permissions:

| Feature | Create  | Update | Delete | View |
|-----------|----------------|----------------|----------------|----------------|
|   [!DNL Brands]| no  | no | no |  yes |
|   [!DNL Campaigns] | no    |   no      |  no       |    yes       |
|   [!DNL Content] |     no  |   no     |    no   |   yes      |
|   [!DNL Create] |     no  |   no     |    no   |   yes      |
|   [!DNL Insights] |    no |  no  |   no  |   yes  |
|   [!DNL Personas] | no    |   no      |  no       |    yes       |
|   [!DNL Products] | no    |   no      |  no       |    yes       |
|   [!DNL Reviews and approvals] |   no     |   no  |  no       |   yes      |
|   [!DNL Templates]| no  | no | no |  yes |

### GenStudio system managers

_GenStudio system managers_ have the most powerful set of permissions within GenStudio for Performance Marketing. These power users perform the essential onboarding task of establishing the fundamental guardrails for campaign asset creation and deployment. System managers implement these guardrails by uploading brand and organizational-specific information such as [brand guidelines](./guidelines/overview.md). System managers have permission to create and publish [!DNL Brands], but have no user administration privileges.

The following table displays the default system manager permissions:

| Feature | Create  | Update | Delete | View |
|-----------|----------------|----------------|----------------|----------------|
|   [!DNL Brands]| yes  | yes | yes |  yes |
|   [!DNL Campaigns] | yes    |   yes      |  yes       |    yes       |
|   [!DNL Content] |     yes  |   yes     |    yes   |   yes      |
|   [!DNL Insights] |  yes   |  yes  |   yes |  yes   |
|   [!DNL Personas] | yes    |   yes      |  yes       |    yes       |
|   [!DNL Products]  | yes    |   yes      |  yes       |    yes       |
|   [!DNL Reviews and approvals] |  yes      | yes    |     yes    |   yes      |
|   [!DNL Templates]| yes  | yes | yes |  yes |

System managers can also upload templates.

See [Get started with Adobe GenStudio for Performance Marketing](get-started.md) for an overview of preliminary set-up tasks.
