# Android Install Notes

## Latest APK

~~~text
https://github.com/qiuqing005/paotuan-releases/blob/main/packages/yehang-paotuan-android-v0.2.8.apk?raw=1
~~~

## Install Steps

1. Download the APK to an Android phone.
2. Open the APK. If Android blocks unknown sources, allow installs from the current browser or file manager.
3. Open Yehang Paotuan from the launcher.
4. Allow microphone permission when entering voice features.

## Notes

v0.2.8 includes the native URL/config fix, room chat send acknowledgement, reply target validation, direct-message loading fixes, improved dice input, and the dedicated room Flow tab.

The app connects to the production service by default:

~~~text
https://38-76-162-111.sslip.io
wss://voice.38-76-162-111.sslip.io
~~~

If an older test APK is already installed and Android reports an update failure, uninstall the old APK first, then install v0.2.8.

## Verified

- APK signature verified with apksigner verify.
- APK metadata: package com.yehang.paotuan, versionCode 12, versionName 0.2.8.
- APK bundle contains assets/www/index.html, assets/www/native-config.js, compiled JS, and compiled CSS.
- Android emulator screenshot checked after install.