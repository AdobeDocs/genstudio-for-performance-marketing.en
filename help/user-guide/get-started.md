---
title: Get started with Adobe GenStudio for Performance Marketing
description: Learn how to set up your GenStudio for Performance Marketing to generate new brand-aligned marketing content.
level: Beginner
feature: Prompt, Brands Service, Personas Service, Products Service, Generative AI, Guidelines
exl-id: bcb03198-bbcb-45ae-af01-25c1e834b563
---
# Get started with Adobe GenStudio for Performance Marketing

Adobe GenStudio for Performance Marketing is a comprehensive platform for creating, evaluating, and managing marketing experiences that reflect and adhere to your brand identity.

Stakeholder access to its many capabilities is controlled by assigned _user roles_. Your assigned user role determines the tasks that you can perform within GenStudio for Performance Marketing. An Adobe system administrator assigns your permissions in the GenStudio for Performance Marketing product profile in the Adobe Admin Console. Your welcome email identifies your assigned role.

If you are new to generative AI-based tools or are simply curious about GenStudio for Performance Marketing core principles, see [Concepts](concepts.md) and [Write effective prompts](effective-prompts.md).

## User roles

Creating and deploying modern marketing campaigns requires collaboration among stakeholders with varying responsibilities and skill sets.

Three types of GenStudio for Performance Marketing user roles support this diversity of organizational roles. Permissions are tailored to each of these user types and support each user's responsibilities in the marketing organization.

**The three user role types are**:

* **Editors** use GenStudio for Performance Marketing generative AI capabilities to create marketing campaign assets, request content review and approval, and publish approved drafts of this content. All GenStudio for Performance Marketing users can access and use an asset once its creator has saved it to Content.

* **Collaborators** are the widest range of GenStudio for Performance Marketing users. Collaborators can view and approve content and are an essential part of the workflow that ensures that the content you generate matches your organization's needs and standards.

* **System managers** have the broadest set of permissions within GenStudio for Performance Marketing. System managers perform the essential onboarding task of establishing the fundamental guardrails for campaign asset creation and deployment. System managers implement these guardrails by uploading brand and organizational-specific information such as [brand guidelines](/help/user-guide/guidelines/overview.md). GenStudio for Performance Marketing system managers have permission to create and publish brands, but have no user administration privileges.

>[!NOTE]
>Before any users are provisioned into these roles, an Adobe system administrator must be designated in the Adobe Admin Console to perform one-time setup tasks. This Adobe admin role operates only in the context of the Adobe Admin Console. It has no role in the GenStudio for Performance Marketing platform interface.

### GenStudio for Performance Marketing editors

**Editors** have the core permissions needed to create GenStudio for Performance Marketing [!DNL Brands], [!DNL Campaigns], and [!DNL Content] assets. They can also edit and delete assets they have created. GenStudio for Performance Marketing supports the quick creation of hundreds of pieces of content. These users can generate content sections or whole experiences that orchestrate discrete pieces of approved content to meet the needs of specific marketing campaigns.

Editors interact with GenStudio for Performance Marketing generative AI technologies through _prompting_. The prompt area in the Canvas provides tools to place prompts in the context of a specific campaign's guidelines. As a result, the quality and success of generated content partially depend on the quality of the brand guidelines your organization has uploaded and the specificity of your prompt.

See [Write effective prompts](effective-prompts.md).

The following table displays the default editor permissions:

| Feature | Create  | Update | Delete | View |
|-----------|----------------|----------------|----------------|----------------|
|   [!DNL Brands]| no  | no | no |  yes |
|   [!DNL Campaigns] | yes    |   yes      |  yes       |    yes       |
|   [!DNL Content] |     yes  |   yes     |    yes   |   yes      |
|   [!DNL Insights] |  can configure ad connectors only  |    |     |   yes  |
|   [!DNL Personas] | yes    |   yes      |  yes       |    yes       |
|   [!DNL Products] | yes    |   yes      |  yes       |    yes       |
|   [!DNL Reviews and approvals]  |   yes     |  yes   |    yes     |    yes     |

### GenStudio for Performance Marketing collaborators

