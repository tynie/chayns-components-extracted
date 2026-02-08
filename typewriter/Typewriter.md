# Typewriter

**Package:** `@chayns-components/typewriter` (5.0.0-beta.1411)

## Code Example

```tsx
import React, { FC } from 'react';
import { Typewriter } from '@chayns-components/typewriter';

const Component: FC = () => {
    return (
        <Typewriter>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Ut vel finibus nunc, a cursus
            magna.
        </Typewriter>
    );
};

Component.displayName = 'Component';

export default Component;

```

## Props

| Name | Type | Required | Description |
|------|------|----------|-------------|
| `animationSteps` | `number` |  | The number of characters that will be animated per animation cycle. |
| `autoSpeedBaseFactor` | `number` |  | The base speed factor to calculate the animation speed. |
| `children` | `ReactElement \| ReactElement[] \| string \| string[]` | ✓ | The text to type |
| `cursorType` | `CursorType` |  | The type of the cursor. Use the CursorType enum for this prop. |
| `nextTextDelay` | `TypewriterDelay` |  | The delay in milliseconds before the next text is shown. This prop is only used if multiple texts are given. |
| `onFinish` | `() => void` |  | Function that is executed when the typewriter animation has finished. This function will not be executed if multiple texts are used. |
| `onResetAnimationEnd` | `() => void` |  | Function that is executed when the reset animation has finished. This function will not be executed if `shouldUseResetAnimation` is not set to `true`. |
| `onResetAnimationStart` | `() => void` |  | Function that is executed when the reset animation has started. This function will not be executed if `shouldUseResetAnimation` is not set to `true`. |
| `onTypingAnimationEnd` | `() => void` |  | Function that is executed when the typing animation has finished. If multiple texts are given, this function will be executed for each text. |
| `onTypingAnimationStart` | `() => void` |  | Function that is executed when the typing animation has started. If multiple texts are given, this function will be executed for each text. |
| `pseudoChildren` | `ReactElement \| string` |  | Pseudo-element to be rendered invisible during animation to define the size of the element for the typewriter effect. By default, the "children" is used for this purpose. |
| `resetDelay` | `TypewriterDelay` |  | Waiting time in milliseconds before the typewriter resets the text. This prop is only used if multiple texts are given. |
| `resetSpeed` | `TypewriterSpeed \| number` |  | The reset speed of the animation. Use the TypewriterSpeed enum for this prop. |
| `shouldCalcAutoSpeed` | `boolean` |  | Whether the animation speed should be calculated with the chunk interval. |
| `shouldForceCursorAnimation` | `boolean` |  | Specifies whether the cursor should be forced to animate even if no text is currently animated. |
| `shouldHideCursor` | `boolean` |  | Specifies whether the cursor should be hidden |
| `shouldRemainSingleLine` | `boolean` |  | Whether the content should remain a single line. |
| `shouldSortChildrenRandomly` | `boolean` |  | Specifies whether the children should be sorted randomly if there are multiple texts. This makes the typewriter start with a different text each time and also changes them in a random order. |
| `shouldUseAnimationHeight` | `boolean` |  | Specifies whether the animation should use its full height or the height of the current chunk. |
| `shouldUseResetAnimation` | `boolean` |  | Specifies whether the reset of the text should be animated with a backspace animation for multiple texts. |
| `shouldWaitForContent` | `boolean` |  | Whether the typewriter should wait for new content |
| `speed` | `TypewriterSpeed \| number` |  | The speed of the animation. Use the TypewriterSpeed enum for this prop. |
| `startDelay` | `TypewriterDelay` |  | The delay in milliseconds before the typewriter starts typing. |
| `textStyle` | `CSSPropertiesWithVars` |  | The style of the typewriter text element |

## Types

### CursorType

```typescript
{ Default = "default", Thin = "thin" }
```

### TypewriterDelay

```typescript
{ ExtraSlow = 4000, Slow = 2000, Medium = 1000, Fast = 500, ExtraFast = 250, None = 0 }
```

### TypewriterSpeed

```typescript
{ ExtraSlow = 40, Slow = 20, Medium = 10, Fast = 5, ExtraFast = 2.5 }
```

