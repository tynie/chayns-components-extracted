# HighlightSlider

**Package:** `@chayns-components/core` (5.0.0-beta.1411)

## Code Example

```tsx
import React, { FC, useState } from 'react';
import { HighlightSlider } from '@chayns-components/core';

const Component: FC = () => {
    const [currentIndex, setCurrentIndex] = useState(0);

    return (
        <HighlightSlider
            count={13}
            currentIndex={currentIndex}
            onIndexChange={(index) => setCurrentIndex(index)}
        />
    );
};

Component.displayName = 'Component';

export default Component;

```

## Props

| Name | Type | Required | Description |
|------|------|----------|-------------|
| `colors` | `HighlightSliderColors` |  | The Colors of the slider. |
| `count` | `number` | ✓ | The total number of sections, that should be displayed. |
| `currentIndex` | `number` | ✓ | The current index. |
| `duration` | `number` |  | The duration of the animation of a single item in seconds. |
| `onIndexChange` | `(index: number) => void` |  | Function to be executed if the index has changed. |

## Types

### HighlightSliderColors

```typescript
{ backgroundColor: string; fillColor: string; }
```

