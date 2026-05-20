# Android Install Notes

## Latest APK

Download and install:

```text
https://github.com/qiuqing005/paotuan-releases/releases/download/v0.2.2/yehang-paotuan-android-v0.2.2.apk
```

## Install Steps

1. Download the APK to an Android phone.
2. Open the APK. If Android blocks unknown sources, allow installs from the current browser or file manager.
3. Open "夜航跑团桌" from the launcher.
4. Allow microphone permission when entering voice features.

## Notes

`v0.2.2` fixes the Android avatar upload button. It was tested in an Android emulator: tapping "选择图片" opens the system DocumentsUI image picker, selecting an image returns to the app, and saving the profile succeeds.

The app connects to the production service by default:

```text
https://38-76-162-111.sslip.io
wss://voice.38-76-162-111.sslip.io
```

If you previously installed an older test APK and Android reports an update failure, uninstall the old APK first, then install `v0.2.2`.

## Verified

- `npm run test` passed.
- `npm run build` passed.
- APK signature verified with `apksigner verify`.
- APK metadata: package `com.yehang.paotuan`, versionCode `6`, versionName `0.2.2`.
- Android UI screenshots checked for login, profile, image picker, selected avatar, and saved avatar state.
