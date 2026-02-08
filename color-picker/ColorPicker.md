# ColorPicker

**Package:** `@chayns-components/color-picker` (5.0.0-beta.1411)

## Props

| Name | Type | Required | Description |
|------|------|----------|-------------|
| `alignment` | `PopupAlignment` |  | The alignment of the popup |
| `children` | `ReactNode` |  | The element that should be rendered to trigger the ColorPicker popup on click. |
| `onPresetColorAdd` | `(presetColor: PresetColor) => void` |  | Function to be executed when a preset color is added. |
| `onPresetColorRemove` | `(presetColorId: PresetColor['id']) => void` |  | Function to be executed when a preset color is removed. |
| `onSelect` | `(color: string) => void` |  | Function to be executed when a color is selected. |
| `presetColors` | `PresetColor[]` |  | Colors the user can select from. |
| `selectedColor` | `string` |  | The color that should be preselected. |
| `shouldHideColorArea` | `boolean` |  | Whether the color area should be displayed. |
| `shouldHideDefaultPresetColors` | `boolean` |  | Whether the default preset colors should be hidden. |
| `shouldShowAsPopup` | `boolean` |  | Whether the ColorPicker should be displayed inside a popup. |
| `shouldShowMoreOptions` | `boolean` |  | Whether the more options accordion should be displayed. |
| `shouldShowPresetColors` | `boolean` |  | Whether the preset colors should be displayed. |
| `shouldShowPreviewColorString` | `boolean` |  | Whether the preview color should be displayed as text. |
| `shouldShowRoundPreviewColor` | `boolean` |  | Whether the preview color should be displayed round. |
| `shouldShowTransparencySlider` | `boolean` |  | Whether the transparency slider should be displayed. |
| `shouldUseSiteColors` | `boolean` |  | Whether presetColors should be got and uploaded to the site storage. |

## Types

### PopupAlignment

```typescript
{ TopLeft = 0, TopCenter = 1, TopRight = 2, BottomLeft = 3, BottomCenter = 4, BottomRight = 5 }
```

### PresetColor

```typescript
{ isCustom?: boolean; id: string; color: string; }
```

