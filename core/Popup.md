# Popup

**Package:** `@chayns-components/core` (5.0.0-beta.1411)

## Code Example

```tsx
import React, { FC } from 'react';
import { Popup } from '@chayns-components/core';

const Component: FC = () => {
    const popupContent = <div>Lorem</div>;

    return <Popup content={popupContent}>Lorem</Popup>;
};

Component.displayName = 'Component';

export default Component;

```

## Props

| Name | Type | Required | Description |
|------|------|----------|-------------|
| `alignment` | `PopupAlignment` |  | The alignment of the popup. By default, the popup will calculate the best alignment. |
| `children` | `ReactNode` |  | The element over which the content of the `ContextMenu` should be displayed. |
| `container` | `Element` |  | The element where the content of the `Popup` should be rendered via React Portal. |
| `content` | `ReactNode` | ✓ | The content that should be displayed inside the popup. |
| `onHide` | `() => void` |  | Function to be executed when the content of the Context menu has been hidden. |
| `onShow` | `() => void` |  | Function to be executed when the content of the Context menu has been shown. |
| `shouldHideOnChildrenLeave` | `boolean` |  | Whether the tooltip should be hidden after the children is not hovered. |
| `shouldScrollWithContent` | `boolean` |  | Whether the popup should scroll with the content. |
| `shouldShowOnHover` | `boolean` |  | Whether the popup should be opened on hover. If not, the popup will be opened on click. |
| `shouldUseChildrenWidth` | `boolean` |  | Whether the width of the children should be used. |
| `shouldUseFullWidth` | `boolean` |  | Whether the popup children should use the full width. |
| `yOffset` | `number` |  | The Y offset of the popup to the children. |
| `ref` | `PopupRef` |  |  |

## Types

### PopupAlignment

```typescript
{ TopLeft = 0, TopCenter = 1, TopRight = 2, BottomLeft = 3, BottomCenter = 4, BottomRight = 5 }
```

### PopupRef

```typescript
{ hide: VoidFunction; show: VoidFunction; }
```

