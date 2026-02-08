# PositionInput

**Package:** `@chayns-components/maps` (5.0.0-beta.1411)

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
| `apiToken` | `string` | ✓ | The api token for google maps. |
| `initialPosition` | `Position` |  | The position of the center of the map on the initial render. |
| `markers` | `Marker[]` |  | Markers that should be displayed. |
| `onMarkerAdd` | `(marker: Marker) => void` |  | Function to be executed when a marker is added. |
| `onMarkerChange` | `(markers: Marker[]) => void` |  | Function to be executed when a marker position is changed. |
| `onMarkerRemove` | `(id: number) => void` |  | Function to be executed when a marker is removed. |
| `polygonOptions` | `PolygonOptions` |  | Options to style the polygon. |
| `searchPlaceholder` | `string` |  | The placeholder of the search input. |
| `zoom` | `number` |  | The zoom of the map. |

## Types

### Marker

```typescript
{ position: Position; id: number; }
```

### PolygonOptions

```typescript
{ strokeColor: string; strokeOpacity: number; strokeWeight: number; fillColor: string; fillOpacity: number; clickable: boolean; draggable: boolean; editable: boolean; visible: boolean; radius: number; zIndex: number; }
```

### Position

```typescript
{ lat: number; lng: number; }
```

