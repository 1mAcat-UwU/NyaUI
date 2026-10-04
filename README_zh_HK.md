[English](README.md) | [繁體中文（香港）](README_zh_HK.md)

# NyaUI

> [!IMPORTANT]
> **免責聲明：** 使用、修改、分發或基於本項目進行二次開發前，請務必先閱讀 [免責聲明](Disclaimer_免責聲明_zh_HK.md)。

一個 Android UI 客戶端。

![Package](https://img.shields.io/badge/Package-com.nyaui.me-blue)
![Min SDK](https://img.shields.io/badge/Min%20SDK-31-green)
![Target SDK](https://img.shields.io/badge/Target%20SDK-36-orange)

## 授權

NyaUI 的 UI 源碼採用 **GNU General Public License v3.0（GPL-3.0）** 授權。

對 UI 源碼進行修改或重新分發時，必須遵守 GPL-3.0 的相關授權要求。

獨立的核心功能及非 GPL 組件可以根據其自身授權條款進行分發或保持閉源，但必須與 GPL-3.0 授權的 UI 源碼保持適當的代碼及授權邊界。

完整授權條款請參閱 [LICENSE](LICENSE) 文件。

## 功能特色

- 靈動島
- HUD
- Default UI
- Classic UI
- 可自訂 UI 設置
- 模組分類及管理
- 等......

## 構建需求

- JDK 17
- Android SDK (Platform 36)
- Gradle 8.13+

## 構建説明

### 方式一：使用 Android Studio（電腦）

1. 開啟 **Android Studio**。
2. 點選 **File -> Open**，選擇項目根目錄。
3. Android Studio 會自動產生 `local.properties` 檔案並設定 SDK 路徑。
4. 點選 **Build -> Build Bundle(s) / APK(s) -> Build APK(s)**。
5. 構建完成後，點擊通知裏的 "locate" 即可找到 APK。

### 方式二：使用命令列（適用於所有平台）

在命令列構建前，必須在項目根目錄的 `local.properties` 中設定 Android SDK 路徑：

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

## 輸出路徑

- **Debug APK:** `app/build/outputs/apk/debug/app-debug.apk`
- **Release APK:** `app/build/outputs/apk/release/app-release.apk`（已簽名）

## 備註

- 此倉庫主要為 NyaUI UI 層。
- 遊戲端行為依賴於 Hook / 原生環境。
- 核心功能可以與 GPL-3.0 授權的 UI 層分開開發及分發。
