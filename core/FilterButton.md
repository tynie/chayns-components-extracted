# FilterButton

**Package:** `@chayns-components/core` (5.0.0-beta.1411)

## Props

| Name | Type | Required | Description |
|------|------|----------|-------------|
| `color` | `CSSProperties['color']` |  |  |
| `count` | `number` |  |  |
| `icons` | `string[]` |  |  |
| `id` | `string` | ✓ |  |
| `isDisabled` | `boolean` |  |  |
| `isSelected` | `boolean` | ✓ |  |
| `onSelect` | `(key: string) => void` | ✓ |  |
| `shape` | `FilterButtonItemShape` | ✓ |  |
| `size` | `FilterButtonSize` | ✓ |  |
| `text` | `string` | ✓ |  |

## Types

### FilterButtonItemShape

```typescript
{ Round = 0, Rectangular = 1 }
```

### FilterButtonSize

```typescript
{ Small = 0, Normal = 1 }
```

