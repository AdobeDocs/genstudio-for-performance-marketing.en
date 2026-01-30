---
title: Set Up Logo Swap in Templates
description: Configure brand logo placeholders in templates to enable logo swap in [!DNL GenStudio for Performance Marketing].
feature: Create Canvas, Templates
role: User
level: Intermediate
---
# Set up logo swap in templates

This guide explains how to configure brand logo placeholders in your templates to enable the [logo swap feature](/help/user-guide/create/logo-swap.md) in [!DNL GenStudio for Performance Marketing]. Use these guidelines to ensure the placeholder displays correctly across various image sizes and aspect ratios.

## Quick setup

Use the following basic template code for your logo image:

```html
<img
  src="{{brand_logo}}"
  style="{{defaultLogo}}"
  class="my-logo"
>
```

Required:

- `src="{{brand_logo}}"`—Enables logo swap functionality.
- `style="{{defaultLogo}}"`—Applies the placeholder border styling.

Optional:

- `class="my-logo"`—Your custom CSS class for sizing and styling.

## Understand the placeholder border

When no logo is selected, `{{brand_logo}}` contains a transparent 1×1 pixel image. The `{{defaultLogo}}` style automatically applies an outline so the placeholder is visible:

```css
outline: clamp(1px, 0.1em, 5px) dashed #FFF;
```

Border behavior:

- Appears when the default placeholder is shown.
- Disappears automatically after a logo is swapped.
- Scales based on the parent font size.

### Border sizing

The `clamp()` function adapts the outline thickness to the template size:

| Parent font size | Outline size |
| --- | --- |
| 10px | 1px (min) |
| 16px | 1.6px |
| 24px | 2.4px |
| 32px | 3.2px |
| 50px+ | 5px (max) |

Formula: `0.1em` equals 10% of the inherited font size, clamped between `1px` and `5px`.

## Customize the placeholder border

You can override the default outline using CSS classes. The `{{defaultLogo}}` style applies the base outline, and your class can customize color, width, and style.

Template HTML:

```html
<img
  src="{{brand_logo}}"
  style="{{defaultLogo}}"
  class="logo-custom-border"
>
```

Template CSS:

```css
.logo-custom-border {
  outline-color: #0066CC !important;
  outline-width: 2px !important;
  outline-style: dotted !important;
}
```

>[!NOTE]
>Custom outline styles only affect the placeholder. Once a logo is swapped, all outline styles are removed automatically.

## Set recommended logo sizing

To ensure the placeholder is visible and prevents layout shifts, set explicit sizing in your CSS class:

Template HTML:

```html
<img
  src="{{brand_logo}}"
  style="{{defaultLogo}}"
  class="logo-standard"
>
```

Template CSS:

```css
.logo-standard {
  width: 120px;
  height: 60px;
}
```

## Control logo positioning

Use `object-fit` and `object-position` to control how the logo scales within its container.

### Logo centered (most common)

The logo scales to fit within 150×80 pixels, centered both horizontally and vertically.

```html
<img
  src="{{brand_logo}}"
  style="{{defaultLogo}}"
  class="logo-centered"
>
```

```css
.logo-centered {
  width: 150px;
  height: 80px;
  object-fit: contain;
  object-position: center center;
}
```

### Logo aligned left

Logo scales to fit, aligned to the left edge, vertically centered.

```html
<img
  src="{{brand_logo}}"
  style="{{defaultLogo}}"
  class="logo-left"
>
```

```css
.logo-left {
  width: 200px;
  height: 60px;
  object-fit: contain;
  object-position: left center;
}
```

### Logo in the top-right corner

Logo scales to fit, positioned in the top-right corner.

```html
<img
  src="{{brand_logo}}"
  style="{{defaultLogo}}"
  class="logo-top-right"
>
```

```css
.logo-top-right {
  width: 100px;
  height: 100px;
  object-fit: contain;
  object-position: right top;
}
```

## Complete examples

### Minimal setup

