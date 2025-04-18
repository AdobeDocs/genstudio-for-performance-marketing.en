---
title: Customize a Template
description: Learn how to customize your HTML template using content placeholders recognized by Adobe GenStudio for Performance Marketing generative AI.
level: Intermediate
role: Developer
feature: Media Templates, Content Generation, Generative AI
exl-id: 292c1689-1b12-405d-951e-14ee6aebc75a
---
# Customize a template

You can customize a template for use in GenStudio for Performance Marketing by inserting content placeholders, or fields, that the generative AI uses to insert content.

The next few sections explain how to adapt your HTML templates for GenStudio for Performance Marketing by using the _[!DNL Handlebars]_ templating language. The [!DNL Handlebars] syntax uses regular text with double braces as content placeholders. See [What is [!DNL Handlebars]](https://handlebarsjs.com/guide/#what-is-handlebars) in the _Handlebars language guide_ to learn how to prepare your template.

Once your template is ready, you can [upload it to GenStudio for Performance Marketing](use-templates.md#upload-a-template) and start generating personalized emails based on your custom template.

>[!TIP]
>
>Follow [accessibility guidelines](accessibility-for-templates.md) and [best practices](/help/user-guide/content/best-practices-for-templates.md) so that you can reach more of your audience and provide an optimal experience.

## Content placeholders

GenStudio for Performance Marketing recognizes certain [elements](use-templates.md#template-elements) within a template, but only if you identify them with a [recognized field name](#recognized-field-names).

Within the head or body of an HTML template, you can use the [!DNL Handlebars] syntax to insert a content placeholder where you require GenStudio for Performance Marketing to populate the template with actual content. GenStudio for Performance Marketing recognizes and interprets the content placeholders based on the [recognized _field_ name](#recognized-field-names).

For example, you can use `{{ headline }}` with the [!DNL Handlebars] syntax to indicate where the headline of the email should be placed. GenStudio recognizes this field, generates a relevant headline based on your guidelines and prompt criteria, and inserts the headline in this location:

```handlebars
<div>{{ headline }}</div>
```

### Recognized field names

The following table lists the field names recognized by GenStudio for Performance Marketing for adding a placeholder into a template. Add these field names using the [!DNL Handlebars] syntax to your template where you need GenStudio for Performance Marketing to generate a certain type of content.

| Field                   | Role                      | Channel template                                 |
| ----------------------- | ------------------------- | ------------------------------------------------ |
| `{{pre_header}}`        | Preheader                 | email                                            |
| `{{headline}}`          | Headline                  | email <br>Meta ad <br>Banner and Display ad <br>LinkedIn ad |
| `{{sub_headline}}`      | Sub-Headline              | email<br>Banner and Display ad                   |
| `{{introductory_text}}` | Introductory text         | LinkedIn ad                                      |
| `{{body}}`              | Body copy                 | email <br>Meta ad <br>Banner and Display ad      |
| `{{cta}}`               | Call to action<br>See [Calls to action](#calls-to-action) | email <br>Meta ad <br>Banner and Display ad <br>LinkedIn ad |
| `{{image}}`             | Image—select from [!DNL Content] | email <br>Meta ad <br>Banner and Display ad <br>LinkedIn ad |
| `{{on_image_text}}`     | On image text<br>See [On image text](#on-image-text). | Meta ad <br>LinkedIn ad                          |
| `{{link}}`              | Call to action on image<br>See [Link on image](#link-on-image). | email      |

<!-- | `{{brand_logo}}`        | Logo of selected brand<br>See [Brand logo field name](#brand-logo-field-name). | email<br>Meta ad <br>LinkedIn ad | -->

GenStudio for Performance Marketing generates certain fields automatically in the following templates:

- **Email template** does not require you to identify the `subject` field
- **Meta ad template** does not require you to identify the `headline`, `body`, and `CTA` fields
- **Banner and Display ad template** does not require you to identify the `CTA` field
- **LinkedIn ad template** does not require you to identify the `headline`, `introductory_text`, and `CTA` fields

>[!WARNING]
>
>For Instagram ads, the generated headline does not appear in the final experience.

There is a limit of 20 fields when uploading a template to GenStudio for Performance Marketing. Since the `subject` field is automatically generated in an email, it counts as one field. This means that there are 19 fields allowed in an email template.

>[!TIP]
>
>You can verify your template using the [template preview](#template-preview) in GenStudio for Performance Marketing.

### Calls to action

A Call to action (CTA) includes a phrase and a link. For the _[!UICONTROL Rephrase]_ and _[!UICONTROL Add link]_ capabilities to work properly during the variant generation process, you must include placeholders for the link and the phrase in your template.

Use the following guidance to set up CTA placeholders:

- CTA rephrase is available and link is editable

   ```html
   <a class="button" href="{{pod1_link}}" >{{cta}}</a>
   ```

- CTA rephrase is available, but link is **not** editable because actual link is provided in the template

   ```html
   <a align="center" href="https://link">{{cta}}</a>
   ```

- CTA link is editable, but rephrase is **not** available because phrase is provided in the template

   ```html
   <a class="button" href="{{pod1_link}}" >Register now</a>
   ```

GenStudio for Performance Marketing can provide variant calls-to-action phrases, too. See [Revise Call to action](/help/user-guide/create/manage-variants.md#revise-call-to-action).

### Link on image

You can customize your email template to allow creatives to add a link to an image. Similar to the CTA link, use the following guidance to apply a `link` placeholder to an image tag:

```html
<a href="{{link}}"><img src="image-source.jpg" alt="{{imageDescription}}"></a>
```

In this example:

- `{{link}}` is a placeholder for the actual URL.
- `src="image-source.jpg"` should be replaced with the actual image source URL.
- `{{imageDescription}}` is a user-defined field name that provides a placeholder for the image's alternative text, which is useful for accessibility and SEO.

<!-- this field does not work in Create canvas 2025/03

### Brand logo field name

At this time, you cannot select the brand logo for the template upload. The following examples demonstrate two methods that conditionally render the brand logo. Each method verifies the source, provides a default or alternative image in case the brand logo is not available, and applies a style:

**Example 1**: Using [!DNL Handlebars] Built-in Helpers condition directly in the HTML `img src` attribute:

```html
<img src="{{#if brand_logo}}{{brand_logo}}{{else}}<default-image>{{/if}}" alt="img alt text" style="max-width: 88px; margin: 10px auto; display: block;">
```

**Example 2**: Using [!DNL Handlebars] Built-in condition statement to wrap the HTML `img` tag:

```html
{{#if brand_logo}}
    <img src="{{brand_logo}}" alt="img alt text" style="width: 120px; height: 45px; margin: 10px auto; display: block;">
    {{else}}
    <img src="data:image/png;base64,iVBORw0KGgo..." alt="img alt text" style="width: 120px; height: 45px; margin: 10px auto; display: block;">
{{/if}}
```

-->

### Manual field names

All other field names are user-defined and treated as manually populated fields. For example, you may want to reserve a section for footer content.

To create an editable section, add double brackets around the section name:

```html
<tbody>
    <tr>
        <td>
            <p><span class="footer-text">{{ footerLegal }}</span></p>
        </td>
    </tr>
</tbody>
```

## On image text

The `{{ on_image_text }}` placeholder is used to specify a text overlay of short impactful messages, placed directly on the image in an experience.

```html
<div class="image-text">{{ on_image_text }}</div>
```

## Sections or groups

_Sections_ inform GenStudio for Performance Marketing that the fields in this section require a high degree of coherence. Establishing this relationship helps the AI to generate content that matches the creative elements in the section.

Use a prefix of your choice in the field name to indicate that a field is part of a section or group. Use a field name (`headline`, `body`, `image`, or `cta`) after the underscore (`_`).

- _Correct_ (👍): `pod1_body`
- _Incorrect_ (❌): `pod1_link`

Each section can use only one of each field type. For example, the following fields belong to the `pod1` section:

- `pod1_headline`
- `pod1_body`
- `pod1_image`
- `pod1_cta`

Because of this rule, the sections cannot be nested.

Each template type, such as email or Meta ad, has channel-specific constraints on the use of sections. See [channel-specific guidelines](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/content/templates/best-practices-for-templates#follow-channel-specific-template-guidelines) in the _Best practices for using templates_ topic.

For example, an email template can include up to three sections; therefore, you could have three headline and body sections:

- `pre_header`
- `pod1_headline`
- `pod1_body`
- `pod2_headline`
- `pod2_body`
- `pod3_headline`
- `pod3_body`
- `cta`

GenStudio for Performance Marketing understands that `pod1_headline` is more closely related to `pod1_body` than to `pod2_body`.

See [Structured prompts](/help/user-guide/effective-prompts.md#structured-prompts) to learn how to craft a prompt that generates varying content for each section in a multi-section email.

## Template preview

When you [upload a template](use-templates.md#upload-a-template), GenStudio for Performance Marketing scans the HTML file for recognized fields. Use the preview to review your [template elements](use-templates.md#template-elements) and confirm that you identified them properly with the [recognized field names](#recognized-field-names).

Example Preview for an email template:

![Preview fields detected](/help/assets/template-detected-fields.png "Check detected fields"){zoomable="yes"}

See [Template code editor](/help/user-guide/content/code-editor.md).

### Control preview

You can control the visibility of special content by using Built-in Helpers (special expressions in the [!DNL Handlebars] template language that perform certain actions). For example, you can add a conditional statement that adds tracking parameters to links in the exported template while keeping the preview links clean.

The `_genStudio.browser` value is set when rendering a template, and the `genStudio.export` value is set when exporting a template. You may decide to include certain content at the top of an email using a conditional wrapper, for example, when the template is used for export:

```handlebars
{{#if _genStudio.export}}
<%@ include view='emailParent' %>
{{/if}}
```

Another example may be to prevent the use of tracking codes when previewing a template in GenStudio for Performance Marketing. The following example shows how to add tracking parameters to links in the exported template, while keeping the preview links clean:

```html
<a class="button" {{#if _genStudio.browser }}
   href="{{ link }}"{{/if}}{{#if _genStudio.export }}
   href="{{ link }}?trackingid=<%=getTrackingId()%>&mv=email"{{/if}}
   target="_blank">{{ cta }}</a>
```

## Static content

Email and Meta templates often link to images and CSS files hosted on other domains. When GenStudio for Performance Marketing generates thumbnails for template previews or the experiences derived from them, it validates the content source and embeds a copy for preview purposes.

External files are temporarily embedded only for the purpose of creating the template preview, which ensures that the preview accurately reflects the content as it appears at the time of creation. These external files are **not** stored permanently in GenStudio for Performance Marketing. After the template preview is created, GenStudio for Performance Marketing continues to reference the original source link provided in the template.

### Refresh content

If the source changes after creating the initial preview, use the [refresh](/help/user-guide/content/use-templates.md#refresh-template) function to update the template preview with the most recent version of the content from the external sources.

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
    <body>{{ pre_header }}
        <div class="container">
            <h1>{{ headline }}</h1>
            <p><a href="{{ link }}">
            <img alt="{{ headline }}"
                    src="{{ image }}"
                    width="600" height="600"
                    border="0"/></a></p>
            <p>{{ body }}</p>
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
    <body>{{ pre_header }}
        <div class="container">
            <h1>{{ headline }}</h1>
            <p>{{ body }}</p>
            <!-- Pod1 -->
            <div class="pod">
                <h2>{{ pod1_headline }}</h2>
                <p><img alt="{{ headline }}" src="{{ pod1_image }}" width="200" height="200" border="0"></p>
                <p>{{ pod1_body }}</p>
            </div>
            <!-- End of Pod1 -->
            <!-- Pod2 -->
            <div class="pod">
                <h2>{{ pod2_headline }}</h2>
                <p><img alt="{{ headline }}" src="{{ pod2_image }}" width="200" height="200" border="0"></p>
                <p>{{ pod2_body }}</p>
            </div>
            <!-- End of Pod2 -->
        </div>
    </body>
</html>
```

+++

+++Example: Meta ad template

The following is a basic example of a Meta ad template. The head contains inline CSS for styling. The body uses [content placeholders](#content-placeholders), such as `image` and `on_image_text`, to indicate where GenStudio for Performance Marketing can generate content.

```html {line-numbers="true" highlight="33"}
<!DOCTYPE html>
<html>
    <head>
        <meta charset="UTF-8" />
        <meta name="viewport" content="width=device-width, initial-scale=1.0" />
        <title>Adobe</title>
        <style>
            .ad-container {
            font-family: Helvetica, sans-serif;
            position: relative;
            text-align: center;
            height: 100%;
            }
            .ad-image {
            width: 100%;
            height: 100%;
            object-fit: cover;
            }
            .ad-text {
            position: absolute;
            top: 0;
            left: 0;
            margin: 1em;
            background-color: rgba(0, 0, 0, 0.5);
            color: white;
            padding: 1em;
            font-size: 75px;
            }
        </style>
    </head>
    <body>
        <div class="ad-container">
            <img src="{{ image }}" alt="Ad Image" class="ad-image" />
            <div class="ad-text">{{ on_image_text }}</div>
        </div>
    </body>
</html>
```

+++
