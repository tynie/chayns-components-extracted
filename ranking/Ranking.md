# Ranking

**Package:** `@chayns-components/ranking` (5.0.0-beta.1411)

## Code Example

```tsx
import React, { FC } from 'react';
import { Ranking, RankingEntry } from '@chayns-components/ranking';

const Component: FC = () => {
    const entries: RankingEntry[] = [
        {
            rank: 1,
            name: 'Michael Gesenhues',
            personId: 'MIC-HAEL1',
            points: 12,
            content: [
                {
                    id: '12345-54321',
                    name: 'Richtiges Ergebnis',
                    value: '4',
                },
            ],
        },
        {
            rank: 2,
            name: 'Jannik Weise',
            personId: 'JAN-NIK96',
            points: 11,
            content: [
                {
                    id: '12345-54321',
                    name: 'Richtiges Ergebnis',
                    value: '3',
                },
            ],
        },
    ];

    const friendPersonIds = ['JAN-NIK96'];

    return <Ranking entries={entries} friendPersonIds={friendPersonIds} />;
};

Component.displayName = 'Component';

export default Component;

```

## Props

| Name | Type | Required | Description |
|------|------|----------|-------------|
| `entries` | `RankingEntry[]` | ✓ | Array of ranking entries to be displayed in the ranking list. |
| `friendPersonIds` | `string[]` | ✓ | Array of personIds that represent the user's friends. |
| `isLoadingData` | `boolean` |  | Whether new data is loading. |
| `onFriendAdd` | `(personId: string) => void` |  | Callback function triggered when a friend is added to the friends list. |
| `onFriendRemove` | `(personId: string) => void` |  | Callback function triggered when a friend is removed from the friends list. |
| `onFriendVisibleChange` | `() => void` |  | Callback function triggered when the visibility of friends is toggled. |
| `onLoadMore` | `() => void` |  | Callback function when the load more button is clicked. |
| `onSearchChange` | `(value: string) => void` |  | Callback function triggered when the search input value changes. |
| `searchValue` | `string` |  | The current value of the search input field. |
| `shouldShowOnlyFriends` | `boolean` |  | Whether only the friends of the user should be displayed (filtering and fetching the correct data is done by you). |
| `title` | `string` |  | The title of the top Accordion. |

## Types

### RankingContentEntry

```typescript
{ id: string; name: string; value: string; }
```

### RankingContentHeadline

```typescript
{ headline: string; id: string; }
```

### RankingEntry

```typescript
{ rank: number; name: string; personId: string; points: number; content?: Array; icons?: ReactNode; }
```

