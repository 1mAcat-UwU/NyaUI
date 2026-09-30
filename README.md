# NyaUI

Android UI Client

Package: com.nyaui.me  
Version: 1.0.2  
Min SDK: 31 (Android 12)  
Target SDK: 36  

## Features

- Landscape immersive fullscreen UI  
- Dynamic Island (music / FPS)  
- Module menu (Combat, Movement, Player, Visual, World, Misc, Settings)  
- Watermark, theme, config import/export  
- FakeFps (Settings): override the FPS shown on the Dynamic Island  
- English-only UI  

## Build

Requirements: JDK 17, Android SDK (platform 36).

echo "sdk.dir=/path/to/Android/Sdk" > local.properties
./gradlew assembleDebug

APK output:

app/build/outputs/apk/debug/app-debug.apk

## Notes

- This repository is primarily the UI layer. Game-side behavior depends on the hooked / native side of your environment.  
- No source comments are included by design.  
- Credit: forked from ZuoUI by 1mAcat.
