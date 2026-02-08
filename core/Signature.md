# Signature

**Package:** `@chayns-components/core` (5.0.0-beta.1411)

## Code Example

```tsx
import React, { FC } from 'react';
import { Signature } from '@chayns-components/core';

const Component: FC = () => {
    return <Signature buttonText="Unterschreiben" />;
};

Component.displayName = 'Component';

export default Component;

```

## Props

| Name | Type | Required | Description |
|------|------|----------|-------------|
| `buttonText` | `string` | ✓ | The text that should be displayed inside the button. |
| `isDisabled` | `boolean` |  | Whether the button is disabled. |
| `onEdit` | `(signatureUrl: string) => void` |  | Function to be executed when the signature is edited. |
| `onRemove` | `() => void` |  | Function to be executed when the user deletes the signature. |
| `onSubscribe` | `(signatureUrl: string) => void` |  | Function to be executed when the user subscribes. |
| `onUnsubscribe` | `() => void` |  | Function to be executed when the user unsubscribes. |
| `ref` | `SignatureRef` |  |  |

## Types

### Signature

```typescript
{ verify: string; signature: string; expires: Date; }
```

### SignatureRef

```typescript
{ edit: VoidFunction; delete: VoidFunction; }
```

