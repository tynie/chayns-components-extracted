# Slider

**Package:** `@chayns-components/core` (5.0.0-beta.1411)

## Code Example

```tsx
import React, { FC } from 'react';
import { Slider } from '@chayns-components/core';

const Component: FC = () => {
    return <Slider maxValue={100} minValue={0} />;
};

Component.displayName = 'Component';

export default Component;

```

## Props

| Name | Type | Required | Description |
|------|------|----------|-------------|
| `interval` | `SliderInterval` |  | The current interval of the slider. |
| `isDisabled` | `boolean` |  | Disables the slider, preventing user interaction. |
| `maxEnabledValue` | `number` |  | The maximum enabled value of the slider. |
| `maxValue` | `number` | ✓ | The maximum value of the slider. |
| `minEnabledValue` | `number` |  | The minimum enabled value of the slider. |
| `minValue` | `number` | ✓ | The minimum value of the slider. |
| `onChange` | `(value?: number, interval?: SliderInterval) => void` |  | Callback function that is called when the slider value changes. |
| `onSelect` | `(value?: number, interval?: SliderInterval) => void` |  | Callback function that is called when the slider selection is finalized. |
| `shouldHighlightSteps` | `boolean` |  | Indicates whether the slider should highlight steps. |
| `shouldShowThumbLabel` | `boolean` |  | Indicates whether the slider should show a label on the thumb. |
| `step` | `number` |  | The step size for the slider. |
| `thumbLabelFormatter` | `(value: number) => string` |  | A function to format the thumb label. |
| `value` | `number` |  | The current value of the slider. |

## Types

### SliderInterval

```typescript
{ maxValue: number; minValue: number; }
```

