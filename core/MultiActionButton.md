# MultiActionButton

**Package:** `@chayns-components/core` (5.0.0-beta.1411)

## Code Example

```tsx
import React, { FC } from 'react';
import {
    MultiActionButton,
    MultiActionButtonStatusType,
} from '@chayns-components/core';

const Component: FC = () => {
    return (
        <MultiActionButton
            primaryAction={{
                icon: 'fa fa-pen',
                label: 'Chatten',
                onClick: () => console.log('Primary'),
            }}
            secondaryAction={{
                icon: 'fa fa-microphone',
                label: 'Mitschnitt starten',
                onClick: () => console.log('Secondary'),
                status: {
                    type: MultiActionButtonStatusType.Pulse,
                    pulseColor: 'rgba(255, 0, 0, 0.6)',
                },
            }}
        />
    );
};

Component.displayName = 'Component';

export default Component;

```

## Props

| Name | Type | Required | Description |
|------|------|----------|-------------|
| `className` | `string` |  | Additional class name for the wrapper element. |
| `extendedTimeoutMs` | `number` |  | Auto-reset timeout for the extended state (ms). |
| `isCollapsed` | `boolean` |  | Whether the button is collapsed to a single icon. |
| `isDisabled` | `boolean` |  | Whether the whole control is disabled. |
| `primaryAction` | `MultiActionButtonAction & { label: ReactNode }` | ✓ | Primary action configuration. |
| `secondaryAction` | `MultiActionButtonAction` |  | Secondary action configuration. |
| `width` | `number \| MotionValue<number>` |  | Optional width override for the whole button. |

## Types

### MultiActionButtonAction

```typescript
MultiActionButtonAction
```

