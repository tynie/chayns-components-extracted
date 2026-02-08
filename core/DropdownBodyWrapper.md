# DropdownBodyWrapper

**Package:** `@chayns-components/core` (5.0.0-beta.1411)

## Code Example

```tsx
import React, { FC, useRef } from 'react';
import { DropdownBodyWrapper } from '@chayns-components/core';

const Component: FC = () => {
    const ref = useRef<HTMLDivElement>(null);

    return (
        <>
            <div ref={ref} />
            {ref.current && (
                <DropdownBodyWrapper anchorElement={ref.current} shouldShowDropdown>
                    Lorem
                </DropdownBodyWrapper>
            )}
        </>
    );
};

Component.displayName = 'Component';

export default Component;

```

## Props

| Name | Type | Required | Description |
|------|------|----------|-------------|
| `anchorElement` | `Element` | ✓ | The anchor element of the dropdown. |
| `bodyWidth` | `number` |  | The width of the Body. |
| `children` | `ReactNode` | ✓ | The content of the dropdown body. |
| `container` | `Element` |  | The element where the content should be rendered via React Portal. |
| `contentHeight` | `number` |  | The height of the content |
| `direction` | `DropdownDirection` |  | The direction of the dropdown. |
| `maxHeight` | `number` |  | The max height of the dropdown. |
| `minBodyWidth` | `number` |  | The minimum width of the body. |
| `onClose` | `() => void` |  | Function to be executed when the body is closed. |
| `onMeasure` | `DelayedDropdownContentProps['onMeasure']` |  | Function to be executed when the content is measured. |
| `onOutsideClick` | `() => boolean \| void` |  | Function to be executed when the user clicks outside the dropdown. If the function returns `true`, the dropdown will not be closed. |
| `shouldShowDropdown` | `boolean` | ✓ | Whether the dropdown should be visible. |

## Types

### DelayedDropdownContentProps

```typescript
DelayedDropdownContentProps
```

### DropdownDirection

```typescript
{ BOTTOM = 0, TOP = 1, BOTTOM_LEFT = 2, BOTTOM_RIGHT = 3, TOP_LEFT = 4, TOP_RIGHT = 5, LEFT = 6, RIGHT = 7 }
```

### DropdownMeasurements

```typescript
{ width: number; height: number; scrollHeight: number; x: number; y: number; element: Element; }
```

