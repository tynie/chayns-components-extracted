# EmojiPickerPopup

**Package:** `@chayns-components/emoji-input` (5.0.0-beta.1411)

## Code Example

```tsx
import React, { FC } from 'react';
import { EmojiPickerPopup } from '@chayns-components/emoji-input';

const Component: FC = () => {
    const handleEmojiSelect = (emoji: string) => {
        console.log('Emoji:', emoji);
    };

    return <EmojiPickerPopup onSelect={handleEmojiSelect} />;
};

Component.displayName = 'Component';

export default Component;

```

## Props

| Name | Type | Required | Description |
|------|------|----------|-------------|
| `accessToken` | `string` |  | Access token of the logged-in user. Is needed to load and save the history of the emojis. |
| `onPopupVisibilityChange` | `(isVisible: boolean) => void` |  | Function that is executed when the visibility of the popup changes. |
| `onSelect` | `(emoji: string) => void` | ✓ | Function executed when an emoji is selected in the popup |
| `personId` | `string` |  | Person id of the logged-in user. Is needed to load and save the history of the emojis. |

