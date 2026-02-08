# AnimatedNumber

**Package:** `@chayns-components/core` (5.0.0-beta.1411)

## Code Example

```tsx
import React, { FC } from 'react';
import { AnimatedNumber } from '@chayns-components/core';

const Component: FC = () => {
    return <AnimatedNumber value={420} />;
};

Component.displayName = 'Component';

export default Component;

```

## Props

| Name | Type | Required | Description |
|------|------|----------|-------------|
| `delay` | `number` |  | Start delay of the animation in seconds. |
| `duration` | `number` |  | Total duration of the animation in seconds. |
| `ease` | `Ease` |  | Easing curve of the animation (e.g., cubic-bezier like [0.16, 1, 0.3, 1] or predefined easings). Controls how the animation accelerates/decelerates. |
| `format` | `(n: number) => string` |  | Custom formatter for the displayed value. If provided, it overrides locale/toLocaleString and round. Example: (n) => `${Math.round(n)} points` |
| `locale` | `string` |  | Locale used by toLocaleString when no custom formatter is provided. |
| `onComplete` | `() => void` |  | Callback invoked when the animation completes. |
| `round` | `(n: number) => number` |  | Custom rounding function when no custom formatter is provided. Default: Math.round |
| `startFrom` | `number` |  | Starting value for the animation. Default: 0 |
| `value` | `number` | ✓ | Target value to animate to. |

## Types

### Ease

```typescript
string | [number, number, number, number] | unknown
```

