# FileSelect

**Package:** `@chayns-components/core` (5.0.0-beta.1411)

## Code Example

```tsx
import React, { FC } from 'react';
import { FileSelect } from '@chayns-components/core';

const Component: FC = () => {
    return <FileSelect />;
};

Component.displayName = 'Component';

export default Component;

```

## Props

| Name | Type | Required | Description |
|------|------|----------|-------------|
| `fileSelectionIcons` | `string[]` |  | An array of icons that should be displayed inside the FileInput |
| `fileSelectionPlaceholder` | `string` |  | The text that should be displayed inside the FileInput. |
| `fileTypes` | `string` |  | The filetypes that could be selected. Example for multiple types: 'image/*, video/*'. |
| `imageSelectIcons` | `string[]` |  | The icon of the image selection. |
| `imageSelectPlaceholder` | `string` |  | If set, pictures can be select via Pixabay. |
| `isDisabled` | `boolean` |  | Whether the FileInput is disabled. |
| `maxFiles` | `number` |  | The maximum amount of Files that can be uploaded. |
| `maxFileSizeInMB` | `number` |  | The maximum size of a file in MB. |
| `onAdd` | `(files: File[] \| UploadedFile[]) => void` |  | A function to be executed when files are added. |
| `shouldPreventImageUpload` | `boolean` |  | Whether the image upload should be prevented. |

## Types

### UploadedFile

```typescript
{ url: string; size?: number; name?: string; }
```

