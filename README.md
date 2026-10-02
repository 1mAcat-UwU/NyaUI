[English](README.md) | [繁體中文（香港）](README_zh_HK.md)

# NyaUI

> [!IMPORTANT]
> **Disclaimer:** Please read the [Disclaimer](Disclaimer_en.md) before using, modifying, redistributing, or developing based on this project.

An Android UI Client.

![Package](https://img.shields.io/badge/Package-com.nyaui.me-blue)
![Min SDK](https://img.shields.io/badge/Min%20SDK-31-green)
![Target SDK](https://img.shields.io/badge/Target%20SDK-36-orange)

## License

The NyaUI UI source code is licensed under the **GNU General Public License v3.0 (GPL-3.0)**.

The UI source code must remain compliant with the GPL-3.0 license when modified or redistributed.

Independent core functionality and non-GPL components may be distributed or kept closed-source under their respective licenses, provided that they remain properly separated from the GPL-licensed UI source code.

See the [LICENSE](LICENSE) file for the full license text.

## Features

- Dynamic Island
- HUD
- Module List
- Notifications
- Default UI
- Classic UI
- Configurable UI settings
- And others......

## Build Requirements

- JDK 17
- Android SDK (Platform 36)
- Gradle 8.13+

## Build Instructions

### Option 1: Using Android Studio (Desktop)

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

**2. Build Release APK:**
*(Ensure your signing configurations are set up in `app/build.gradle` first)*
- **macOS / Linux / Termux:** `./gradlew assembleRelease`
- **Windows:** `gradlew.bat assembleRelease`

## Output

- **Debug APK:** `app/build/outputs/apk/debug/app-debug.apk`
- **Release APK:** `app/build/outputs/apk/release/app-release.apk` (signed)

## Notes

- This repository primarily contains the NyaUI UI layer.
- Game-side behavior depends on the hooked / native side of your environment.
- Core functionality may be developed and distributed separately from the GPL-licensed UI layer.
