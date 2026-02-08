# FilterButtons

**Package:** `@chayns-components/core` (5.0.0-beta.1411)

## Code Example

```tsx
import React, { FC } from 'react';
import { FilterButtons, FilterButtonItem } from '@chayns-components/core';

const ITEMS: FilterButtonItem[] = [
    {
        id: '1',
        text: 'Essen',
        color: 'red',
        icons: ['fa fa-burger'],
        count: 5,
    },
    {
        id: '2',
        text: 'Getränke',
        color: 'green',
        icons: ['fa fa-bottle-water'],
        count: 74,
    },
];

const Component: FC = () => {
    return <FilterButtons items={ITEMS} />;
};

Component.displayName = 'Component';

export default Component;

```

## Props

| Name | Type | Required | Description |
|------|------|----------|-------------|
| `allCount` | `number` |  | The number that should be displayed as count in the "all" button. |
| `items` | `FilterButtonItem[]` | ✓ | The items that should be displayed. |
| `onSelect` | `(keys: string[]) => void` |  | A function that should be executed when an item is selected. |
| `selectedItemIds` | `string[]` |  | The keys of items that should be selected. |
| `shouldCalcCountForAll` | `boolean` |  | If true, the count of all items will be shown in the "all" button. |
| `size` | `FilterButtonSize` |  | The size auf the filter buttons. Use the FilterButtonSize enum. |

## Types

### FilterButtonItem

```typescript
{ id: string; text: string; color?: CSSProperties['color']; icons?: Array; count?: number; isDisabled?: boolean; }
```

### FilterButtonSize

```typescript
{ Small = 0, Normal = 1 }
```

