# SearchBox

**Package:** `@chayns-components/core` (5.0.0-beta.1411)

## Code Example

```tsx
import React, { ChangeEvent, FC } from 'react';
import { SearchBox, SearchBoxItems } from '@chayns-components/core';

const LISTS: SearchBoxItems[] = [
    {
        groupName: undefined,
        list: [
            {
                imageUrl: 'https://picsum.photos/200',
                id: '1',
                text: 'Pizza',
            },
            { imageUrl: 'https://picsum.photos/200', id: '2', text: 'Burger' },
            { imageUrl: 'https://picsum.photos/200', id: '3', text: 'Nudeln' },
            { imageUrl: 'https://picsum.photos/200', id: '4', text: 'Steak' },
            { imageUrl: 'https://picsum.photos/200', id: '5', text: 'Pommes' },
            { imageUrl: 'https://picsum.photos/200', id: '6', text: 'Reis' },
        ],
    },
];

const Component: FC = () => {
    const handleChange = (event: ChangeEvent<HTMLInputElement>) => {
        console.log(event.target.value);
    };

    return <SearchBox onChange={handleChange} lists={LISTS} shouldAddInputToList />;
};

Component.displayName = 'Component';

export default Component;

```

## Props

| Name | Type | Required | Description |
|------|------|----------|-------------|
| `container` | `Element` |  | The element where the content of the `ComboBox` should be rendered via React Portal. |
| `customFilter` | `(item: SearchBoxItem) => boolean` |  | An optional callback function to filter the elements to be displayed |
| `dropdownDirection` | `DropdownDirection` |  | The direction in which the dropdown should be displayed. By default, it is displayed below the input. |
| `hintText` | `string` |  | A text that should be displayed if no results are found. |
| `isInvalid` | `boolean` |  | If true, the input field is marked as invalid |
| `leftIcons` | `string[]` |  | An optional icon that is displayed inside the left side of the input. |
| `lists` | `SearchBoxItems[]` | ✓ | List of groups with items that can be searched. It is possible to give only one list; if multiple lists are provided, the 'group name' parameter becomes mandatory. |
| `onBlur` | `FocusEventHandler<HTMLInputElement>` |  | Function to be executed when the input lost focus. |
| `onChange` | `ChangeEventHandler<HTMLInputElement>` |  | Function to be executed when the input is changed. |
| `onKeyDown` | `KeyboardEventHandler<HTMLInputElement>` |  | Function that is executed when a letter is pressed |
| `onSelect` | `(item: SearchBoxItem) => void` |  | Function to be executed when an item is selected. |
| `placeholder` | `string` |  | The placeholder that should be displayed. |
| `presetValue` | `string` |  | Set an input for the search box - it is not an item of a list, just a string. |
| `selectedId` | `string` |  | Control the selected item. If you use this prop, make sure to update it when the user selects an item. |
| `shouldAddInputToList` | `boolean` | ✓ | If true, the value in the Input is displayed in the list. |
| `shouldHideFilterButtons` | `boolean` |  | If true, the filter buttons are hidden. |
| `shouldShowContentOnEmptyInput` | `boolean` |  | Whether the full list of items should be displayed if the input is empty. |
| `shouldShowRoundImage` | `boolean` |  | If true, the images of the items are displayed in a round shape. |
| `shouldShowToggleIcon` | `boolean` |  | Whether the icon to open and close the list should be displayed. |
| `tagInputSettings` | `TagInputSettings` |  | Settings for the TagInput. |
| `ref` | `SearchBoxRef` |  |  |

## Types

### DropdownDirection

```typescript
{ BOTTOM = 0, TOP = 1, BOTTOM_LEFT = 2, BOTTOM_RIGHT = 3, TOP_LEFT = 4, TOP_RIGHT = 5, LEFT = 6, RIGHT = 7 }
```

### SearchBoxItem

```typescript
{ text: string; id: string; imageUrl?: string; }
```

### SearchBoxItems

```typescript
{ groupName?: string; list: Array; }
```

### SearchBoxRef

```typescript
{ clear: VoidFunction; }
```

### Tag

```typescript
{ id: string; text: string; rightElement?: ReactNode; }
```

### TagInputSettings

```typescript
{ onAdd?: unknown; onRemove?: unknown; shouldAllowMultiple?: boolean; tags?: Array; }
```

