# NyaUI

An Android UI Client.

![Package](https://img.shields.io/badge/Package-com.nyaui.me-blue)
![Min SDK](https://img.shields.io/badge/Min%20SDK-31-green)
![Target SDK](https://img.shields.io/badge/Target%20SDK-36-orange)

## Features

- Landscape immersive fullscreen UI
- Dynamic Island
- Module menu
- Watermark, theme, config import/export
- English-only UI

## Build Requirements

- JDK 17
- Android SDK (Platform 36)
- Gradle 8.13+

## Build Instructions

Before building, you must configure your local Android SDK path in `local.properties`:

```bash
# 1. Configure SDK path
echo "sdk.dir=/path/to/Android/Sdk" > local.properties

# 2. Build Debug APK
./gradlew assembleDebug

# 3. (Optional) Build Release APK
# Ensure your signing configurations are set up in app/build.gradle first
./gradlew assembleRelease
```

## Output

- **Debug APK:** `app/build/outputs/apk/debug/app-debug.apk`
- **Release APK:** `app/build/outputs/apk/release/app-release.apk` (signed)

## Notes

- This repository is primarily the UI layer. Game-side behavior depends on the hooked / native side of your environment.
- No source comments are included by design.
- Credit: forked from ZuoUI by 1mAcat.
