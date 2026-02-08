# PageProvider

**Package:** `@chayns-components/core` (5.0.0-beta.1411)

## Code Example

```tsx
import React, { FC } from 'react';
import { PageProvider } from '@chayns-components/core';

const Component: FC = () => {
    return <PageProvider>Lorem</PageProvider>;
};

Component.displayName = 'Component';

export default Component;

```

## Props

| Name | Type | Required | Description |
|------|------|----------|-------------|
| `children` | `ReactNode` | ✓ | The content of the application or the components for which the styles should be set |
| `color` | `string` |  | The hex color to be used for the children |
| `colorMode` | `ColorMode` |  | The color mode to be used for the children |
| `customVariables` | `Record<string, string>` |  | Additional variables to extend the theme |
| `iconColor` | `string` |  | An optional color for all icons |
| `secondaryColor` | `string` |  | The secondary hex color to be used for the children |
| `shouldReduceUsableHeightByCoverHeight` | `boolean` |  | Controls whether the usable height should be reduced by the cover height |
| `shouldRemovePadding` | `boolean` |  | Controls whether padding should be removed from the page |
| `shouldUseUsableHeight` | `boolean` |  | Controls whether the component should use the calculated usable height |
| `siteId` | `string` |  | The site id of the page for which the design settings should be fetched |
| `style` | `{ [key: string]: string \| number }` |  | Additional styles set on the root element |

