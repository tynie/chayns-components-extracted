# ContextMenu

**Package:** `@chayns-components/core` (5.0.0-beta.1411)

## Code Example

```tsx
import React, { FC } from 'react';
import { ContextMenu, ContextMenuItem } from '@chayns-components/core';

const ITEMS: ContextMenuItem[] = [
    {
        icons: ['fa fa-pencil'],
        key: 'rename',
        onClick: () => alert('Option "Umbenennen" wurde geklickt...'),
        text: 'Umbenennen',
    },
    {
        icons: ['fa fa-eye'],
        key: 'show',
        onClick: () => alert('Option "Einblenden" wurde geklickt...'),
        text: 'Einblenden',
        shouldShowSpacer: true,
    },
    {
        icons: ['fa fa-trash'],
        key: 'delete',
        onClick: () => alert('Option "Löschen" wurde geklickt...'),
        text: 'Löschen',
    },
];

const Component: FC = () => {
    return <ContextMenu items={ITEMS} />;
};

Component.displayName = 'Component';

export default Component;

```

## Props

| Name | Type | Required | Description |
|------|------|----------|-------------|
| `alignment` | `ContextMenuAlignment` |  | Context menu alignment |
| `children` | `ReactNode` |  | Children element |
| `container` | `Element` |  | Container element |
| `coordinates` | `ContextMenuCoordinates` |  | Custom coordinates |
| `headline` | `string` |  | Context menu headline |
| `items` | `ContextMenuItem[]` | ✓ | Menu items |
| `onHide` | `() => void` |  | Hide callback function |
| `onShow` | `() => void` |  | Show callback function |
| `shouldCloseOnPopupClick` | `boolean` |  | Close on popup click flag |
| `shouldDisableClick` | `boolean` |  | Disable click flag |
| `shouldHidePopupArrow` | `boolean` |  | Hide popup arrow flag |
| `shouldShowHoverEffect` | `boolean` |  | Show hover effect flag |
| `zIndex` | `number` |  | Z-index value |
| `ref` | `ContextMenuRef` |  |  |

## Types

### ContextMenuAlignment

```typescript
{ TopLeft = 0, BottomLeft = 1, TopRight = 2, BottomRight = 3, TopCenter = 4, BottomCenter = 5 }
```

### ContextMenuCoordinates

```typescript
ContextMenuCoordinates
```

### ContextMenuItem

```typescript
ContextMenuItem
```

### ContextMenuRef

```typescript
{ hide: VoidFunction; show: VoidFunction; }
```

