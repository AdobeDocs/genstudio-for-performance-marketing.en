---
title: Set up Adobe GenStudio for Performance Marketing
description: Learn how to set up your GenStudio for Performance Marketing to generate new brand-aligned marketing content.
level: Beginner
feature: Prompt, Brands Service, Personas Service, Products Service, Generative AI, Guidelines
exl-id: bcb03198-bbcb-45ae-af01-25c1e834b563
---

# Set up Adobe GenStudio for Performance Marketing

GenStudio system managers prepare their organization's Adobe GenStudio for Performance Marketing environment before content editors and collaborators start creating and reviewing campaign assets. These preliminary set-up tasks focus on either manually entering or uploading the organization-specific information that the product's generative AI capabilities can use to support content creation.

Once an Adobe system admin has provisioned your organization's product instance and assigned GenStudio system manager permissions, a GenStudio system manager can prepare the product's underlying generative AI framework by either manually entering or uploading your organization's specific brand requirements.

## Step 1: Add guidelines

Setting up the key building blocks of your organization's brand identity is an essential prerequisite for the work of content editors and collaborators. Guidelines capture brand characteristics such as logos, tone of voice, and color palettes. You can either upload brand guideline documents or manually enter brand information. GenStudio for Performance Marketing's underlying generative AI capabilities use these guidelines to establish guardrails that guide the content generation. 

### Prepare your guideline documents

Comprehensive, focused [!DNL Brands], [!DNL Products], and [!DNL Personas] guidelines define core aspects of your organization's marketing campaigns. GenStudio for Performance Marketing extracts information from this information to begin building your brand.

Follow these general guidelines when preparing guidelines:

* Use specific as possible in language and specification

* Include the best examples you can find of the style and tone you want campaign assets to embody. 

* Avoid redundancy. You might be tempted to repeat a directive multiple times, but redundancy in your guidlines does not help the underlying LLM capture and implement your brand guidelines.

* Identify elements you want the LLM to exclude during content generation (for example, exclamation points in text)

You can upload guideline documents or consult them as you manually enter information into GenStudio for Performance Marketing. See [Add guidelines](./guidelines/overview.md) for guidance on uploading or entering this information.

### Edit or complete brand guideline fields as needed

Once GenStudio for Performance Marketing has extracted the information it needs from your brand guideline documents, you are prompted to manually edit or complete fields of extracted information. Specify individual product focus areas for content creation by adding a [!DNL Product]. [!DNL Personas] guidelines help tailor content creation for defined customer segments.

Although setting up an organization's brand guidelines can be a one-time action, you might need to revise and enhance these guidelines based on your organization's volatility, growth, and changing market circumstances.

## Step 2: Upload templates

Templates provide shortcuts and accelerate content creation. A template contains approved features, such as headers and footers, and are often optimized for specific channels. System managers typically upload and manage templates for their organization. Content editors use templates to jumpstart the content creation process within the established boundaries of the organizational brand.

See [Work with templates](./content/templates/use-templates.md) for directions on customizing and uploading templates.

## Step 3: Upload approved assets

Approved assets in [!DNL Content] are available to all GenStudio for Performance Marketing editors. You can seed [!DNL Content] with assets that content editors can use to create new experiences or assets. See [Upload approved assets](./content/manage-assets.md) for guidance on uploading and managing assets.

## Step 4: Connect to a Meta (Facebook) account

Configure a connection between GenStudio for Performance Marketing and your organization's social accounts to receive data from your active marketing campaigns, assets, and experiences. [[!DNL Insights]](./insights/overview.md) provides tools to analyze channel-derived data. See [Connect to a Meta (Facebook) account](./insights/connect-channel.md).
