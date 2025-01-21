# Expo Camera onBarCodeScanned not firing

This repository demonstrates a bug in Expo's Camera API where the `onBarCodeScanned` function fails to trigger despite a barcode being detected. The camera preview functions correctly, but the callback function remains inactive.

## Bug Description
The `onBarCodeScanned` prop of the Expo Camera component is not called when a barcode is scanned.  The camera preview displays correctly, but the expected callback function never executes.  This prevents barcode scanning functionality from working as intended.

## Steps to Reproduce
1. Clone this repository.
2. Run the app using Expo Go.
3. Point the camera at a barcode.
4. Observe that the `onBarCodeScanned` function is not called despite successful barcode detection.

## Solution
The solution involves ensuring that the barcode data format and callback function registration are correctly configured.  Refer to `bugSolution.js` for a working example.