---
title: Email Template Guidelines
description: Follow best practices when using email templates with Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Developer, User
feature: Media Templates
exl-id: 8b1e8d32-5a23-45ce-a2d4-ae6de3698c45
---
# Email template guidelines

A marketing email template serves as the foundation for visually engaging and responsive email campaigns. In general, HTML templates allow you to control the layout, typography, colors, and imagery to align with your brand guidelines. When preparing your template for use in GenStudio for Performance Marketing, use semantic HTML and inline CSS for styling, and avoid scripts or external dependencies. Well-structured HTML templates can enhance the recipient's experience and improve deliverability and engagement rates.

Follow these design best practices when customizing email templates to work with GenStudio for Performance Marketing:

- Use Adobe or Google fonts
- Use clean and responsive HTML and inline CSS
- Do **not** use JavaScript
- Do **not** use fixed width in body or container
- Do **not** use base64 encoding for images because it can significantly increase the template size
- The maximum HTML file size is 102 KB

## Recognized field names

When you customize your email template, use content placeholders for the following required fields:

- `headline`
- `sub_headline`
- `body`
- `cta`
- `image` (selected from Content JPEG, PNG, or GIF)

GenStudio for Performance Marketing automatically generates the following fields. Rich text is not enabled. You don't have to apply content placeholders for:

- `pre_header`
- `subject`

The maximum fields allowed in a template are 20. See [Content placeholders](/help/user-guide/content/customize-template.md#content-placeholders) to understand more about using field names in templates.

## Multi-section email

_Sections_ allow you to organize content into distinct groups, supporting more complex layouts. In GenStudio for Performance Marketing, you can define each section using a group naming convention. See [Customize template sections](/help/user-guide/content/customize-template.md#sections-or-groups).

Multi-section templates can have 0, 2, or 3 sections:

- A basic template (zero sections) can generate a single set of template elements, which doesn't require the group naming convention.
- A complex template (multiple sections) can generate up to three sets of template elements, which requires you to adhere to the group naming convention: `<groupname_fieldname>`. 
- When using multiple sections, any elements left standalone, outside of a section, will not be populated.

Here are examples of field names, using the group naming convention, for two sections:

- In section 1:`pod1_headline`, `pod1_body`, `pod1_cta`
- In section 2:`pod2_headline`, `pod2_body`, `pod2_cta`

## Template examples

+++Example: Email template with one section

Here is a basic example of an HTML email template with one section. The `<head>` includes simple inline CSS for styling, and the `<body>` uses content placeholders such as `pre_header`, `headline`, `sub_headline`, `body`, `cta`, and `image` with link, and. These placeholders allow GenStudio for Performance Marketing to inject dynamic content during email generation.

```html
<!DOCTYPE html>
<html>
    <head>
        <title>Marketing Email</title>
        <style>
            .container {
                width: 100%;
                padding: 20px;
                font-family: Arial, sans-serif;
            }
            .cta-button {
                display: inline-block;
                background-color: #fff;
                color: #000;
                border: 2px solid #000;
                padding: 10px 20px;
                text-decoration: none;
                font-family: 'Source Sans Pro', Arial, sans-serif;
                font-weight: 600;
                font-size: 14px;
                margin-top: 20px;
                text-align: center;
            }
        </style>
    </head>
    <body>
        <div class="container">
            {{pre_header}}
            <h1>{{headline}}</h1>
            <p>
                <a href="{{link}}">
                    <img alt="banner headline" src="{{image}}" width="600" height="600">
                </a>
            </p>
            <h2>{{sub_headline}}</h2>
            <p>{{body}}</p>
            <a href="#" class="cta-button">{{cta}}</a>
        </div>
    </body>
</html>
```

+++

+++Example: Email template with multiple sections

Here is the same HTML template in the example above, but with two more sections. The head contains inline CSS for styling a group. The body uses two groups with [content placeholders](#content-placeholders) using a prefix.

```html
<!DOCTYPE html>
<html>
    <head>
        <title>Adobe</title>
        <style>
            .container {
            width: 100%;
            padding: 20px;
            font-family: Arial, sans-serif;
            }
            .pod {
            background-color: #f8f8f8;
            margin: 10px;
            padding: 20px;
            border-radius: 5px;
            }
            .pod h2 {
            color: #333;
            }
            .pod p {
                color: #666;
            }
            .cta-button {
            display: inline-block;
            background-color: #fff; /* Background color to white */
            color: #000; /* Text color to black */
            border: 2px solid #000; /* Border color to black */
            padding: 10px 20px;
            text-decoration: none;            
            font-family: 'Source Sans Pro', Arial, sans-serif;
            font-weight: 600; /* Semibold */
            font-size: 14px;
            margin-top: 20px;
            text-align: center;
            }
        </style>
    </head>
    <body>{{pre_header}}
        <div class="container">
            <!-- Pod1 -->
            <div class="pod">
                <h2>{{pod1_headline}}</h2>
                <p><img alt="pic1" src="{{pod1_image}}" width="200" height="200" border="0"></p>
                <p>{{pod1_body}}</p>
            </div>
            <!-- End of Pod1 -->
            <!-- Pod2 -->
            <div class="pod">
                <h2>{{pod2_headline}}</h2>
                <p><img alt="pic2" src="{{pod2_image}}" width="200" height="200" border="0"></p>
                <p>{{pod2_body}}</p>
            </div>
            <!-- End of Pod2 -->
            <a href="#" class="cta-button">{{cta}}</a>
        </div>
    </body>
</html>
```

+++
