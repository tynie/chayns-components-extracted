# Gallery

**Package:** `@chayns-components/gallery` (5.0.0-beta.1411)

## Code Example

```tsx
import React, { FC } from 'react';
import { Gallery } from '@chayns-components/gallery';

const Component: FC = () => {
    return <Gallery />;
};

Component.displayName = 'Component';

export default Component;

```

## Props

| Name | Type | Required | Description |
|------|------|----------|-------------|
| `allowDragAndDrop` | `boolean` |  | Whether drag and drop is allowed or not |
| `doubleFileDialogMessage` | `string` |  | The message that should be displayed if a File is already given. |
| `fileMinWidth` | `number` |  | The minimum width of a file in the edit mode |
| `files` | `FileItem[]` |  | Images and videos which should be displayed |
| `isEditMode` | `boolean` |  | Whether images and videos can be edited |
| `maxFiles` | `number` |  | The maximum amount of images and videos that can be uploaded. |
| `onAdd` | `(file: FileItem) => void` |  | Function to be executed when files are added and uploaded |
| `onFileCountChange` | `(fileCount: number) => void` |  | Function to be executed when the count of files are changed. Needed to check if all files are uploaded |
| `onRemove` | `(file: FileItem) => void` |  | Function to be executed when a file is removed |
| `viewMode` | `GalleryViewMode` |  | The mode how the images should be displayed. |

## Types

### FileItem

```typescript
{ file: Video | Image; id?: string; }
```

### GalleryViewMode

```typescript
{ SQUARE = 0, GRID = 1 }
```

### Image

```typescript
{ id?: string; url: string; meta?: Meta; ratio?: number; }
```

### Meta

```typescript
{ preview: string; width: string; height: string; }
```

### Video

```typescript
{ id: string; originalVideoQuality?: string; thumbnailUrl: string; url: string; ratio?: number; }
```