**Collaborators** can view assets in GenStudio for Performance Marketing but not create, edit, or delete these assets. Collaborators include stakeholders who are essential to the success of the review and approval process for content but who do not need to create or directly edit content. Legal experts and managers of creators are examples of potential collaborators. GenStudio for Performance Marketing collaborators might have permissions to create and view assets in other Creative Cloud products.

The following table displays the default collaborator permissions:

| Feature | Create  | Update | Delete | View |
|-----------|----------------|----------------|----------------|----------------|
|   [!DNL Brands]| no  | no | no |  yes |
|   [!DNL Campaigns] | no    |   no      |  no       |    yes       |
|   [!DNL Content] |     no  |   no     |    no   |   yes      |
|   [!DNL Insights] |    no |  no  |   no  |   yes  |
|   [!DNL Personas] | no    |   no      |  no       |    yes       |
|   [!DNL Products] | no    |   no      |  no       |    yes       |
|   [!DNL Reviews and approvals] |   no     |   no  |  no       |   yes      |

### GenStudio for Performance Marketing system managers

**GenStudio system managers** complete the initial tasks that prepare your organization to deploy GenStudio for Performance Marketing.

The following table displays the default GenStudio for Performance Marketing system manager permissions:

| Feature | Create  | Update | Delete | View |
|-----------|----------------|----------------|----------------|----------------|
|   [!DNL Brands]| yes  | yes | yes |  yes |
|   [!DNL Campaigns] | yes    |   yes      |  yes       |    yes       |
|   [!DNL Content] |     yes  |   yes     |    yes   |   yes      |
|   [!DNL Insights] |  yes   |  yes  |   yes |  yes   |
|   [!DNL Personas] | yes    |   yes      |  yes       |    yes       |
|   [!DNL Products]  | yes    |   yes      |  yes       |    yes       |
|   [!DNL Reviews and approvals] |  yes      | yes    |     yes    |   yes      |


## Prepare GenStudio for Performance Marketing to generate content

GenStudio for Performance Marketing system managers prepare their organization's GenStudio for Performance Marketing environment for editors and collaborators to create campaign assets. These preliminary set-up tasks include:

1. [Add guidelines](./guidelines/overview.md) for [!DNL Brands], [!DNL Products], and [!DNL Personas]. Setting up the key building blocks of your organization's brand identity is an essential prerequisite for the work of creators and collaborators. You can either upload brand guideline documents or manually enter brand information.
   * **Prepare your guidelines documents**. The more descriptive and comprehensive your brand guidelines, the better the output. Include brief examples of features that you consider essential to your brand and add descriptions of behavior you want to exclude from content creation. GenStudio for Performance Marketing extracts information from these uploaded documents and begins building your brand. Information such as brand voice, channel, and image guidelines, are populated as GenStudio for Performance Marketing assembles each guideline from your uploaded documents.
   * **Edit or complete brand guideline fields as needed**. Comprehensive brand guidelines form the basis of GenStudio for Performance Marketing understanding of your organization's brand. Once GenStudio for Performance Marketing has extracted the information it needs from your brand guideline documents, you are prompted to manually edit or complete fields of extracted information. Specify individual product focus areas for content creation by adding a [!DNL Product]. [!DNL Personas] guidelines help tailor content creation for defined customer segments.

   Although setting up an organization's brand guidelines can be a one-time action, you might need to revise and enhance these guidelines based on your organization's volatility, growth, and changing market circumstances.

1. **[Upload templates](./content/use-templates.md)**. Templates provide shortcuts and accelerate content creation. A template contains approved features, such as headers and footers, and establishes guardrails for content creation. System managers typically upload and manage templates for their organization. Creators use templates to jumpstart the content creation process within the established boundaries of the organizational brand.

1. **[Upload approved assets](./content/manage-assets.md)**. Approved assets in [!DNL Content] are available to all GenStudio for Performance Marketing creators. You can seed [!DNL Content] with assets that creators can use to create new experiences or assets.

1. **[Connect to a Meta (Facebook) account](./insights/connect-channel.md)**. Configure a connection between GenStudio for Performance Marketing and your organization's social accounts to receive data from your active marketing campaigns, assets, and experiences. [[!DNL Insights]](./insights/overview.md) provides tools to analyze channel-derived data.
