# ProgressBar

**Package:** `@chayns-components/core` (5.0.0-beta.1411)

## Code Example

```tsx
import React, { FC } from 'react';
import { ProgressBar } from '@chayns-components/core';

const Component: FC = () => {
    return <ProgressBar percentage={69} />;
};

Component.displayName = 'Component';

export default Component;

```

## Props

| Name | Type | Required | Description |
|------|------|----------|-------------|
| `colors` | `Colors` |  | The colors of the ProgressBar. |
| `label` | `string` |  | The label that should be displayed under the progressbar. |
| `percentage` | `Range<0, 101>` |  | The percentage of the progress. Number between 0 and 100. |
| `shouldHideProgress` | `boolean` |  | Whether the progress should be hide and just display the label. |
| `shouldShowLabelInline` | `boolean` |  | Whether the label should be displayed inside the ProgressBar. |
| `steps` | `Range<0, 101>[]` |  | Visual marked steps. |

## Types

### Colors

```typescript
{ backgroundColor?: string; progressColor?: string; stepColor?: string; primaryTextColor?: string; secondaryTextColor?: string; }
```

### Range

```typescript
Range<F, T>
```

