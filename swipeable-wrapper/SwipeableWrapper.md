# SwipeableWrapper

**Package:** `@chayns-components/swipeable-wrapper` (5.0.0-beta.1411)

## Code Example

```tsx
import React, { FC } from 'react';
import { SwipeableWrapper, SwipeableActionItem } from '@chayns-components/swipeable-wrapper';
import { Icon } from '@chayns-components/core';

const Component: FC = () => {
    const leftActions: SwipeableActionItem[] = [
        {
            action: () => console.log('Comment'),
            backgroundColor: 'blue',
            color: 'white',
            icon: <Icon color="white" icons={['fa fa-comment']} />,
            key: 'comment',
            text: 'Comment',
        },
    ];

    const rightActions: SwipeableActionItem[] = [
        {
            action: () => console.log('Star'),
            backgroundColor: 'darkkhaki',
            color: 'black',
            icon: <Icon color="black" icons={['fa fa-star']} />,
            key: 'star',
            text: 'Star',
        },
        {
            action: () => console.log('Fire'),
            backgroundColor: 'red',
            color: 'white',
            icon: <Icon color="white" icons={['fa fa-fire']} />,
            key: 'fire',
            text: 'Fire',
        },
    ];

    return (
        <SwipeableWrapper rightActions={rightActions} leftActions={leftActions}>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit.
        </SwipeableWrapper>
    );
};

Component.displayName = 'Component';

export default Component;

```

## Props

| Name | Type | Required | Description |
|------|------|----------|-------------|
| `children` | `ReactNode` | ✓ | The content of the Swipeable item. |
| `isDisabled` | `boolean` |  | Whether the swipeable functionality is disabled |
| `leftActions` | `SwipeableActionItem[]` |  | The left-side actions, ordered from the left to the right. |
| `onSwipeEnd` | `() => void` |  | Callback to be executed when the swiping is ended. |
| `onSwipeStart` | `() => void` |  | Callback to be executed when the swiping is started. |
| `rightActions` | `SwipeableActionItem[]` |  | The right-side actions, ordered from left to the right. |
| `shouldUseOpacityAnimation` | `boolean` |  | Whether the opacity should be animated when swiping in the actions. |

## Types

### SwipeableActionItem

```typescript
SwipeableActionItem
```

