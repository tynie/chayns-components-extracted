# SliderButton

**Package:** `@chayns-components/core` (5.0.0-beta.1411)

## Code Example

```tsx
import React, { FC } from 'react';
import { SliderButton, SliderButtonItem } from '@chayns-components/core';

const ITEMS: SliderButtonItem[] = [
    { id: 'montag', text: 'Mo.' },
    { id: 'dienstag', text: 'Di.' },
    { id: 'mittwoch', text: 'Mi.' },
    { id: 'donnerstag', text: 'Do.' },
    { id: 'freitag', text: 'Fr.' },
    { id: 'samstag', text: 'Sa.' },
    { id: 'sonntag', text: 'So.' },
];

const Component: FC = () => {
    return <SliderButton items={ITEMS} />;
};

Component.displayName = 'Component';

export default Component;

```

## Props

| Name | Type | Required | Description |
|------|------|----------|-------------|
| `isDisabled` | `boolean` |  | Whether the button is disabled and cannot be clicked anymore. |
| `isSecondary` | `boolean` |  | Displays the button in the secondary style. |
| `items` | `SliderButtonItem[]` | ✓ | The items that should be displayed in the slider button. |
| `onChange` | `(id: string) => void` |  | Function to be executed when a button is selected. The id of the selected button is passed as an argument. |
| `selectedButtonId` | `string` |  | The id of the button that should be selected. |

## Types

### SliderButtonItem

```typescript
{ id: string; text: string; }
```

