# OpeningTimes

**Package:** `@chayns-components/date` (5.0.0-beta.1411)

## Code Example

```tsx
import React, { FC } from 'react';
import { OpeningTimes, Weekday, OpeningTime } from '@chayns-components/date';

const WEEKDAYS: Weekday[] = [
    { id: 0, name: 'Montag' },
    { id: 1, name: 'Dienstag' },
    { id: 2, name: 'Mittwoch' },
    { id: 3, name: 'Donnerstag' },
    { id: 4, name: 'Freitag' },
    { id: 5, name: 'Samstag' },
    { id: 6, name: 'Sonntag' },
];

const OPENING_TIMES: OpeningTime[] = [
    {
        id: 'montag',
        weekdayId: 0,
        times: [{ start: '08:00', end: '18:00', id: '1' }],
        isDisabled: true,
    },
    {
        id: 'dienstag',
        weekdayId: 1,
        times: [
            { start: '08:00', end: '12:00', id: '2' },
            { start: '11:00', end: '18:00', id: '3' },
        ],
    },
    { id: 'mittwoch', weekdayId: 2, times: [{ start: '08:00', end: '18:00', id: '4' }] },
    { id: 'donnerstag', weekdayId: 3, times: [{ start: '08:00', end: '18:00', id: '5' }] },
    { id: 'freitag', weekdayId: 4, times: [{ start: '08:00', end: '18:00', id: '6' }] },
    { id: 'samstag', weekdayId: 5, times: [{ start: '08:00', end: '18:00', id: '7' }] },
    { id: 'sonntag', weekdayId: 6, times: [{ start: '18:00', end: '08:00', id: '8' }] },
];

const Component: FC = () => {
    return <OpeningTimes openingTimes={OPENING_TIMES} weekdays={WEEKDAYS} />;
};

Component.displayName = 'Component';

export default Component;

```

## Props

| Name | Type | Required | Description |
|------|------|----------|-------------|
| `closedText` | `string` |  | The text that should be displayed when a day is closed. |
| `currentDayId` | `OpeningTime['id']` |  | If set just the current day is displayed and the whole week in a tooltip. |
| `editMode` | `boolean` |  | Whether the opening times can be edited. |
| `hintText` | `string` |  | The text that should be displayed if times are colliding. |
| `hintTextPosition` | `HintTextPosition` |  | The position of the hint text. |
| `onChange` | `({ time, enabledDays, dayId, isValid }: OnChange) => void` |  | Function to be executed when a time is changed or a day is enabled/disabled. |
| `onTimeAdd` | `({ time, dayId, isValid }: OnTimeAdd) => void` |  | Function to be executed when a time is added. |
| `onTimeRemove` | `(id: string) => void` |  | Function to be executed when a time is removed. |
| `openingTimes` | `OpeningTime[]` | ✓ | The opening times corresponding to its weekday. |
| `weekdays` | `Weekday[]` | ✓ | The weekdays that should be displayed. |

## Types

### HintTextPosition

```typescript
{ Top = 0, Bottom = 1 }
```

### OnChange

```typescript
{ enabledDays?: Array; dayId?: string; time?: Time; isValid?: boolean; }
```

### OnTimeAdd

```typescript
{ dayId: string; time: Time; isValid: boolean; }
```

### OpeningTime

```typescript
{ weekdayId: number; id: string; isDisabled?: boolean; times: Array; }
```

### Time

```typescript
{ id: string; start: string; end: string; }
```

### Weekday

```typescript
{ name: string; id: number; }
```

