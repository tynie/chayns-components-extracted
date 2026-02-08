# Accordion

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
| `bodyMaxHeight` | `number` |  | Maximum height of the accordion body element. This automatically makes the content of the body element scrollable. |
| `children` | `ReactNode` | ✓ | The content of the accordion body |
| `icon` | `string` |  | The icon that is displayed in front of the title |
| `isDefaultOpen` | `boolean` |  | This can be used to automatically expand the Accordion during the first render. |
| `isDisabled` | `boolean` |  | This will disable the Accordion so that it cannot be opened and will gray out the title. Does not work with isOpened. |
| `isFixed` | `boolean` |  | This can be used so that the Accordion cannot be opened or closed. In addition, in this case the icon is exchanged to mark the Accordions. |
| `isOpened` | `boolean` |  | This can be used to open the Accordion from the outside |
| `isTitleGreyed` | `boolean` |  | This will gray out the title of the Accordion to indicate hidden content, for example. |
| `onBodyAnimationComplete` | `() => void` |  | Function that is executed when the accordion body is animated |
| `onBodyScroll` | `(event: UIEvent<HTMLDivElement>) => void` |  | Function that is executed when the accordion body will be scrolled |
| `onClose` | `() => void` |  | Function that is executed when the accordion will be closed. |
| `onHoverEnd` | `MouseEventHandler<HTMLDivElement>` |  | Function to be executed when the accordion is no longer hovered. |
| `onHoverStart` | `MouseEventHandler<HTMLDivElement>` |  | Function to be executed when the accordion is hovered. |
| `onOpen` | `() => void` |  | Function that is executed when the accordion will be opened. |
| `onSearchChange` | `ChangeEventHandler<HTMLInputElement>` |  | Function that is executed when the text of the search in the accordion head changes. When this function is given, the search field is displayed in the Accordion Head. |
| `onTitleInputChange` | `ChangeEventHandler<HTMLInputElement>` |  | Function that is executed when the text of the search in the accordion title changes. When this function is given, the search field is displayed as the Accordion title. |
| `rightElement` | `ReactNode` |  | Content to be displayed on the right side in the head of the Accordion |
| `searchPlaceholder` | `string` |  | The placeholder to be used for the search |
| `searchValue` | `string` |  | The value that is displayed inside the search |
| `shouldForceBackground` | `boolean` |  | This will force the background color of the accordion to be used even if it is closed and not hovered. |
| `shouldHideBackground` | `boolean` |  | This will hide the background color of the accordion |
| `shouldHideBottomLine` | `boolean` |  | Whether the bottom line should be hidden. |
| `shouldIndex` | `boolean` |  | Whether the accordion should be indexed. |
| `shouldRenderClosed` | `boolean` |  | This will render the Accordion closed on the first render. |
| `shouldRotateIcon` | `boolean` |  | Whether the icon should be rotating. |
| `shouldSkipAnimation` | `boolean` |  | Whether the animation should be skipped. If 'isDefaultOpen' is true the initial animation will be skipped even this prop is false |
| `title` | `string` |  | Title of the Accordion displayed in the head |
| `titleColor` | `CSSProperties['color']` |  | The title color. |
| `titleElement` | `ReactNode` |  | Additional elements to be displayed in the header next to the title. |
| `titleInputProps` | `InputProps` |  | The props of the title Input. |

## Types

### InputProps

```typescript
InputProps
```

