# EmojiInput

**Package:** `@chayns-components/emoji-input` (5.0.0-beta.1411)

## Code Example

```tsx
import React, { FC, useState } from 'react';
import { EmojiInput } from '@chayns-components/emoji-input';

const Component: FC = () => {
    const [value, setValue] = useState('');

    return <EmojiInput value={value} onInput={(event, originalText) => setValue(originalText)} />;
};

Component.displayName = 'Component';

export default Component;

```

## Props

| Name | Type | Required | Description |
|------|------|----------|-------------|
| `accessToken` | `string` |  | Access token of the logged-in user. Is needed to load and save the history of the emojis. |
| `height` | `CSSProperties['height']` |  | Sets the height of the input field to a fixed value. If this value is not set, the component will use the needed height until the maximum height is reached. |
| `inputId` | `string` |  | HTML id of the input element |
| `isDisabled` | `boolean` |  | Disables the input so that it cannot be changed anymore |
| `maxHeight` | `CSSProperties['maxHeight']` |  | Sets the maximum height of the input field. |
| `onBlur` | `FocusEventHandler<HTMLDivElement>` |  | Function that is executed when the input field loses focus. |
| `onCursorPositionChange` | `(position: number) => void` |  | Function to be executed when the cursor position is changed. |
| `onFocus` | `FocusEventHandler<HTMLDivElement>` |  | Function that is executed when the input field gets the focus. |
| `onInput` | `(event: ChangeEvent<HTMLDivElement>, originalText: string) => void` |  | Function that is executed when the text of the input changes. In addition to the original event, the original text is returned as second parameter, in which the internally used HTML elements have been converted back to BB codes. |
| `onKeyDown` | `KeyboardEventHandler<HTMLDivElement>` |  | Function that is executed when a key is pressed down. |
| `onPopupVisibilityChange` | `(isVisible: boolean) => void` |  | Function that is executed when the visibility of the popup changes. |
| `onPrefixElementRemove` | `() => void` |  | Function to be executed if the prefixElement is removed. |
| `personId` | `string` |  | Person id of the logged-in user. Is needed to load and save the history of the emojis. |
| `placeholder` | `string \| ReactElement` |  | Placeholder for the input field |
| `popupAlignment` | `PopupAlignment` |  | Sets the alignment of the popup to a fixed value. If this value is not set, the component calculates the best position on its own. Use the imported 'PopupAlignment' enum to set this value. |
| `prefixElement` | `string` |  | Element that is rendered before the input field but the placeholder is still visible. |
| `rightElement` | `ReactNode` |  | Element that is rendered inside the EmojiInput on the right side. |
| `shouldHidePlaceholderOnFocus` | `boolean` |  | Whether the placeholder should be shown after the input has focus. |
| `shouldPreventEmojiPicker` | `boolean` |  | Prevents the EmojiPickerPopup icon from being displayed |
| `value` | `string` | ✓ | The plain text value of the input field. Instead of HTML elements BB codes must be used at this point. These are then converted by the input field into corresponding HTML elements. |
| `ref` | `EmojiInputRef` |  |  |

## Types

### EmojiInputRef

```typescript
{ insertTextAtCursorPosition: unknown; replaceText: unknown; startProgress: unknown; stopProgress: unknown; focus: unknown; blur: unknown; }
```

### PopupAlignment

```typescript
{ TopLeft = 0, TopCenter = 1, TopRight = 2, BottomLeft = 3, BottomCenter = 4, BottomRight = 5 }
```

### ReplaceTextOptions

```typescript
{ editorElement: HTMLDivElement; searchText: string; pasteText: string; options?: ReplaceTextOptions; }
```

