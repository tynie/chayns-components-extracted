# ExpandableContent

**Package:** `@chayns-components/core` (5.0.0-beta.1411)

## Code Example

```tsx
import React, { FC } from 'react';
import { ExpandableContent } from '@chayns-components/core';

const Component: FC = () => {
    return <ExpandableContent isOpen>Lorem</ExpandableContent>;
};

Component.displayName = 'Component';

export default Component;

```

## Props

| Name | Type | Required | Description |
|------|------|----------|-------------|
| `children` | `ReactNode` | ✓ | The children that should be animated. |
| `isOpen` | `boolean` | ✓ | Whether the content is expanded. |
| `startDelay` | `number` |  | An optional start delay. |

