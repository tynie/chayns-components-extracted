# RankingOverview

**Package:** `@chayns-components/ranking` (5.0.0-beta.1411)

## Code Example

```tsx
import React, { FC } from 'react';
import { PositionInput } from '@chayns-components/maps';

const Component: FC = () => {
    return <PositionInput apiToken="..." />;
};

Component.displayName = 'Component';

export default Component;

```

## Props

| Name | Type | Required | Description |
|------|------|----------|-------------|
| `suffix` | `string` | ✓ | A suffix that will be displayed before the total players. |
| `totalPlayers` | `number` | ✓ | The amount of the total players. |
| `userRank` | `number` |  | The Rank of the current user. |

