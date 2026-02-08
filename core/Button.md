# Button

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
| `buttonDesign` | `number` |  | Optional button design override. |
| `children` | `ReactNode` |  | The label of the button. |
| `className` | `string` |  | Additional class names for the button element. |
| `icon` | `string` |  | An icon that is displayed on the left-hand side of the button text. |
| `isDisabled` | `boolean` |  | Whether the button is disabled and cannot be clicked anymore. |
| `isSecondary` | `boolean` |  | Displays the button in the secondary style. |
| `onClick` | `MouseEventHandler<HTMLButtonElement>` | ✓ | Function to be executed when the button is clicked. |
| `shouldShowAsSelectButton` | `boolean` |  | Whether the button should be displayed as a selectButton. |
| `shouldShowTextAsRobotoMedium` | `boolean` |  | Whether the text should be 'Roboto Medium'. |
| `shouldShowWaitCursor` | `boolean` |  | Shows a wait cursor instead of button text. |
| `shouldStopPropagation` | `boolean` |  | Stops event propagation on click. |

