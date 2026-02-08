# Icon

**Package:** `@chayns-components/core` (5.0.0-beta.1411)

## Code Example

```tsx
import React, { FC } from 'react';
import { Icon } from '@chayns-components/core';

const Component: FC = () => {
    return <Icon icons={['fa fa-burger']} />;
};

Component.displayName = 'Component';

export default Component;

```

## Props

| Name | Type | Required | Description |
|------|------|----------|-------------|
| `className` | `string` |  | Additional class name for the icon wrapper element. |
| `color` | `string` |  | The color of the icon. |
| `icons` | `string[]` | ✓ | The icon(s) to be displayed. |
| `isDisabled` | `boolean` |  | Whether the icon should be disabled. |
| `onClick` | `MouseEventHandler<HTMLSpanElement>` |  | Function to be executed when the icon is clicked. |
| `onDoubleClick` | `MouseEventHandler<HTMLSpanElement>` |  | Function to be executed when the icon is double-clicked. |
| `onMouseDown` | `MouseEventHandler<HTMLSpanElement>` |  | Function to be executed when the icon is pressed. |
| `shouldStopPropagation` | `boolean` |  | Stops event propagation on click. |
| `size` | `number` |  | The size of the icon. |
| `tabIndex` | `number` |  | Optional tab index for the icon. |

