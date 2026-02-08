# PersonFinder

**Package:** `@chayns-components/person-finder` (5.0.0-beta.1411)

## Code Example

```tsx
import React, { FC } from 'react';
import { PersonFinder } from '@chayns-components/person-finder';

const Component: FC = () => {
    return <PersonFinder />;
};

Component.displayName = 'Component';

export default Component;

```

## Props

| Name | Type | Required | Description |
|------|------|----------|-------------|
| `container` | `Element` |  | The element where the content of the `PersonFinder` should be rendered via React Portal. |
| `dropdownDirection` | `DropdownDirection` |  | The direction in which the dropdown should be displayed. By default, it is displayed below the input. |
| `filterTypes` | `PersonFinderFilterTypes[]` |  | The filter options of the component. |
| `friendsPriority` | `Priority` |  | Determines the priority level for displaying friends in search results. |
| `leftElement` | `ReactElement` |  | An element that should be displayed on the left side of the input. |
| `maxEntries` | `number` |  | The maximum number of entries that can be selected. |
| `onAdd` | `(entry: PersonFinderEntry) => void` |  | Function to be executed if a person or site is added. |
| `onDropdownHide` | `() => void` |  | Function to be executed if the dropdown is hidden. |
| `onDropdownShow` | `() => void` |  | Function to be executed if the dropdown is shown. |
| `onRemove` | `(id: PersonFinderEntry['id']) => void` |  | Function to be executed if a person or site is removed. |
| `placeholder` | `string` |  | The placeholder that should be displayed. |
| `shouldAllowMultiple` | `boolean` |  | Whether multiple persons and sites should be selected. |
| `shouldDisableRemove` | `boolean` |  | Whether the remove action should be disabled. |
| `shouldHideResultsOnAdd` | `boolean` |  | Whether the dropdown should be hidden after adding an entry. By default, it is not hidden. |
| `shouldRenderInline` | `boolean` |  | Whether the `PersonFinder` should be rendered inline without a dropdown. |
| `ref` | `PersonFinderRef` |  |  |

## Types

### DropdownDirection

```typescript
{ BOTTOM = 0, TOP = 1, BOTTOM_LEFT = 2, BOTTOM_RIGHT = 3, TOP_LEFT = 4, TOP_RIGHT = 5, LEFT = 6, RIGHT = 7 }
```

### PersonEntry

```typescript
{ id: string; firstName: string; lastName: string; commonSites: number; isVerified: boolean; type: PERSON; }
```

### PersonFinderEntry

```typescript
PersonEntry | SiteEntry | UACEntry
```

### PersonFinderFilterTypes

```typescript
{ PERSON = "person", SITE = "site", UAC = "uac" }
```

### PersonFinderRef

```typescript
PersonFinderRef
```

### Priority

```typescript
{ HIGH = 0, NORMAL = 1 }
```

### SiteEntry

```typescript
{ id: string; url: string; name: string; type: SITE; }
```

### UACEntry

```typescript
{ id: number; name: string; isSystemGroup: boolean; }
```

