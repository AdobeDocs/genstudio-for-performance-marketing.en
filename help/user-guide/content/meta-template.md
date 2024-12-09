---
title: Prepare a Meta ad template for Adobe GenStudio for Performance Marketing
description: Learn how to build a custom Meta ad template for Adobe GenStudio for Performance Marketing.
level: Intermediate
hidefromtoc: yes
feature: Templates, Content
exl-id: e69039b0-272d-4f39-b0e4-916be710fd5f
---
# Prepare Meta ad template for Adobe GenStudio for Performance Marketing

Creating a Meta ad template involves a structured approach tailored for social media. After a Meta ad template is designed and tested, you can prepare it for upload and use in GenStudio for Performance Marketing.

## Add guidelines

Before you prepare a Meta ad template, ensure that you have added [guidelines](/help/user-guide/guidelines/overview.md) to your GenStudio for Performance Marketing and populated them with comprehensive info for relevant brands. The [brand guidelines](/help/user-guide/guidelines/brands.md) directly influence generated content.

**Example**: If you want the body of a Meta ad template to be no larger than 500 characters, add that requirement to the [channel guidelines](/help/user-guide/guidelines/brands.md#channel-guidelines) for the "body" field.

If guidelines are not added to GenStudio for Performance Marketing, defaults are used.

## Design a template

Typically, a designer creates the visual design of a template in a design program such as Adobe XD.

See [Template elements](use-templates.md#template-elements) and [Template examples](/help/user-guide/content/customize-template.md#template-examples).

### Ad specifications

GenStudio for Performance Marketing supports these aspect ratios for Meta ads:

* Square (1:1): 1080 x 1080 pixels
* Vertical (4:5): 1080 x 1350 pixels
* Story (9:16): 1080 x 1920 pixels

If the ad is not designed in one of these aspect ratios, GenStudio for Performance Marketing automatically crops the image into the appropriate size.

## Test a Meta ad template

Test your template using Meta's Creative Hub to see how the ad looks in different placements such as in a feed or as a story.

Use your email delivery or proofing platform to test your email and verify that it renders properly across different email clients and devices.

## Define generated content areas

Define the areas in your email template that should be dynamically populated with content from GenStudio for Performance Marketing.

To define generated content areas:

* Identify the text elements in the template that GenStudio for Performance Marketing should auto-generate, such as the headline or CTA.
* Adapt your HTML template by inserting placeholders within it using the Handlebars syntax.

See [Content placeholders](/help/user-guide/content/customize-template.md#content-placeholders).

## Preview the template

Control the visibility of specific content areas with Built-In Helpers. For example, include tracking parameters to links in an exported template while maintaining clean preview links.

See [Template preview](/help/user-guide/content/customize-template.md#template-preview).

## Upload and use template

After your template is designed, coded, tested, and previewed, upload it to GenStudio for Performance Marketing for use in generating brand new marketing content.

See [Working with templates](use-templates.md).
