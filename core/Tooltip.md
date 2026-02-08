# Tooltip

**Package:** `@chayns-components/core` (5.0.0-beta.1411)

## Code Example

```tsx
import React, { FC } from 'react';
import { Tooltip } from '@chayns-components/core';

const Component: FC = () => {
    return (
        <Tooltip
            item={{
                key: 'tooltip',
                text: 'Tooltip',
            }}
        >
            Lorem
        </Tooltip>
    );
};

Component.displayName = 'Component';

export default Component;

```

## Props

| Name | Type | Required | Description |
|------|------|----------|-------------|
| `alignment` | `PopupAlignment` |  | The alignment of the tooltip. By default, the tooltip will calculate the best alignment. |
| `children` | `ReactNode` | ✓ | The elements that the tooltip should surround. |
| `container` | `Element` |  | The element where the content of the `Tooltip` should be rendered via React Portal. |
| `isDisabled` | `boolean` |  | whether the tooltip should be shown. |
| `item` | `ITooltipItem \| ReactNode` | ✓ | The content that should be displayed. |
| `itemWidth` | `CSSProperties['width']` |  | The width of an item. |
| `maxItemWidth` | `number` |  | The max width of the Tooltip. |
| `shouldHideOnChildrenLeave` | `boolean` |  | Whether the tooltip should be hidden after the children is not hovered. |
| `shouldUseChildrenWidth` | `boolean` |  | Whether the width of the children should be used. |
| `shouldUseFullWidth` | `boolean` |  | Whether the tooltip children should use the full width. |
| `yOffset` | `number` |  | The Y offset of the tooltip to the children. |

## Types

### ITooltipItem

```typescript
{ headline?: string; text: string; imageUrl?: string; button?: unknown; }
```

### PopupAlignment

```typescript
{ TopLeft = 0, TopCenter = 1, TopRight = 2, BottomLeft = 3, BottomCenter = 4, BottomRight = 5 }
```

