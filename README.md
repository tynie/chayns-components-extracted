# @chayns-components v5 – Extracted Documentation

Extracted component documentation from the official chayns-components v5 Doku.

**Data source:** [`https://chayns.space/77896-21884/chayns-components/v5/docs.json`](https://chayns.space/77896-21884/chayns-components/v5/docs.json)

## Structure

Each package has its own folder with one Markdown file per component:

| Package | Components |
|---------|-----------|
| `core` | Accordion, Button, Input, ComboBox, Filter, ... (57) |
| `color-picker` | ColorPicker, ColorPickerPopup, HueSlider, TransparencySlider |
| `date` | Calendar, DateInfo, OpeningInputs, OpeningTimes |
| `emoji-input` | EmojiInput, EmojiPicker, EmojiPickerPopup |
| `navigation` | DynamicToolbar, DynamicToolbarSpacer |
| `person-finder` | PersonFinder |
| `gallery` | Gallery |
| `code-highlighter` | CodeHighlighter |
| `devalue-slider` | DevalueSlider |
| `maps` | PositionInput |
| `ranking` | Ranking, RankingOverview |
| `scanner` | CodeScanner |
| `swipeable-wrapper` | SwipeableWrapper |
| `textstring` | Textstring, TextstringProvider |
| `translation` | AdaptiveTranslation, TranslationOptionsProvider |
| `typewriter` | Typewriter |

## Content per file

- **Code Example** – Complete TSX import and usage
- **Props Table** – Name, Type, Required, Description
- **Types** – TypeScript type definitions

## Installation

```bash
# Core components
npm install @chayns-components/core

# Additional components
npm install @chayns-components/code-highlighter
npm install @chayns-components/color-picker
npm install @chayns-components/date
npm install @chayns-components/devalue-slider
npm install @chayns-components/emoji-input
npm install @chayns-components/gallery
npm install @chayns-components/maps
npm install @chayns-components/navigation
npm install @chayns-components/person-finder
npm install @chayns-components/ranking
npm install @chayns-components/scanner
npm install @chayns-components/swipeable-wrapper
npm install @chayns-components/textstring
npm install @chayns-components/translation
npm install @chayns-components/typewriter
```

## Verwendung

Der PageProvider sorgt dafür, dass alle Deine Komponenten die richtigen Farben erhalten. Verwende den PageProvider einfach in der AppWrapper-Komponente, und alle Deine Komponenten, die von der App-Komponente ausgehen, profitieren davon.

```bash
import React from 'react';
import { ChaynsProvider } from 'chayns-api';
import { PageProvider } from '@chayns-components/core';
import App from './App';

const AppWrapper = () => (
    <ChaynsProvider>
        <PageProvider>
            <App />
        </PageProvider>
    </ChaynsProvider>
);

export default AppWrapper;
```
