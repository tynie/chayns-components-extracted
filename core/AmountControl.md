# AmountControl

**Package:** `@chayns-components/core` (5.0.0-beta.1411)

## Code Example

```tsx
import React, { FC } from 'react';
import { AmountControl } from '@chayns-components/core';

const Component: FC = () => {
    return <AmountControl />;
};

Component.displayName = 'Component';

export default Component;

```

## Props

| Name | Type | Required | Description |
|------|------|----------|-------------|
| `amount` | `number` |  | The amount that should be displayed. |
| `icon` | `string` |  | The icon that should be displayed if no amount is selected. |
| `iconColor` | `string` |  | The color of the icon. |
| `isDisabled` | `boolean` |  | Whether the control should be disabled |
| `label` | `string` |  | A Text that should be displayed if no amount is selected; |
| `maxAmount` | `number` |  | The maximum allowed amount. If the maxAmount is reached, a check icon is displayed on the left side. |
| `minAmount` | `number` |  | The minimum allowed amount. |
| `onChange` | `(amount: number) => void` |  | A Function that is executed when the amount is changed |
| `shouldForceLabel` | `boolean` |  | Whether the label should be displayed even if an amount is selected. |
| `shouldShowAddIconOnMinAmount` | `boolean` |  | Whether the "add"-icon should be displayed if the minAmount is reached. |
| `shouldShowIcon` | `boolean` |  | Whether the icon should be displayed if no amount is selected |
| `shouldShowWideInput` | `boolean` |  | Whether the input should be wider |
| `step` | `number` |  | Defines the amount that will change when adjusted |

