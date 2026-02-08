# Badge

**Package:** `@chayns-components/core` (5.0.0-beta.1411)

## Code Example

```tsx
import React, { FC } from 'react';
import { Badge } from '@chayns-components/core';

const Component: FC = () => {
    return <Badge>13</Badge>;
};

Component.displayName = 'Component';

export default Component;

```

## Props

| Name | Type | Required | Description |
|------|------|----------|-------------|
| `backgroundColor` | `CSSProperties['backgroundColor']` |  | The background color of the badge. |
| `children` | `ReactNode` |  | The content of the badge. |
| `className` | `string` |  | Additional class names for the badge element. |
| `design` | `BadgeDesign` |  | The design of the Badge. |
| `fontColor` | `CSSProperties['color']` |  | The font color of the badge. |
| `onClick` | `MouseEventHandler` |  | Function to be executed when the badge is clicked. |
| `size` | `BadgeSize` |  | The size of the badge. |

## Types

### BadgeDesign

```typescript
{ DEFAULT = "default", BORDER = "border" }
```

### BadgeSize

```typescript
{ SMALL = "small", DEFAULT = "default" }
```

