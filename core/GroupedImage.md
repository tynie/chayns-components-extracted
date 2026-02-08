# GroupedImage

**Package:** `@chayns-components/core` (5.0.0-beta.1411)

## Code Example

```tsx
import React, { FC } from 'react';
import { GroupedImage } from '@chayns-components/core';

const IMAGES = [
    'https://tsimg.cloud/77896-21884/8aee1a304297729a4542b97325940a656a3da8f2.png',
    'https://tsimg.cloud/77896-21884/54a117f35e5fb57520e64471461af5491c0eff06.png',
];

const Component: FC = () => {
    return <GroupedImage images={IMAGES} />;
};

Component.displayName = 'Component';

export default Component;

```

## Props

| Name | Type | Required | Description |
|------|------|----------|-------------|
| `cornerElement` | `ReactNode` |  | Optional Element to display in the right corner of the image |
| `cornerImage` | `string` |  | Optional image to display in the bottom right corner of the grouped image. |
| `height` | `number` |  | Height of the grouped image container. |
| `imageBackground` | `CSSProperties['background']` |  | Background for the single images. |
| `images` | `string[]` | ✓ | Array of image URLs to display in the grouped image. If only one image is provided, it will be displayed as a full image. |
| `onClick` | `MouseEventHandler<HTMLDivElement>` |  | Optional click handler for the grouped image. |
| `onImageError` | `(event: SyntheticEvent<HTMLImageElement, Event>, index: number) => void` |  | Optional handler for image load errors. |
| `shouldPreventBackground` | `boolean` |  | Whether to prevent the background of the images from being set. |
| `shouldShowRoundImage` | `boolean` |  | Whether to show the images in a round shape. |

