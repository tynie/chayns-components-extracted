# ContentCard

**Package:** `@chayns-components/core` (5.0.0-beta.1411)

## Code Example

```tsx
import React, { FC } from 'react';
import { ContentCard } from '@chayns-components/core';

const Component: FC = () => {
    return <ContentCard>Lorem</ContentCard>;
};

Component.displayName = 'Component';

export default Component;

```

## Props

| Name | Type | Required | Description |
|------|------|----------|-------------|
| `children` | `ReactNode` |  | The content of the content card |
| `onClick` | `() => void` |  | The onClick event handler |
| `type` | `ContentCardType` |  | The type of the content card |

## Types

### ContentCardType

```typescript
{ Default = "default", Error = "error", Success = "success", Warning = "warning", SiteColor = "siteColor" }
```

