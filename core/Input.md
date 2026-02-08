# Input

**Package:** `@chayns-components/core` (5.0.0-beta.1411)

## Code Example

```tsx
import React, { FC, useState } from 'react';
import { Input } from '@chayns-components/core';

const Component: FC = () => {
    const [value, setValue] = useState('');

    return <Input value={value} onChange={(e) => setValue(e.target.value)} />;
};

Component.displayName = 'Component';

export default Component;

```

## Props

| Name | Type | Required | Description |
|------|------|----------|-------------|
| `autoComplete` | `AutoComplete` |  | Defines the auto Complete of the input |
| `disabledHint` | `string` |  | If set and the input is disabled, the input will display a tooltip with this message. |
| `id` | `string` |  | The id of the input |
| `inputMode` | `InputMode` |  | Defines the input mode of the input |
| `isDisabled` | `boolean` |  | Disables the input so that it cannot be changed anymore |
| `isInvalid` | `boolean` |  | If true, the input field is marked as invalid |
| `leftElement` | `ReactNode` |  | An element to be displayed on the left side of the input field |
| `onBlur` | `FocusEventHandler<HTMLInputElement>` |  | Function that is executed when the input field loses focus |
| `onChange` | `ChangeEventHandler<HTMLInputElement>` |  | Function that is executed when the text of the input changes |
| `onFocus` | `FocusEventHandler<HTMLInputElement>` |  | Function that is executed when the input field is focused |
| `onKeyDown` | `KeyboardEventHandler<HTMLInputElement>` |  | Function that is executed when a letter is pressed |
| `onPaste` | `(event: ClipboardEvent<HTMLInputElement>) => void` |  | Function that is executed when content is pasted into the input field |
| `placeholder` | `ReactNode` |  | Placeholder for the input field |
| `rightElement` | `ReactElement` |  | An element that should be displayed on the right side of the Input. |
| `shouldPreventPlaceholderAnimation` | `boolean` |  | Whether the placeholder animation should be prevented. |
| `shouldRemainPlaceholder` | `boolean` |  | Whether the placeholder should remain at its position if a value is typed. |
| `shouldShowCenteredContent` | `boolean` |  | Whether the content should be displayed centered inside the input. |
| `shouldShowClearIcon` | `boolean` |  | If true, a clear icon is displayed at the end of the input field |
| `shouldShowOnlyBottomBorder` | `boolean` |  | Whether only the bottom border should be displayed |
| `shouldShowTransparentBackground` | `boolean` |  | Whether the background should be transparent. |
| `shouldUseAutoFocus` | `boolean` |  | If true, the input field is focused when the component is mounted |
| `size` | `InputSize` |  | The size of the input field |
| `type` | `HTMLInputTypeAttribute` |  | Input type set for an input element (e.g. 'text', 'number' or 'password') |
| `value` | `string` |  | Value if the input field should be controlled |
| `ref` | `InputRef` |  |  |

## Types

### AutoComplete

```typescript
"name" | "email" | "tel" | "url" | "on" | "off" | "username" | "new-password" | "current-password" | "street-address" | "postal-code" | "country"
```

### InputMode

```typescript
"text" | "none" | "search" | "email" | "tel" | "url" | "numeric" | "decimal"
```

### InputRef

```typescript
{ focus: VoidFunction; blur: VoidFunction; }
```

### InputSize

```typescript
{ Small = "small", Medium = "medium" }
```

