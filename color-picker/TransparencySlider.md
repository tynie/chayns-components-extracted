# TransparencySlider

**Package:** `@chayns-components/color-picker` (5.0.0-beta.1411)

## Code Example

```tsx
import React, { FC } from 'react';
import { TransparencySlider } from '@chayns-components/color-picker';

const Component: FC = () => {
    return <TransparencySlider />;
};

Component.displayName = 'Component';

export default Component;

```

## Props

| Name | Type | Required | Description |
|------|------|----------|-------------|
| `color` | `string` |  | The color that should be selected. |
| `onChange` | `(color: string) => void` |  | Function that will be executed when the opacity is changed. |
| `onEnd` | `(color: string) => void` |  | Function that will be executed when the opacity is ending to change. |
| `onStart` | `(color: string) => void` |  | Function that will be executed when the opacity is starting to change. |

