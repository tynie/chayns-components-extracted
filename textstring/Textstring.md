# Textstring

**Package:** `@chayns-components/textstring` (5.0.0-beta.1411)

## Props

| Name | Type | Required | Description |
|------|------|----------|-------------|
| `children` | `ReactElement` |  | The element that the text should be displayed in. |
| `childrenClassName` | `string` |  | The class name of the HTML element that the text should be displayed in. Only used if `children` is not set. |
| `childrenStyles` | `CSSProperties` |  | The styles of the HTML element that the text should be displayed in. Only used if `children` is not set. |
| `childrenTagName` | `keyof ReactHTML` |  | The tag of the HTML element that the text should be displayed in. Only used if `children` is not set. |
| `isTextstringHTML` | `boolean` |  | Whether the textstring contains HTML elements and should be displayed as HTML. |
| `replacements` | `TextstringReplacement` |  | Replacement values for the textstring. |
| `textstring` | `ITextstring` | ✓ | The text that should be displayed. |

## Types

### ITextstring

```typescript
{ fallback: string; name: string; }
```

### TextstringReplacement

```typescript
{ }
```