```html
<img src="{{brand_logo}}" style="{{defaultLogo}}">
```

>[!NOTE]
>This setup works, but the placeholder may be nearly invisible because the transparent 1×1 pixel image collapses to its natural size. Use a CSS class with `width` and `height` for a visible placeholder.

### Recommended setup

```html
<img
  src="{{brand_logo}}"
  style="{{defaultLogo}}"
  class="brand-logo"
>
```

```css
.brand-logo {
  width: 120px;
  height: 60px;
  object-fit: contain;
  object-position: center center;
}
```

### Advanced setup with a custom border

```html
<img
  src="{{brand_logo}}"
  style="{{defaultLogo}}"
  class="sponsor-logo"
>
```

```css
.sponsor-logo {
  width: 180px;
  height: 90px;
  object-fit: contain;
  object-position: left center;
  outline-color: #0066CC !important;
  outline-width: 2px !important;
  outline-style: solid !important;
}
```

### Flexible setup with size boundaries

Use `min-*` and `max-*` properties for responsive templates or varying logo sizes.

```html
<img
  src="{{brand_logo}}"
  style="{{defaultLogo}}"
  class="logo-flexible"
>
```

```css
.logo-flexible {
  min-width: 20px;
  min-height: 20px;
  max-width: 200px;
  max-height: 100px;
  object-fit: contain;
  object-position: center center;
}
```

How it works:

- `min-width` and `min-height` keep the placeholder visible.
- `max-width` and `max-height` prevent oversized logos from breaking layout.
- The logo scales proportionally within these boundaries.

## CSS properties reference

| Category | Property | Value | Purpose |
| --- | --- | --- | --- |
| Required (HTML) | `src` | `{{brand_logo}}` | Enables logo swap functionality. |
| Required (HTML) | `style` | `{{defaultLogo}}` | Applies the placeholder outline. |
| Recommended (CSS class) | `width` | `120px` | Sets maximum logo width. |
| Recommended (CSS class) | `height` | `60px` | Sets maximum logo height. |
| Recommended (CSS class) | `object-fit` | `contain` | Scales the logo without cropping. |
| Recommended (CSS class) | `object-position` | `center center` | Controls logo alignment. |
| Optional (CSS class) | `outline-color` | `#FF0000` | Changes outline color. |
| Optional (CSS class) | `outline-width` | `3px` | Changes outline thickness. |
| Optional (CSS class) | `outline-style` | `solid` | Changes outline style. |
| Flexible sizing (CSS class) | `min-width` | `20px` | Ensures placeholder visibility. |
| Flexible sizing (CSS class) | `min-height` | `20px` | Ensures placeholder visibility. |
| Flexible sizing (CSS class) | `max-width` | `200px` | Prevents overflow. |
| Flexible sizing (CSS class) | `max-height` | `100px` | Controls layout bounds. |

## Best practices

Do:

- Always include `{{brand_logo}}` and `{{defaultLogo}}`.
- Define `width` and `height` so the placeholder is visible.
- Use CSS classes for sizing and outline customization.
- Use `object-fit: contain` to preserve logo aspect ratios.
- Test with logos of different sizes and aspect ratios.

Don't:

- Use `border` instead of `outline` (the border will not auto-hide).
- Put sizing properties in inline styles.
- Omit size constraints (the placeholder renders at 1×1 pixels).
- Use `object-fit: cover` (it may crop logos).

## Troubleshooting

Border not visible:

- Ensure `style="{{defaultLogo}}"` is included.
- Confirm that `width` and `height` are defined in your CSS class.

Placeholder is too small (1px):

- Add explicit `width` and `height` to your CSS class.

Border doesn't disappear after swap:

- Use outline properties in your CSS class, not `border`.

Logo gets cropped:

- Use `object-fit: contain` instead of `cover`.

Logo too small or too large:

- Adjust `width` and `height` in your CSS class.

Custom border not showing:

- Confirm `{{defaultLogo}}` is in the `style` attribute.
- Put custom `outline-*` properties in the CSS class.
