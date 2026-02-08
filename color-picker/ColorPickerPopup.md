# ColorPickerPopup

**Package:** `@chayns-components/color-picker` (5.0.0-beta.1411)

## Code Example

```tsx
import React, { FC } from 'react';
import { ColorPickerPopup } from '@chayns-components/color-picker';

const Component: FC = () => {
    return (
        <ColorPickerPopup
            shouldShowPresetColors
            shouldShowTransparencySlider
            shouldShowMoreOptions
            shouldUseSiteColors
        />
    );
};

Component.displayName = 'Component';

export default Component;

```

## Props

| Name | Type | Required | Description |
|------|------|----------|-------------|
| `onPresetColorAdd` | `(presetColor: PresetColor) => void` |  |  |
| `onPresetColorRemove` | `(presetColorId: PresetColor['id']) => void` |  |  |
| `presetColors` | `PresetColor[]` |  |  |
| `shouldHideColorArea` | `boolean` | ✓ |  |
| `shouldHideDefaultPresetColors` | `boolean` | ✓ |  |
| `shouldShowMoreOptions` | `boolean` | ✓ |  |
| `shouldShowPresetColors` | `boolean` | ✓ |  |
| `shouldShowTransparencySlider` | `boolean` | ✓ |  |
| `shouldUseSiteColors` | `boolean` | ✓ |  |

## Types

### PresetColor

```typescript
{ isCustom?: boolean; id: string; color: string; }
```

