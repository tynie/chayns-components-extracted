# SmallWaitCursor

**Package:** `@chayns-components/core` (5.0.0-beta.1411)

## Code Example

```tsx
import React, { FC } from 'react';
import { SmallWaitCursor } from '@chayns-components/core';

const Component: FC = () => {
    return <SmallWaitCursor />;
};

Component.displayName = 'Component';

export default Component;

```

## Props

| Name | Type | Required | Description |
|------|------|----------|-------------|
| `color` | `string` |  |  |
| `shouldHideBackground` | `boolean` |  |  |
| `shouldHideWaitCursor` | `boolean` |  |  |
| `size` | `SmallWaitCursorSize \| number` |  |  |
| `speed` | `SmallWaitCursorSpeed` |  |  |

## Types

### SmallWaitCursorSize

```typescript
{ Small = 16, Medium = 30 }
```

### SmallWaitCursorSpeed

```typescript
{ Slow = 1.5, Medium = 1, Fast = 0.5 }
```

