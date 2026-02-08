# MentionFinder

**Package:** `@chayns-components/core` (5.0.0-beta.1411)

## Code Example

```tsx
import React, { FC, useState } from 'react';
import {
    Input,
    MentionFinder,
    MentionMember,
    MentionFinderPopupAlignment,
} from '@chayns-components/core';

const MEMBERS: MentionMember[] = [
    {
        id: 'JAN-NIK96',
        imageUrl: 'https://sub60.tobit.com/u/JAN-NIK96',
        name: 'Jannik Weise',
        shouldShowRoundImage: true,
    },
    {
        id: 'MIC-HAEL1',
        imageUrl: 'https://sub60.tobit.com/u/MIC-HAEL1',
        name: 'JMichael Gesenhues',
        shouldShowRoundImage: true,
    },
];

const Component: FC = () => {
    const [value, setValue] = useState('');

    const handleSelect = ({ fullMatch, member }: { fullMatch: string; member: MentionMember }) => {
        console.log('MentionFinder:', { fullMatch, member });
    };

    return (
        <>
            <Input value={value} onChange={(event) => setValue(event.target.value)} />
            <MentionFinder
                inputValue={value}
                members={MEMBERS}
                onSelect={handleSelect}
                popupAlignment={MentionFinderPopupAlignment.Bottom}
            />
        </>
    );
};

Component.displayName = 'Component';

export default Component;

```

## Props

| Name | Type | Required | Description |
|------|------|----------|-------------|
| `dragCloseThresholdInPx` | `number` |  | Threshold in pixels to drag to close the popup |
| `enableDragHandle` | `boolean` |  | Enables the optional drag handle inside the popup |
| `inputValue` | `string` | ✓ | The text from the input field |
| `members` | `MentionMember[]` | ✓ | Members that can be selected |
| `onSelect` | `({ fullMatch, member }: { fullMatch: string; member: MentionMember }) => void` | ✓ | Function to be executed when a member is selected |
| `overlayContainerSelector` | `string` |  | Selector for the container to render the overlay into (defaults to closest dialog, thread, page provider or tapp) |
| `popupAlignment` | `MentionFinderPopupAlignment` | ✓ | Alignment of the popup |

## Types

### MentionFinderPopupAlignment

```typescript
{ Top = 0, Bottom = 1 }
```

### MentionMember

```typescript
MentionMember
```

