# NumberInput

**Package:** `@chayns-components/core` (5.0.0-beta.1411)

## Code Example

```tsx
import React, { FC } from 'react';
import { NumberInput } from '@chayns-components/core';

const Component: FC = () => {
    return <NumberInput />;
};

Component.displayName = 'Component';

export default Component;

```

## Props

| Name | Type | Required | Description |
|------|------|----------|-------------|
| `isDecimalInput` | `boolean` |  | Applies rules for decimal input. Enables the user to input one zero as number before the comma |
| `isDisabled` | `boolean` |  | Whether the input is disabled |
| `isInvalid` | `boolean` |  | Whether the value is invalid. |
| `isMoneyInput` | `boolean` |  | Applies rules for money input. Rules: only two decimal places, one zero before the comma |
| `isTimeInput` | `boolean` |  | Whether the value should be formatted as a time. |
| `maxNumber` | `number` |  | Limits the number to this value |
| `minNumber` | `number` |  | Limits the number to this value |
| `onBlur` | `(newNumber: number \| string \| null, isInvalid: boolean) => void` |  | Callback function that is called when the input gets out of focus |
| `onChange` | `(newValue: string) => void` |  | Callback function that is called when the input changes It will pass the text from the input |
| `placeholder` | `string` |  | Placeholder for the input field |
| `shouldShowOnlyBottomBorder` | `boolean` |  | Whether only the bottom border should be displayed |
| `shouldTriggerChangeOnFormat` | `boolean` |  | Whether the onChange function should be triggert when the value is formatted on the focus or blur |
| `value` | `string` |  | The value, that should be displayed in the input, when it is in focus. You can also pass a stringified number as default value. NOTE: If you pass a stringified number, it will be formatted to the selected format |

