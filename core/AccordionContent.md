# AccordionContent

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
| `children` | `ReactNode` | ✓ | The content of the accordion content element |
| `maxHeight` | `number` |  | Maximum height of the element. This automatically makes the content of the element scrollable. |
| `onScroll` | `(event: UIEvent<HTMLDivElement>) => void` |  | Function that is executed when the element will be scrolled |
| `shouldPreventBottomSpace` | `boolean` |  | Whether the bottom space should be removed. |

