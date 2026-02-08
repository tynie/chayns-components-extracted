# ListItem

**Package:** `@chayns-components/core` (5.0.0-beta.1411)

## Code Example

```tsx
import React, { FC } from 'react';
import { List, ListItem } from '@chayns-components/core';

const Component: FC = () => {
    return (
        <List>
            <ListItem title="Test 1" />
            <ListItem title="Test 2" />
            <ListItem title="Test 3" />
        </List>
    );
};

Component.displayName = 'Component';

export default Component;

```

## Props

| Name | Type | Required | Description |
|------|------|----------|-------------|
| `backgroundColor` | `CSSProperties['backgroundColor']` |  | The background color of the `ListItem`. |
| `careOfLocationId` | `number` |  | DEPRECATED: Use `cornerImage` instead. |
| `children` | `ReactNode` |  | The content of the `ListItem` body. When the `ListItem` has children, it can be opened and also gets an icon as an indicator automatically. |
| `cornerElement` | `ReactNode` |  | Optional Element to display in the right corner of the image |
| `cornerImage` | `string` |  | The image that is displayed in the bottom right corner of the grouped image of list item. |
| `hoverItem` | `ReactNode` |  | Element that is displayed when hovering over the `ListItem` on the right side. On mobile devices, this element is not displayed. |
| `icons` | `string[]` |  | The FontAwesome or tobit icons to render like an image on the left side of the header. Multiple icons are stacked. See the `Icon` component documentation for more information. |
| `imageBackground` | `CSSProperties['background']` |  | The background of the image. This is only used if images are passed. |
| `images` | `string[]` |  | A list of image URLs that are displayed on the left side of the header. If multiple URLs are passed, the image is assembled from the first three image URLs as a puzzle. |
| `isDefaultOpen` | `boolean` |  | This can be used to automatically expand the `ListItem` during the first render. |
| `isOpen` | `boolean` |  | This overrides the internal opening state of the item and makes it controlled. |
| `isTitleGreyed` | `boolean` |  | Whether the ListItem locks disabled but has full functionality. |
| `leftElements` | `ListItemElements` |  | Elements that are displayed on the left side of the header. If multiple elements are specified, they are displayed one aside the other. |
| `onClick` | `MouseEventHandler<HTMLDivElement>` |  | Function to be executed when the header of the `ListItem` was clicked |
| `onClose` | `() => void` |  | Function to be executed when the ListItem is closed. |
| `onImageError` | `(event: SyntheticEvent<HTMLImageElement, Event>, index: number) => void` |  | Optional handler for image load errors. |
| `onLongPress` | `TouchEventHandler<HTMLDivElement>` |  | Function to be executed when the header of the `ListItem` is pressed for 400 milliseconds. |
| `onOpen` | `() => void` |  | Function to be executed when the ListItem is opened. |
| `onSizeChange` | `(sizes: ListItemSize) => void` |  | Function to be executed if the size are changed. |
| `rightElements` | `IListItemRightElements` |  | Elements that are displayed on the right side of the header. If multiple elements are specified, they are displayed one below the other. |
| `shouldDisableAnimation` | `boolean` |  | Whether the ListItem Animation should be disabled. |
| `shouldForceBackground` | `boolean` |  | This will force the background color of the ListItem to be used even if it is closed and not hovered. |
| `shouldForceBottomLine` | `boolean` |  | Whether the line should be forced, e.g., so that it is also displayed if the item is the last element in the list. |
| `shouldForceHover` | `boolean` |  | Whether the hover item should be forced. |
| `shouldHideBottomLine` | `boolean` |  | Whether the bottom line should be hidden. |
| `shouldHideImageOrIconBackground` | `boolean` |  | Whether the background and border of the shape on which the image or icon of the element is displayed should be hidden. |
| `shouldHideIndicator` | `boolean` |  | If the `ListItem` is expandable, the indicator is displayed on the left side of the header. If this property is set to true, the indicator is hidden. |
| `shouldOpenImageOnClick` | `boolean` |  | Whether the image should be opened on click. |
| `shouldPreventLayoutAnimation` | `boolean` |  | Whether the layout animation should be prevented. This is useful when the `ListItem` is used in a list with a lot of items and the layout animation is not desired. |
| `shouldRenderClosed` | `boolean` |  | This will render the ListItem closed on the first render. |
| `shouldShowRoundImageOrIcon` | `boolean` |  | Whether the image or icon should be displayed in a round shape. This should always be used for images of persons. |
| `shouldShowSeparatorBelow` | `boolean` |  | Whether a separator should be displayed below this item. In this case, the border is displayed thicker than normal. |
| `shouldShowTooltipOnTitleOverflow` | `boolean` |  | Whether a Tooltip should be displayed on hover if the title is cut. |
| `subtitle` | `ReactNode` |  | Subtitle of the `ListItem` displayed in the head below the title |
| `title` | `ReactNode` | ✓ | Title of the `ListItem` displayed in the head |
| `titleElement` | `ReactNode` |  | Additional elements to be displayed in the header next to the title. |
| `ref` | `ListItemSize` |  |  |

## Types

### IListItemRightElement

```typescript
{ bottom?: ReactNode; center?: ReactNode; top?: ReactNode; topAlignment?: string & unknown | "-moz-initial" | "inherit" | "initial" | "revert" | "revert-layer" | "unset" | "left" | "center" | "right" | "space-around" | "space-between" | "space-evenly" | "stretch" | "end" | "flex-end" | "flex-start" | "start" | "normal"; bottomAlignment?: string & unknown | "-moz-initial" | "inherit" | "initial" | "revert" | "revert-layer" | "unset" | "left" | "center" | "right" | "space-around" | "space-between" | "space-evenly" | "stretch" | "end" | "flex-end" | "flex-start" | "start" | "normal"; }
```

### IListItemRightElements

```typescript
ReactNode
```

### ListItemElements

```typescript
ListItemElements
```

### ListItemSize

```typescript
{ titleWidth: number; titleMaxWidth: number; }
```

