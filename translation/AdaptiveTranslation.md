# AdaptiveTranslation

**Package:** `@chayns-components/translation` (5.0.0-beta.1409)

## Code Example

```tsx
import React, { FC } from 'react';
import { AdaptiveTranslation, TranslationOptionsProvider } from '@chayns-components/translation';
import { Language, useLanguage } from 'chayns-api';

const Component: FC = () => {
    const language = useLanguage();

    return (
        <TranslationOptionsProvider
            from={language.site as Exclude<Language, Language.Unknown>}
            to={language.active as Exclude<Language, Language.Unknown>}
        >
            <AdaptiveTranslation>
                Lorem ipsum dolor sit amet, consectetur adipiscing elit. Ut vel finibus nunc, a
                cursus magna.
            </AdaptiveTranslation>
        </TranslationOptionsProvider>
    );
};

Component.displayName = 'Component';

export default Component;

```

## Props

| Name | Type | Required | Description |
|------|------|----------|-------------|
| `children` | `TranslationChildren` | ✓ | The Text that should be translated. |
| `className` | `string` |  | The className of the element. |
| `from` | `Exclude<Language, Language.Unknown>` |  | The language from which the text should be translated. |
| `onStateChange` | `(isLoading: boolean, isFetching: boolean) => void` |  | Function to be executed when the state of the translation is changed. |
| `shouldDisableOpacity` | `boolean` |  | Whether the opacity change should be disabled. |
| `style` | `CSSProperties` |  | Optional styles of the HTML element. |
| `tagName` | `keyof HTMLElementTagNameMap` |  | The HTML tag of the children. |
| `text` | `string` |  | The text that should be translated. Only active if the children is type of function. |
| `textType` | `string` |  | The type of the text. |
| `to` | `Exclude<Language, Language.Unknown>` |  | The language to which the text should be translated. |

## Types

### TranslationChildren

```typescript
string | unknown
```

