# DateInfo

**Package:** `@chayns-components/date` (5.0.0-beta.1411)

## Code Example

```tsx
import React, { FC } from 'react';
import { DateInfo } from '@chayns-components/date';

const Component: FC = () => {
    return <DateInfo date={new Date('2004-08-13')} />;
};

Component.displayName = 'Component';

export default Component;

```

## Props

| Name | Type | Required | Description |
|------|------|----------|-------------|
| `date` | `Date` | ✓ | The date that should be displayed |
| `language` | `Language` |  | The language that should be used for the date. Defaults to the active language given by chayns api. |
| `preText` | `string` |  | Additional text for the "shouldShowDateToNowDifference" prop. Writes a text before the calculated time. |
| `shouldShowDateToNowDifference` | `boolean` |  | Shows the difference from the date to now. The component handles updates itself. |
| `shouldShowDayOfWeek` | `boolean` |  | Adds the day of the week to the display |
| `shouldShowOnlyTime` | `boolean` |  | Whether only the time should be displayed. |
| `shouldShowRelativeDayOfWeek` | `boolean` |  | Whether the relative day of the week to today should be shown (today, yesterday or tomorrow). |
| `shouldShowTime` | `boolean` |  | Adds the time to the display. |
| `shouldShowYear` | `boolean` |  | Adds the current year to the display |
| `shouldUseShortText` | `boolean` |  | Shortens the day and month text to the maximum three digits |

