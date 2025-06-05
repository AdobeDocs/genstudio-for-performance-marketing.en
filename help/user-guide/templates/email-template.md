---
title: Email template guidelines
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

GenStudio for Performance Marketing automatically generates the `subject` field for emails. When you customize your template, use content placeholders for the following required fields:

- `pre_header` (rich text not enabled)
- `headline`
- `sub_headline`
- `body`
- `cta`
- `image` (selected from Content JPEG, PNG, or GIF)

The maximum fields allowed in a template are 20. See [Content placeholders](/help/user-guide/content/customize-template.md#content-placeholders) to understand more about using field names in templates.

## Multi-section email

_Sections_ allow you to organize content into distinct groups, which supports more complex layouts. In Genstudio for Performance Marketing, you can define each section using a group naming convention. See [Customize template sections](/help/user-guide/content/customize-template.md#sections-or-groups).

Multi-section templates can have 0, 2, or 3 sections:

- A basic template (zero sections) can generate a single set of template elements, which does not require the group naming convention.
- A complex template (multiple sections) can generate up to three sets of template elements, which requires you to adhere to the group naming convention: (`groupname_fieldname`)

Example field names for two sections:

- `pod1_headline`, `pod1_body`, `pod1_cta`
- `pod2_headline`, `pod2_body`, `pod2_cta`

## Template examples

+++Example: Email template with one section

The following is a basic example of an HTML template for an email that contains one section. The head contains simple, inline CSS for styling. The body contains a `pre_header`, `headline`, and `image` [placeholder](#content-placeholders) for use by GenStudio for Performance Marketing to inject content during the email generation process.

```html {line-numbers="true" highlight="13"}
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
        </style>
    </head>
    <body>{{pre_header}}
        <div class="container">
            <h1>{{headline}}</h1>
            <p><a href="{{link}}">
            <img alt="{{headline}}"
                    src="{{image}}"
                    width="600" height="600"
                    border="0"/></a></p>
            <p>{{body}}</p>
        </div>
    </body>
</html>
```

+++

+++Example: Email template with multiple sections

The following is the same HTML template in the example above, but with two more sections. The head contains inline CSS for styling a group. The body uses two groups with [content placeholders](#content-placeholders) using a prefix.

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
        </style>
    </head>
    <body>{{pre_header}}
        <div class="container">
            <h1>{{headline}}</h1>
            <p>{{body}}</p>
            <!-- Pod1 -->
            <div class="pod">
                <h2>{{pod1_headline}}</h2>
                <p><img alt="{{ headline }}" src="{{pod1_image}}" width="200" height="200" border="0"></p>
                <p>{{pod1_body}}</p>
            </div>
            <!-- End of Pod1 -->
            <!-- Pod2 -->
            <div class="pod">
                <h2>{{pod2_headline}}</h2>
                <p><img alt="{{headline}}" src="{{pod2_image}}" width="200" height="200" border="0"></p>
                <p>{{pod2_body}}</p>
            </div>
            <!-- End of Pod2 -->
        </div>
    </body>
</html>
```

+++
