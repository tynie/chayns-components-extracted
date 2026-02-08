# SetupWizardItem

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
| `children` | `ReactNode` | ✓ | The content that should be displayed inside the item. |
| `id` | `number` | ✓ | The id of the item. |
| `step` | `number` | ✓ | The step of the item. |
| `title` | `string` | ✓ | The title of the item. |

