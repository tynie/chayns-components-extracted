# EmojiPicker

**Package:** `@chayns-components/emoji-input` (5.0.0-beta.1411)

## Code Example

```tsx
import React, { FC } from 'react';
import { EmojiPicker } from '@chayns-components/emoji-input';

const Component: FC = () => {
    const handleEmojiSelect = (emoji: string) => {
        console.log('Emoji:', emoji);
    };

    return <EmojiPicker onSelect={handleEmojiSelect} />;
};

Component.displayName = 'Component';

export default Component;

```

## Props

| Name | Type | Required | Description |
|------|------|----------|-------------|
| `accessToken` | `string` |  | Access token of the logged-in user. Is needed to load and save the history of the emojis. |
| `onSelect` | `(emoji: string) => void` | ✓ | Function executed when an emoji is selected in the popup |
| `personId` | `string` |  | Person id of the logged-in user. Is needed to load and save the history of the emojis. |

