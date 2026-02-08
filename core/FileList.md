# FileList

**Package:** `@chayns-components/core` (5.0.0-beta.1411)

## Code Example

```tsx
import React, { FC } from 'react';
import { FileList } from '@chayns-components/core';

const Component: FC = () => {
    return <FileList />;
};

Component.displayName = 'Component';

export default Component;

```

## Props

| Name | Type | Required | Description |
|------|------|----------|-------------|
| `files` | `FileListItem[]` |  | Already uploaded files to display. |
| `onRemove` | `(id: FileListItem['id']) => void` |  | A function to be executed when a file is removed. |

## Types

### FileListItem

```typescript
{ id: string; name: string; size?: number; mimeType: string; }
```

