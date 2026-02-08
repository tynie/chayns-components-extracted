# ListItemContent

**Package:** `@chayns-components/core` (5.0.0-beta.1411)

## Code Example

```tsx
import React, { FC } from 'react';
import { List, ListItem, ListItemContent } from '@chayns-components/core';

const Component: FC = () => {
    return (
        <List>
            <ListItem title="Test 1">
                <ListItemContent>Lorem</ListItemContent>
            </ListItem>
        </List>
    );
};

Component.displayName = 'Component';

export default Component;

```

## Props

| Name | Type | Required | Description |
|------|------|----------|-------------|
| `children` | `ReactNode` | ✓ | The Elements that should be shown inside the LIstItemContent |

