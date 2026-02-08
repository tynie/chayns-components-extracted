# Checkbox

**Package:** `@chayns-components/core` (5.0.0-beta.1411)

## Code Example

```tsx
import React, { FC } from 'react';
import { Button } from '@chayns-components/core';

const Component: FC = () => {
    const handleClick = () => {
        console.log('Click');
    };

    return <Button onClick={handleClick}>Click me!</Button>;
};

Component.displayName = 'Component';

export default Component;

```

## Props

| Name | Type | Required | Description |
|------|------|----------|-------------|
| `children` | `ReactElement \| string` |  | Text for checkbox or switch |
| `isChecked` | `boolean` |  | Indicates whether the checkbox or switch is selected |
| `isDisabled` | `boolean` |  | Disables the checkbox or switch so it cannot be toggled |
| `labelClassName` | `string` |  | Classname for the label |
| `onChange` | `ChangeEventHandler<HTMLInputElement>` |  | Function to be executed if the checked value changes |
| `shouldChangeOnLabelClick` | `boolean` |  | Whether the label should change the state of the checkbox |
| `shouldShowAsSwitch` | `boolean` |  | Changes the design to use switch instead of checkbox |
| `shouldShowCentered` | `boolean` |  | Whether the Checkbox should be displayed centered to the label or at the top |

