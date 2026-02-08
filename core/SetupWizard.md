# SetupWizard

**Package:** `@chayns-components/core` (5.0.0-beta.1411)

## Code Example

```tsx
import React, { FC } from 'react';
import { SetupWizard, SetupWizardItem } from '@chayns-components/core';

const Component: FC = () => {
    return (
        <SetupWizard>
            <SetupWizardItem id={1} step={1} title="Start">
                Lorem
            </SetupWizardItem>
            <SetupWizardItem id={2} step={2} title="Ende">
                Lorem
            </SetupWizardItem>
        </SetupWizard>
    );
};

Component.displayName = 'Component';

export default Component;

```

## Props

| Name | Type | Required | Description |
|------|------|----------|-------------|
| `children` | `ReactElement<SetupWizardItemProps> \| ReactElement<SetupWizardItemProps>[]` | ✓ | The steps of the setup. Use the SetupWizardItem component. |
| `isWrapped` | `boolean` |  | This value must be set if the SetupWizard is inside an Accordion. |
| `ref` | `SetupWizardRef` |  |  |

## Types

### SetupWizardItemProps

```typescript
SetupWizardItemProps
```

### SetupWizardRef

```typescript
{ next: unknown; reset: unknown; }
```

