[English](README.md) | [繁體中文（香港）](README_zh_HK.md)

# NyaUI

> [!IMPORTANT]
> **免責聲明：** 使用、修改、分發或基於本項目進行二次開發前，請務必先閱讀 [免責聲明](Disclaimer_免責聲明_zh_HK.md)。

Minecraft Android 啟動器及 UI/HUD 框架。

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
- 可自訂 UI 設定
- 支援第三方 Client 開發
- 等...

## 安裝說明

請前往 [Releases](../../releases) 下載最新版本的 APK 安裝包。

> [!NOTE]
> **針對配備 Google 流動服務（GMS）的 Android 裝置（2027 年新政策）：**
> 由於 NyaUI 為獨立開源項目，未進行 Google 開發者身份實名驗證，自 2027 年 1 月起，通過 Google 認證的裝置（Android 8.0 及以上）可能會攔截直接安裝。未配備 GMS 的裝置（如中國大陸國行系統）則不受影響。
>
> 如需在 GMS 裝置上安裝，請選擇以下任一方式：
> - **方式一（系統原生解鎖）：** 前往 **設定 > 開發人員選項 > 來自未驗證開發者的應用程式**，開啟該選項並重新啟動手機，等待 24 小時後即可啟用永久側載權限。
> - **方式二（免等待即時安裝）：** 透過 **Shizuku**（配合支援 Shizuku 的安裝器，如 InstallerX）安裝，或連接電腦執行 `adb install app-release.apk` 進行安裝。

## 構建要求

- JDK 17
- Android SDK (Platform 36)
- Gradle 8.13+

## 構建説明

在命令列構建前，必須在項目根目錄的 `local.properties` 中設定 Android SDK 路徑：

- **macOS / Linux / Termux：** `sdk.dir=/path/to/Android/Sdk`
- **Windows：** `sdk.dir=C\:\\Users\\YourName\\AppData\\Local\\Android\\Sdk`

**Debug 版 APK：**

    ./gradlew assembleDebug

**Release 版 APK：**

    ./gradlew assembleRelease

（請先在 `app/build.gradle` 中設定有效的簽署資訊。）

Windows 請使用 `gradlew.bat` 代替 `./gradlew`。

## 輸出路徑

- **Debug APK：** `app/build/outputs/apk/debug/app-debug.apk`
- **Release APK：** `app/build/outputs/apk/release/app-release.apk`

## 備註

- NyaUI 提供 Minecraft 啟動器及通用 UI/HUD 框架。
- 第三方開發者可以基於 NyaUI 框架開發自己的 Client。
- 預設不包含特定 Client 的功能。
