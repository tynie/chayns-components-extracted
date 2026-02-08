# List

**Package:** `@chayns-components/core` (5.0.0-beta.1411)

## Code Example

```tsx
import React, { FC } from 'react';
import { List, ListItem } from '@chayns-components/core';

const Component: FC = () => {
    return (
        <List>
            <ListItem title="Test 1" />
            <ListItem title="Test 2" />
            <ListItem title="Test 3" />
        </List>
    );
};

Component.displayName = 'Component';

export default Component;

```

## Props

| Name | Type | Required | Description |
|------|------|----------|-------------|
| `children` | `ReactNode` | ✓ | The items of the list |
| `isWrapped` | `boolean` |  | This value must be set for nested AccordionGroup components. This adjusts the style of the head and the padding of the content accordions. |

