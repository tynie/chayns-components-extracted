# AccordionGroup

**Package:** `@chayns-components/core` (5.0.0-beta.1411)

## Code Example

```tsx
import React, { FC } from 'react';
import { AccordionGroup, Accordion, AccordionContent } from '@chayns-components/core';

const Component: FC = () => {
    return (
        <AccordionGroup>
            <Accordion title="Accordion">
                <AccordionContent>
                    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Ut vel finibus nunc, a
                    cursus magna.
                </AccordionContent>
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
| `children` | `ReactNode` | ✓ | The Accordions that should be grouped. Accordions with the same group are automatically closed when an `Accordion` of the group is opened. |
| `isWrapped` | `boolean` |  | This value must be set for nested AccordionGroup components. This adjusts the style of the head and the padding of the content accordions. |
| `onClose` | `() => void` |  | Function that is executed when all accordions in group are closed. |
| `onOpen` | `() => void` |  | Function that is executed when any accordion in group will be opened. |

