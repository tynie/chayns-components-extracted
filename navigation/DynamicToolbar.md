# DynamicToolbar

**Package:** `@chayns-components/navigation` (5.0.0-beta.1411)

## Code Example

```tsx
import React, { FC } from 'react';
import { DynamicToolbar } from '@chayns-components/navigation';

const Component: FC = () => {
    return <DynamicToolbar />;
};

Component.displayName = 'Component';

export default Component;

```

## Props

| Name | Type | Required | Description |
|------|------|----------|-------------|
| `activeItemId` | `string \| null` |  |  |
| `className` | `string` |  |  |
| `items` | `DynamicToolbarItem[]` | ✓ |  |
| `layout` | `DynamicToolbarLayout` |  |  |
| `onItemSelect` | `(item: DynamicToolbarItem) => void` |  |  |

## Types

### DynamicToolbarItem

```typescript
DynamicToolbarItem
```

### DynamicToolbarLayout

```typescript
{ Area = "area", Hidden = "hidden", Floating = "floating" }
```

