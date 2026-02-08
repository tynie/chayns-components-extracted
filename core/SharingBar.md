# SharingBar

**Package:** `@chayns-components/core` (5.0.0-beta.1411)

## Code Example

```tsx
import React, { FC } from 'react';
import { SharingBar, ContextMenuAlignment } from '@chayns-components/core';

const Component: FC = () => {
    return (
        <SharingBar
            label="Teilen"
            link="https://www.google.com"
            popupAlignment={ContextMenuAlignment.TopLeft}
        />
    );
};

Component.displayName = 'Component';

export default Component;

```

## Props

| Name | Type | Required | Description |
|------|------|----------|-------------|
| `container` | `Element` |  | The element where the content of the `SharingBar` should be rendered via React Portal. |
| `label` | `string` | ✓ | The label that should be displayed. |
| `link` | `string` | ✓ | The link that should be shared. |
| `popupAlignment` | `ContextMenuAlignment` | ✓ | The alignment of the sharing options. |

## Types

### ContextMenuAlignment

```typescript
{ TopLeft = 0, BottomLeft = 1, TopRight = 2, BottomRight = 3, TopCenter = 4, BottomCenter = 5 }
```

