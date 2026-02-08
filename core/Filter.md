# Filter

**Package:** `@chayns-components/core` (5.0.0-beta.1411)

## Code Example

```tsx
import React, { FC } from 'react';
import { Filter } from '@chayns-components/core';

const Component: FC = () => {
    return <Filter headline="Filter" />;
};

Component.displayName = 'Component';

export default Component;

```

## Props

| Name | Type | Required | Description |
|------|------|----------|-------------|
| `checkboxConfig` | `CheckboxConfig` |  |  |
| `filterButtonConfig` | `FilterButtonConfig` |  |  |
| `headline` | `ReactNode` | ✓ |  |
| `onActiveChange` | `(isActive: boolean) => void` |  |  |
| `rightIcons` | `FilterRightIcon[]` |  |  |
| `searchConfig` | `SearchConfig` |  |  |
| `shouldAutoFocus` | `boolean` |  |  |
| `shouldShowRoundedHoverEffect` | `boolean` |  |  |
| `sortConfig` | `SortConfig` |  |  |
| `ref` | `FilterRef` |  |  |

## Types

### CheckboxConfig

```typescript
CheckboxProps
```

### CheckboxProps

```typescript
CheckboxProps
```

### FilterButtonConfig

```typescript
FilterButtonsProps
```

### FilterButtonsProps

```typescript
FilterButtonsProps
```

### FilterRef

```typescript
FilterRef
```

### FilterRightIcon

```typescript
{ icons: Array; onClick: VoidFunction; }
```

### SearchConfig

```typescript
{ onSearchChange: unknown; searchValue: string; }
```

### SortConfig

```typescript
{ onSortChange: unknown; selectedItem: SortItem; items: Array; }
```

### SortItem

```typescript
{ text: string; id: string | number; }
```

