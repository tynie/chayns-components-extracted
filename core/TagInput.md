# TagInput

**Package:** `@chayns-components/core` (5.0.0-beta.1411)

## Code Example

```tsx
import React, { FC, useState } from 'react';
import { Tag, TagInput } from '@chayns-components/core';

const Component: FC = () => {
    const [tags, setTags] = useState<Tag[]>([]);

    const handleAdd = (tag: Tag) => {
        setTags((prevState) => [...prevState, tag]);
    };

    const handleRemove = (id: Tag['id']) => {
        setTags((prevState) => prevState.filter((tag) => tag.id !== id));
    };

    return <TagInput tags={tags} onAdd={handleAdd} onRemove={handleRemove} />;
};

Component.displayName = 'Component';

export default Component;

```

## Props

| Name | Type | Required | Description |
|------|------|----------|-------------|
| `leftElement` | `ReactNode` |  | An element that should be displayed on the left side of the input. |
| `onAdd` | `(tag: Tag) => Promise<boolean> \| boolean \| void` |  | Function to be executed when a tag is added. |
| `onBlur` | `FocusEventHandler` |  | Function to be executed when the input is blurred. |
| `onChange` | `ChangeEventHandler<HTMLInputElement>` |  | Function to be executed when the value of the input is changed. |
| `onFocus` | `FocusEventHandler` |  | Function to be executed when the input is focused. |
| `onRemove` | `(id: string) => void` |  | Function to be executed when a tag is removed. |
| `placeholder` | `string` |  | The placeholder that should be displayed. |
| `shouldAllowMultiple` | `boolean` |  | Whether multiple tags should be allowed. |
| `shouldPreventEnter` | `boolean` |  | Whether the enter key should be prevented. |
| `tags` | `Tag[]` |  | The tags that should be displayed. |
| `ref` | `TagInputRef` |  |  |

## Types

### Tag

```typescript
{ id: string; text: string; rightElement?: ReactNode; }
```

### TagInputRef

```typescript
{ blur: unknown; getUnsavedTagText: string; resetValue: unknown; }
```

