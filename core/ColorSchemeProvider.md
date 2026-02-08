# ColorSchemeProvider

**Package:** `@chayns-components/core` (5.0.0-beta.1411)

## Code Example

```tsx
import React, { FC } from 'react';
import { ColorSchemeProvider } from '@chayns-components/core';

const Component: FC = () => {
    return (
        <ColorSchemeProvider>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Ut vel finibus nunc, a cursus
            magna.
        </ColorSchemeProvider>
    );
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
| `siteId` | `string` |  | The site id of the page for which the design settings should be fetched |
| `style` | `{ [key: string]: string \| number }` |  | Additional styles set on the root element |

