# RadioButton

**Package:** `@chayns-components/core` (5.0.0-beta.1411)

## Code Example

```tsx
import React, { FC } from 'react';
import { RadioButtonGroup, RadioButton } from '@chayns-components/core';

const Component: FC = () => {
    return (
        <RadioButtonGroup>
            <RadioButton id="1" />
            <RadioButton id="2" />
            <RadioButton id="3">Lorem</RadioButton>
        </RadioButtonGroup>
    );
};

Component.displayName = 'Component';

export default Component;

```

## Props

| Name | Type | Required | Description |
|------|------|----------|-------------|
| `children` | `ReactNode` |  | The children that should be displayed after the RadioButton is checked. |
| `id` | `string` | ✓ | The id of the radio button. |
| `isDisabled` | `boolean` |  | whether the RadioButton should be shown. |
| `label` | `ReactNode` |  | The label that should be displayed next to the radio button. |
| `rightElement` | `ReactNode` |  | An element that should be displayed on the right side of the label. |
| `shouldShowCentered` | `boolean` |  | Whether the RadioButton should be displayed centered to the label or at the top |
| `shouldShowRightElementOnlyOnChecked` | `boolean` |  | Whether the rightElement should only be displayed when the RadioButton is checked |

