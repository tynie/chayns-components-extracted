# SearchInput

**Package:** `@chayns-components/core` (5.0.0-beta.1411)

## Code Example

```tsx
import React, { ChangeEvent, FC } from 'react';
import { SearchInput } from '@chayns-components/core';

const Component: FC = () => {
    const handleChange = (event: ChangeEvent<HTMLInputElement>) => {
        console.log(event.target.value);
    };

    return <SearchInput onChange={handleChange} />;
};

Component.displayName = 'Component';

export default Component;

```

## Props

| Name | Type | Required | Description |
|------|------|----------|-------------|
| `iconColor` | `CSSProperties['color']` |  | Color of the icon |
| `isActive` | `boolean` |  | Force the active state of the input and override the internal state |
| `onActiveChange` | `(isActive: boolean) => void` |  | Function that is executed when the active state of the input changes |
| `onChange` | `ChangeEventHandler<HTMLInputElement>` | ✓ | Function that is executed when the text of the input changes |
| `onKeyDown` | `(event: KeyboardEvent<HTMLInputElement>) => void` |  | Function that is executed when a key is pressed |
| `placeholder` | `string` |  | Placeholder for the input field |
| `shouldUseAbsolutePositioning` | `boolean` |  | Whether the SearchInput should be positioned absolute. |
| `size` | `InputSize` |  | The size of the input field |
| `value` | `string` |  | Value if the input field should be controlled |
| `width` | `number` |  | The width of the parent. |
| `ref` | `InputRef` |  |  |

## Types

### InputRef

```typescript
{ focus: VoidFunction; blur: VoidFunction; }
```

### InputSize

```typescript
{ Small = "small", Medium = "medium" }
```

