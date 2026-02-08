# Truncation

**Package:** `@chayns-components/core` (5.0.0-beta.1411)

## Code Example

```tsx
import React, { FC } from 'react';
import { Truncation } from '@chayns-components/core';

const Component: FC = () => {
    return (
        <Truncation>
            <div>Lorem</div>
        </Truncation>
    );
};

Component.displayName = 'Component';

export default Component;

```

## Props

| Name | Type | Required | Description |
|------|------|----------|-------------|
| `children` | `ReactElement` | ✓ | The elements that should be expanding or collapsing. |
| `clampPosition` | `ClampPosition` |  | The position of the clamp. |
| `collapsedHeight` | `number` |  | The height of the children Element in it`s collapsed state. |
| `isOpen` | `boolean` |  | If set to true, the content is exposed. |
| `lessLabel` | `string` |  | A text that should be displayed if the content is expanded. |
| `moreLabel` | `string` |  | A text that should be displayed if the content is collapsed. |
| `onChange` | `(event: MouseEvent<HTMLAnchorElement>, isOpen: boolean) => void` |  | Function to be executed when the component is expanding or collapsing. |

## Types

### ClampPosition

```typescript
{ Right = 0, Middle = 1, Left = 2 }
```

