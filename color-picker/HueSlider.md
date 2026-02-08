# HueSlider

**Package:** `@chayns-components/color-picker` (5.0.0-beta.1411)

## Code Example

```tsx
import React, { FC } from 'react';
import { HueSlider } from '@chayns-components/color-picker';

const Component: FC = () => {
    return <HueSlider />;
};

Component.displayName = 'Component';

export default Component;

```

## Props

| Name | Type | Required | Description |
|------|------|----------|-------------|
| `color` | `CSSProperties['color']` |  | The color that should be selected. |
| `onChange` | `(rgb: CSSProperties['color'], hsl: CSSProperties['color']) => void` |  | Function that will be executed when the color is changed. |
| `onEnd` | `(rgb: CSSProperties['color'], hsl: CSSProperties['color']) => void` |  | Function that will be executed when the color is ending to change. |
| `onStart` | `(rgb: CSSProperties['color'], hsl: CSSProperties['color']) => void` |  | Function that will be executed when the color is starting to change. |
| `opacity` | `number` |  | The opacity of the Color. Is used if the color has no opacity value. |

