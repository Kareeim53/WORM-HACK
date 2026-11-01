# WORM HACK — Android prototype

Android Studio project for Android 8+ (target SDK 35), including Android 15 and ARM64 devices.

## Current prototype
- Imports a user-selected screenshot of an 8 Ball Pool table.
- Runs an on-device, lightweight color/connected-component ball detector.
- Draws candidate detections over the screenshot.

## Important implementation status
This is a **prototype**, not a finished live overlay or reliable pool solver. The detector uses simple pixel heuristics and will need calibration against multiple real screenshots. It does not read game memory, automate input, or guarantee correct ball identification. Live capture/overlay, pocket geometry, collision physics, and shot ranking are not implemented yet.

## Build
Open this folder in Android Studio (recent version), allow Gradle sync, then Build > Build Bundle(s) / APK(s) > Build APK(s).

Package: `com.worm.hack`
