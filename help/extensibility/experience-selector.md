---
title: GenStudio Experience Selector MFE
description: Understand an implement the Experience Selector Micro FrontEnd for your GenStudio apps and add-ons.
feature:
---
# GenStudio Experience Selector MFE 

Experience Selector is a Micro Frontend (MFE) that provides an `ExperienceSelectorDialog` component for selecting GenStudio experiences. Use the component in your application by importing the `renderExperienceSelectorWithSUSI` function from the standalone JavaScript bundle, which automatically loads the latest deployed Micro Frontend and presents a natural component interface.

The GenStudio Experience Selector MFE allows users to:

- Browse and select GenStudio experiences
- Filter experiences by various criteria
- Support both single and multiple selection modes
- Handle authentication through SUSI (Sign-Up Sign-In) integration
- Provide a consistent UI across different frameworks

## Integration options

The MFE can be integrated using two different approaches:

### ESM (ES Modules) - recommended

```javascript
import { renderExperienceSelectorWithSUSI } from 'https://experience-stage.adobe.com/solutions/GenStudio-experience-selector-mfe/static-assets/resources/@genstudio/experience-selector/esm/standalone.js';
```

### UMD (Universal Module Definition)

```html
<script src="https://experience-stage.adobe.com/solutions/GenStudio-experience-selector-mfe/static-assets/resources/@genstudio/experience-selector/umd/standalone.js"></script>
```

## Configuration properties

The `renderExperienceSelectorWithSUSI` function accepts a configuration object with the following properties:

| Property | Type | Required | Description |
|----------|------|----------|-------------|
| `apiKey` | string | Yes | API key for GenStudio services |
| `imsOrg` | string | Yes | IMS Organization ID |
| `env` | string | Yes | Environment (`stage`, `prod`) |
| `susiConfig` | object | Yes | [SUSI authentication configuration](#susi-configuration) |
| `onSelectionConfirmed` | function | Yes | Callback when selection is confirmed |
| `onDismiss` | function | Yes | Callback when dialog is dismissed |
| `locale` | string | No | Language locale (for example, `en-US`) |
| `isOpen` | boolean | No | Initial dialog state |
| `selectionType` | string | No | The selection mode (`single` or `multiple`) |
| `customFilters` | array | No | Custom filter criteria |
| `dialogTitle` | string | No | Custom dialog title |

### SUSI configuration

The `susiConfig` object may include:

```javascript
{
  clientId: 'genstudio',
  environment: 'stg1', // or 'prod'
  scope: 'additional_info.projectedProductContext,additional_info.ownerOrg,AdobeID,openid,session,read_organizations,ab.manage',
  locale: 'en_US',
  modalSettings: {
    width: 500,
    height: 700
  }
}
```

## QuickStart

1. **Choose your framework** from the available examples below
1. **Navigate to the example directory**
1. **Install dependencies** (for React/Vue examples)
1. **Update configuration** with your API keys and IMS organization:

   ```javascript
   const experienceSelectorProps = {
     locale: 'en-US',
     apiKey: 'exc_app',           
     imsOrg: 'your-ims-org@AdobeOrg',  // Replace with your IMS Org
     env: 'stage', // or 'prod'
     susiConfig: {
        clientId: 'genstudio',
        environment: 'stg1', // or 'prod'
        scope: 'additional_info.projectedProductContext,additional_info.ownerOrg,AdobeID,openid,session,read_organizations,ab.manage',
        locale: 'en_US',
        modalSettings: {
          width: 500,
          height: 700,
        },
     },
     customFilters: ['genstudio-channel:email'],
     selectionType: 'single', // or 'multiple'
     dialogTitle: 'Select Email Templates'
   };
   ```

1. **Run the development server**

### Example implementations

This repository includes working examples for different frameworks:

- [A complete React application demonstrating integration with Vite build system](https://github.com/adobe/genstudio-extensibility-examples/tree/main/genstudio-experience-selector-mfe/react-js).

- [A Vue 3 application with Composition API integration](https://github.com/adobe/genstudio-extensibility-examples/tree/main/genstudio-experience-selector-mfe/vue-js).

- [Two vanilla JavaScript implementations](https://github.com/adobe/genstudio-extensibility-examples/tree/main/genstudio-experience-selector-mfe/vanilla-js):

- [This Vanilla ESM version uses ES6 modules and modern JavaScript](https://github.com/adobe/genstudio-extensibility-examples/tree/main/genstudio-experience-selector-mfe/vanilla-js/vanilla-esm).

- [This Vanilla UMD version uses UMD bundle loaded via script tag](https://github.com/adobe/genstudio-extensibility-examples/tree/main/genstudio-experience-selector-mfe/vanilla-js/vanilla-umd-global-var).

## Authentication Flow

The Experience Selector handles authentication automatically through SUSI:

1. When the dialog opens, it checks for existing authentication.
1. If not authenticated, it opens a SUSI login flow.
1. After successful authentication, the experience selector is displayed.
1. Users can browse and select experiences.
1. Selected experiences are returned through the `onSelectionConfirmed` callback.
