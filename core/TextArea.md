# TextArea

**Package:** `@chayns-components/core` (5.0.0-beta.1411)

## Code Example

```tsx
import React, { FC, useState } from 'react';
import { TextArea } from '@chayns-components/core';

const Component: FC = () => {
    const [value, setValue] = useState('');

    return <TextArea value={value} onChange={(e) => setValue(e.target.value)} />;
};

Component.displayName = 'Component';

export default Component;

```

## Props

| Name | Type | Required | Description |
|------|------|----------|-------------|
| `isDisabled` | `boolean` |  | Disables the text area so that it cannot be changed. |
| `isInvalid` | `boolean` |  | If true, the text area is marked as invalid |
| `maxHeight` | `CSSProperties['maxHeight']` |  | The maximum height of the text area. |
| `minHeight` | `CSSProperties['minHeight']` |  | The minimum height of the text area. |
| `onBlur` | `FocusEventHandler<HTMLTextAreaElement>` |  | Function that is executed when the text area loses focus. |
| `onChange` | `ChangeEventHandler<HTMLTextAreaElement>` |  | Function that is executed when the text of the text area changes. |
| `onFocus` | `FocusEventHandler<HTMLTextAreaElement>` |  | Function that is executed when the input field is focused |
| `onKeyDown` | `KeyboardEventHandler<HTMLTextAreaElement>` |  | Function that is executed when a letter is pressed |
| `placeholder` | `string \| ReactElement` |  | Placeholder for the text area field. |
| `rightElement` | `ReactElement` |  | An element that should be displayed on the right side of the Input. |
| `value` | `string` |  | Value if the text area should be controlled. |
| `ref` | `HTMLTextAreaElement` |  |  |

