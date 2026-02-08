# FileInput

**Package:** `@chayns-components/core` (5.0.0-beta.1411)

## Code Example

```tsx
import React, { FC } from 'react';
import { FileInput } from '@chayns-components/core';

const Component: FC = () => {
    return <FileInput />;
};

Component.displayName = 'Component';

export default Component;

```

## Props

| Name | Type | Required | Description |
|------|------|----------|-------------|
| `files` | `FileListItem[]` |  | Already uploaded files to display. |
| `fileSelectionIcons` | `string[]` |  | An array of icons that should be displayed inside the FileInput |
| `fileSelectionPlaceholder` | `string` |  | The text that should be displayed inside the FileInput. |
| `fileTypes` | `string` |  | The filetypes that could be selected. Example for multiple types: 'image/*, video/*'. |
| `imageSelectIcons` | `string[]` |  | The icon of the image selection. |
| `imageSelectPlaceholder` | `string` |  | If set, pictures can be select via Pixabay. |
| `isDisabled` | `boolean` |  | Whether the FileInput is disabled. |
| `maxFiles` | `number` |  | The maximum amount of Files that can be uploaded. |
| `maxFileSizeInMB` | `number` |  | The maximum size of a file in MB. |
| `onAdd` | `(files: File[] \| UploadedFile[]) => void` |  | A function to be executed when files are added. |
| `onMaxFilesReached` | `() => void` |  | Function to be executed when the maximum amount of Files are reached. |
| `onRemove` | `(file: File \| FileListItem \| UploadedFile) => void` |  | A function to be executed when a file is removed. |
| `shouldPreventImageUpload` | `boolean` |  | Whether the image upload should be prevented. |
| `ref` | `FileInputRef` |  |  |

## Types

### FileInputRef

```typescript
FileInputRef
```

### FileListItem

```typescript
{ id: string; name: string; size?: number; mimeType: string; }
```

### UploadedFile

```typescript
{ url: string; size?: number; name?: string; }
```

