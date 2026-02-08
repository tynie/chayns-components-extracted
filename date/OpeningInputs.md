# OpeningInputs

**Package:** `@chayns-components/date` (5.0.0-beta.1411)

## Props

| Name | Type | Required | Description |
|------|------|----------|-------------|
| `closedText` | `string` |  | The text to show when the inputs are disabled |
| `currentDayId` | `OpeningTime['id']` |  | The id of the current day |
| `editMode` | `boolean` |  | If the edit mode is enabled |
| `id` | `string` | ✓ | The id of the opening time |
| `isDisabled` | `boolean` |  | If the inputs are disabled |
| `onAdd` | `(time: Time, id: string) => void` |  | Function that is called when a new time is added |
| `onChange` | `(time: Time) => void` |  | Function that is called when a time is changed |
| `onInvalid` | `(openingTimeId: string, timeIds: string[]) => void` |  | Function that is called when the times are invalid |
| `onRemove` | `(id: Time['id']) => void` |  | Function that is called when a time is removed |
| `times` | `Time[]` | ✓ | Array of opening times |

## Types

### OpeningTime

```typescript
{ weekdayId: number; id: string; isDisabled?: boolean; times: Array; }
```

### Time

```typescript
{ id: string; start: string; end: string; }
```

