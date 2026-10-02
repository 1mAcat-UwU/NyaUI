[English](README.md) | [繁體中文（香港）](README_zh_HK.md)

# NyaUI

An Android UI Client.

![Package](https://img.shields.io/badge/Package-com.nyaui.me-blue)
![Min SDK](https://img.shields.io/badge/Min%20SDK-31-green)
![Target SDK](https://img.shields.io/badge/Target%20SDK-36-orange)

## Features

- Dynamic Island
- And others...

## Build Requirements

- JDK 17
- Android SDK (Platform 36)
- Gradle 8.13+

## Build Instructions

### Option 1: Using Android Studio (Recommended for Desktop)

1. Open **Android Studio**.
2. Select **File -> Open** and navigate to the project root directory.
3. Android Studio will automatically generate the `local.properties` file and configure your SDK path.
4. Go to **Build -> Build Bundle(s) / APK(s) -> Build APK(s)**.
5. Once finished, click "locate" in the notification to find the APK.

### Option 2: Using Command Line (All Platforms)

Before building from the command line, you must configure your Android SDK path in `local.properties` located at the project root:

- **macOS / Linux / Termux:**
  `sdk.dir=/path/to/Android/Sdk`
- **Windows:**
  `sdk.dir=C\:\\Users\\YourName\\AppData\\Local\\Android\\Sdk`

**1. Build Debug APK:**
- **macOS / Linux / Termux:** `./gradlew assembleDebug`
- **Windows:** `gradlew.bat assembleDebug`

**2. (Optional) Build Release APK:**
*(Ensure your signing configurations are set up in `app/build.gradle` first)*
- **macOS / Linux / Termux:** `./gradlew assembleRelease`
- **Windows:** `gradlew.bat assembleRelease`

## Output

- **Debug APK:** `app/build/outputs/apk/debug/app-debug.apk`
- **Release APK:** `app/build/outputs/apk/release/app-release.apk` (signed)

## Notes

- This repository is primarily the UI layer. Game-side behavior depends on the hooked / native side of your environment.
- No source comments are included by design.
- Credit: forked from ZuoUI by 1mAcat.
