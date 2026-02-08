# Calendar

**Package:** `@chayns-components/date` (5.0.0-beta.1411)

## Code Example

```tsx
import React, { FC } from 'react';
import { Calendar } from '@chayns-components/date';

const Component: FC = () => {
    return <Calendar />;
};

Component.displayName = 'Component';

export default Component;

```

## Props

| Name | Type | Required | Description |
|------|------|----------|-------------|
| `categories` | `Categories[]` |  | An array to group dates into a category. |
| `currentDateBackgroundColor` | `CSSProperties['backgroundColor']` |  | When set, the current date will be highlighted in the corresponding style. |
| `customThumbColors` | `CustomThumbColors` |  | Custom colors for the thumb. |
| `disabledDates` | `Date[]` |  | An array of dates that should be disabled. |
| `highlightedDates` | `HighlightedDates[]` |  | An array with dates and corresponding styles to highlight. |
| `isDisabled` | `boolean` |  | To disable the Calendar |
| `locale` | `Language` |  | The locale language to format the dates. |
| `maxDate` | `Date` |  | The maximum date that can be selected. |
| `minDate` | `Date` |  | The minimum date that can be selected. |
| `onChange` | `(date: Date \| Date[] \| DateInterval) => void` |  | Function to be executed when the selected date, dates or date interval change. |
| `onShownDatesChange` | `(dates: { start: Date; end: Date }) => void` |  | Function to be executed when the shown dates change. Returns the start of the displayed month and the end of the last displayed month (since depending on the available widths, there are one or two months displayed). |
| `shouldShowHighlightsInMonthOverlay` | `boolean` |  | Whether the highlighted dates should be displayed for the greyed month overlay days. |
| `showMonthYearPickers` | `boolean` |  | Shows the month and year pickers, if there are multiple months/years to select from. |

## Types

### Categories

```typescript
{ id: string; dates: Array; color: CSSProperties['color']; }
```

### CustomThumbColors

```typescript
{ mainBackgroundColor?: CSSProperties['color']; mainTextColor?: CSSProperties['color']; secondaryBackgroundColor?: CSSProperties['color']; }
```

### DateInterval

```typescript
DateInterval
```

### HighlightedDates

```typescript
{ dates: Array; style: HighlightedDateStyles; }
```

### HighlightedDateStyles

```typescript
{ backgroundColor: CSSProperties['color']; textColor: CSSProperties['color']; }
```

