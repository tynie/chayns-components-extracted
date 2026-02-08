# ComboBox

**Package:** `@chayns-components/core` (5.0.0-beta.1411)

## Code Example

```tsx
import React, { FC } from 'react';
import { ComboBox, ComboBoxItems } from '@chayns-components/core';

const LIST: ComboBoxItems[] = [
    {
        list: [
            {
                text: 'Margherita',
                value: 1,
            },
            {
                text: 'Thunfisch',
                value: 2,
            },
        ],
    },
];

const Component: FC = () => {
    return <ComboBox lists={LIST} placeholder="Pizza auswählen" />;
};

Component.displayName = 'Component';

export default Component;

```

## Props

| Name | Type | Required | Description |
|------|------|----------|-------------|
| `bodyWidth` | `number` |  | The width of the body. |
| `container` | `Element` |  | The element where the content of the `ComboBox` should be rendered via React Portal. |
| `direction` | `DropdownDirection` |  | The direction in which the combobox should open. |
| `inputValue` | `string` |  | The value of the optional input. |
| `isDisabled` | `boolean` |  | Whether the combobox should be disabled. |
| `lists` | `ComboBoxItems[]` | ✓ | The list of the items that should be displayed. |
| `maxHeight` | `number` |  | The maximum height of the combobox content. |
| `onInputBlur` | `FocusEventHandler<HTMLInputElement>` |  | Function to be executed when the optional input lost its focus. |
| `onInputChange` | `ChangeEventHandler<HTMLInputElement>` |  | Function to be executed when the value of the optional input is changed. |
| `onInputFocus` | `FocusEventHandler<HTMLInputElement>` |  | Function to be executed when the optional input gets its focus. |
| `onSelect` | `(comboboxItem?: ComboBoxItem) => Promise<boolean> \| boolean \| void` |  | Function that should be executed when an item is selected. If the function returns false, the item will not be selected. |
| `placeholder` | `string` | ✓ | A text that should be displayed when no item is selected. |
| `prefix` | `string` |  | A prefix that should be displayed before the placeholder. |
| `prefixMinWidth` | `number` |  | Optional min width for the prefix element. |
| `selectedItem` | `ComboBoxItem` |  | An item that should be preselected. |
| `shouldDropDownUseMaxItemWidth` | `boolean` |  | If true, the dropdown will use the maximum width of the items. |
| `shouldShowBigImage` | `boolean` |  | If true, the images of the items are displayed in a bigger shape. This prop will automatically be set to true if the subtext of an item is given. |
| `shouldShowClearIcon` | `boolean` |  | If true, a clear icon is displayed at the end of the combo box if an item is selected. |
| `shouldShowRoundImage` | `boolean` |  | If true, the images of the items are displayed in a round shape. |
| `shouldShowTransparentBackground` | `boolean` |  | Whether the background should be transparent. |
| `shouldUseCurrentItemWidth` | `boolean` |  | Whether the width of the ComboBox should be the width of the current item. |
| `shouldUseFullWidth` | `boolean` |  | Whether the width of the 'ComboBox' should be the width of the parent or of the widest item. |
| `ref` | `ComboBoxRef` |  |  |

## Types

### ComboBoxItem

```typescript
{ icons?: Array; imageBackground?: string | number | string & unknown; imageUrl?: string; isDisabled?: boolean; rightElement?: ReactNode; subtext?: string; suffixElement?: ReactNode; text: string; value: string | number; textStyles?: ComboBoxTextStyles; }
```

### ComboBoxItems

```typescript
{ groupName?: string; list: Array; shouldShowRoundImage?: boolean; }
```

### ComboBoxRef

```typescript
{ hide: VoidFunction; show: VoidFunction; }
```

### ComboBoxTextStyles

```typescript
{ tagName?: keyof ReactHTML; styles?: Properties & unknown; className?: string; }
```

### DropdownDirection

```typescript
{ BOTTOM = 0, TOP = 1, BOTTOM_LEFT = 2, BOTTOM_RIGHT = 3, TOP_LEFT = 4, TOP_RIGHT = 5, LEFT = 6, RIGHT = 7 }
```

