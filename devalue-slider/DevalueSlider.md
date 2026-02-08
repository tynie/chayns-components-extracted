# DevalueSlider

**Package:** `@chayns-components/devalue-slider` (5.0.0-beta.1411)

## Code Example

```tsx
import React, { FC } from 'react';
import { DevalueSlider } from '@chayns-components/devalue-slider';

const Component: FC = () => {
    return <DevalueSlider />;
};

Component.displayName = 'Component';

export default Component;

```

## Props

| Name | Type | Required | Description |
|------|------|----------|-------------|
| `backgroundColor` | `CSSProperties['backgroundColor']` |  | The basic color of the slider. This color is the background of the track before the slider is devalued. |
| `devalueBackgroundColor` | `CSSProperties['backgroundColor']` |  | The devalue color of the slider. This color fills the track from the left on user movement. This color is the background of the timer after the slider is devalued. |
| `devalueTime` | `Date` |  | If this slider was devalued, provide the time when it was devalued. This will show a timer. |
| `isDisabled` | `boolean` |  | Disables the slider and cancels any active drags. |
| `label` | `string` |  | The label of the slider. The default value is "EINLÖSEN" |
| `onChange` | `DevalueSliderOnChangeHandler` |  | This function is called when the slider value changes. With this function you can keep track of the movement of the slider. |
| `onComplete` | `DevalueSliderOnCompleteHandler` |  | This function is called when the slider is completed. The slider is completed when the user devalues the slider and the animation is completed. |
| `onDevalue` | `DevalueSliderOnDevalueHandler` |  | This function is called when the slider is devalued. |

## Types

### DevalueSliderOnChangeHandler

```typescript
DevalueSliderOnChangeHandler
```

### DevalueSliderOnCompleteHandler

```typescript
DevalueSliderOnCompleteHandler
```

### DevalueSliderOnDevalueHandler

```typescript
DevalueSliderOnDevalueHandler
```

### DevalueSliderOnDevalueHandlerResult

```typescript
DevalueSliderOnDevalueHandlerResult
```

