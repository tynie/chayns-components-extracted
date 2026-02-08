# RadioButtonGroup

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
| `canUncheckRadioButtons` | `boolean` |  | Whether the RadioButtons can be unchecked. |
| `children` | `ReactNode` | ✓ | The RadioButtons that should be grouped. Radio buttons with the same group are automatically unchecked when an `RadioButton` of the group is checked. |
| `onSelect` | `(id?: string) => void` |  | Function to be executed when an id is selected. |
| `selectedId` | `string` |  | The id of the current selected RadioButton. |
| `ref` | `RadioButtonGroupRef` |  |  |

## Types

### IUpdateSelectedRadioButtonId

```typescript
IUpdateSelectedRadioButtonId
```

### RadioButtonGroupRef

```typescript
{ updateSelectedRadioButtonId: IUpdateSelectedRadioButtonId; }
```

