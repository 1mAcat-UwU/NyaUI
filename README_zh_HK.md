[English](README.md) | [繁體中文（香港）](README_zh_HK.md)

# NyaUI

> [!IMPORTANT]  
> **免責聲明：** 使用或分發本項目前，請務必先閱讀 [免責聲明](Disclaimer_免責聲明_zh_HK.md)。

一個Android UI客戶端

![Package](https://img.shields.io/badge/Package-com.nyaui.me-blue)
![Min SDK](https://img.shields.io/badge/Min%20SDK-31-green)
![Target SDK](https://img.shields.io/badge/Target%20SDK-36-orange)

## 功能特色

- 動態島
- 等......

## 構建需求

- JDK 17
- Android SDK (Platform 36)
- Gradle 8.13+

## 構建說明

### 方式一：使用 Android Studio（電腦）

1. 開啟 **Android Studio**。
2. 點選 **File -> Open**，選擇項目根目錄。
3. Android Studio 會自動產生 `local.properties` 檔案並設定 SDK 路徑。
4. 點選 **Build -> Build Bundle(s) / APK(s) -> Build APK(s)**。
5. 構建完成後，點擊通知裏的 "locate" 即可找到 APK。

### 方式二：使用命令列（適用於所有平台）

在命令列構建前，必須在項目根目錄的 `local.properties` 中設定Android SDK路徑：

- **macOS / Linux / Termux:**
  `sdk.dir=/path/to/Android/Sdk`
- **Windows:**
  `sdk.dir=C\:\\Users\\YourName\\AppData\\Local\\Android\\Sdk`

**1. 構建 Debug 版 APK:**
- **macOS / Linux / Termux:** `./gradlew assembleDebug`
- **Windows:** `gradlew.bat assembleDebug`

**2. 構建 Release 版 APK:**
*（請先在 `app/build.gradle` 中設定好簽名資訊）*
- **macOS / Linux / Termux:** `./gradlew assembleRelease`
- **Windows:** `gradlew.bat assembleRelease`

## 輸出路径

- **Debug APK:** `app/build/outputs/apk/debug/app-debug.apk`
- **Release APK:** `app/build/outputs/apk/release/app-release.apk`（已簽名）

## 備註

- 此倉庫主要為UI層，遊戲端行為依賴於 Hook / 原生環境。
