# Yehang Paotuan Releases

This repository only contains user-installable packages and Markdown notes. It does not contain project source code.

## Current Packages

- Android APK: [yehang-paotuan-android-v0.2.2.apk](https://github.com/qiuqing005/paotuan-releases/releases/download/v0.2.2/yehang-paotuan-android-v0.2.2.apk)
- Windows EXE: [yehang-paotuan-windows-v0.2.0.exe](https://github.com/qiuqing005/paotuan-releases/releases/download/v0.2.0/yehang-paotuan-windows-v0.2.0.exe)

## Default Server

```text
https://38-76-162-111.sslip.io
wss://voice.38-76-162-111.sslip.io
```

## Android v0.2.2

- Fixes avatar upload on Android WebView.
- Tapping "选择图片" now opens the Android system image picker.
- Selecting an image returns to the app, loads a preview, and can be saved to the profile.
- APK metadata: package `com.yehang.paotuan`, versionCode `6`, versionName `0.2.2`.

If an older test APK is already installed and Android reports an update failure, uninstall the old APK first, then install `v0.2.2`.

## Email Delivery Note

The app server currently verifies that Cloud Mail is configured with `zhongsheng@yuelanshan.cloud`, but sending registration codes to external inboxes such as QQ still requires an external mail relay such as Resend or a real SMTP service. Cloudflare Email Routing is inbound routing/forwarding and is not an outbound SMTP service.

## Verified

- `npm run test` passed.
- `npm run build` passed.
- APK signed and verified with `apksigner verify`.
- Android emulator screenshots checked for login, profile, system image picker, selected avatar, and saved avatar state.
