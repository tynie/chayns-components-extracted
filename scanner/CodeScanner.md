# CodeScanner

**Package:** `@chayns-components/scanner` (5.0.0-beta.1411)

## Code Example

```tsx
import React, { FC } from 'react';
import { CodeScanner, ScannerErrorMessages } from '@chayns-components/scanner';

const Component: FC = () => {
    const errorMessages: ScannerErrorMessages = {
        alreadyInUse: 'Die Kamera wird bereits von einer anderen Anwendung verwendet.',
        cameraNotAvailable: 'Die Kameranutzung ist nicht möglich.',
        noCodeFound: 'Es konnte kein Code gefunden werden.',
        noPermission: 'Um einen QR-Code zu scannen, aktiviere Deine Kamera.',
    };

    return <CodeScanner errorMessages={errorMessages} />;
};

Component.displayName = 'Component';

export default Component;

```

## Props

| Name | Type | Required | Description |
|------|------|----------|-------------|
| `allowedFormats` | `Array<BarcodeFormat>` |  | Defines which barcode formats are allowed to be detected. |
| `errorMessages` | `ScannerErrorMessages` | ✓ | Custom error messages for various scanner states or failures. |
| `isFileSelectDisabled` | `boolean` |  | Disables the file select feature if set to true. |
| `isTorchDisabled` | `boolean` |  | Disables the torch (flashlight) feature if set to true. |
| `isZoomDisabled` | `boolean` |  | Disables the zoom control if set to true. |
| `maxZoom` | `number` |  | Maximum allowed zoom level for the camera. |
| `minZoom` | `number` |  | Minimum allowed zoom level for the camera. |
| `onScan` | `CodeReaderOnScanCallback` |  | Callback function triggered when a code is successfully scanned. |
| `placeholder` | `string` |  | A placeholder that should be displayed inside the preview. |
| `scanInterval` | `number` |  | The interval of the scans. |
| `shouldShowIconOverlay` | `boolean` |  | Whether a calling code icon should be displayed as an overlay. |
| `shouldTriggerForSameCode` | `boolean` |  | If true, allows scanning the same code multiple times in a row. |
| `trackConstraints` | `MediaTrackConstraints` |  | Custom media track constraints for controlling the video input. |
| `videoConstraints` | `MediaTrackConstraints` |  | Additional video constraints for the camera feed. |

## Types

### CodeReaderOnScanCallback

```typescript
CodeReaderOnScanCallback
```

### ScannerErrorMessages

```typescript
{ noPermission: string; alreadyInUse: string; cameraNotAvailable: string; noCodeFound: string; }
```

