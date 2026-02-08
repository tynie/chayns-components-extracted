# AccordionItem

**Package:** `@chayns-components/core` (5.0.0-beta.1411)

## Code Example

```tsx
import React, { FC } from 'react';
import { AccordionGroup, Accordion, AccordionItem } from '@chayns-components/core';

const Component: FC = () => {
    return (
        <AccordionGroup>
            <Accordion title="Accordion">
                <AccordionItem>Lorem ipsum dolor sit amet</AccordionItem>
            </Accordion>
        </AccordionGroup>
    );
};

Component.displayName = 'Component';

export default Component;

```

## Props

| Name | Type | Required | Description |
|------|------|----------|-------------|
| `children` | `ReactNode` | ✓ | The content of the accordion content element |

