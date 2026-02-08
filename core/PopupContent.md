# PopupContent

**Package:** `@chayns-components/core` (5.0.0-beta.1411)

## Code Example

```tsx
import React, { FC } from 'react';
import { Popup, PopupContent } from '@chayns-components/core';

const Component: FC = () => {
    const popupContent = <PopupContent>Lorem</PopupContent>;

    return <Popup content={popupContent}>Lorem</Popup>;
};

Component.displayName = 'Component';

export default Component;

```

## Props

| Name | Type | Required | Description |
|------|------|----------|-------------|
| `children` | `ReactNode` |  | The elements that should be displayed inside the popup content. |

