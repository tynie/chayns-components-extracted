# SelectButton

**Package:** `@chayns-components/core` (5.0.0-beta.1411)

## Code Example

```tsx
import React, { FC } from 'react';
import { SelectButton, SelectButtonItem } from '@chayns-components/core';

const LIST: SelectButtonItem[] = [
    { text: 'Salami', id: 1 },
    { text: 'Thunfisch', id: 2 },
    { text: 'Döner', id: 3 },
];

const Component: FC = () => {
    return <SelectButton buttonText="Auswählen" list={LIST} />;
};

Component.displayName = 'Component';

export default Component;

```

## Props

| Name | Type | Required | Description |
|------|------|----------|-------------|
| `additionalText` | `string` |  | Text used when there are more selected items than maxDisplayedItems. '##count##' will be displayed with the additional count. |
| `buttonText` | `string` | ✓ | The text that should be displayed inside the button. |
| `isDisabled` | `boolean` |  | Whether the button should be disabled. |
| `list` | `SelectButtonItem[]` | ✓ | A list of item that could be selected. |
| `maxDisplayedItems` | `number` |  | The maximum number of items displayed in the button text. |
| `onSelect` | `(ids: (number \| string)[]) => void` |  | Function to be executed after an item is selected. |
| `selectAllText` | `string` |  | If a string is given and `shouldAllowMultiSelect` is true, the dialog displays a checkbox to select all items at once. |
| `selectedItemIds` | `(number \| string)[]` |  | The id of an item that should be preselected. |
| `shouldAllowMultiSelect` | `boolean` |  | Whether more than one item should be selectable. |
| `shouldShowButtonTextWithSelection` | `boolean` |  | Whether the button text should be displayed also if items are selected. |
| `shouldShowSearch` | `boolean` |  | Whether the search should be displayed inside the dialog. |
| `title` | `string` |  | The title of the dialog. |

## Types

### SelectButtonItem

```typescript
{ text: string; id: string | number; }
```

