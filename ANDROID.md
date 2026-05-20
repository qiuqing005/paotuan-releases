# Android Install Notes

## Latest APK

```text
https://github.com/qiuqing005/paotuan-releases/releases/download/v0.2.5/yehang-paotuan-android-v0.2.5.apk
```

## Install Steps

1. Download the APK to an Android phone.
2. Open the APK. If Android blocks unknown sources, allow installs from the current browser or file manager.
3. Open "Yehang Paotuan" from the launcher.
4. Allow microphone permission when entering voice features.

## Notes

`v0.2.5` includes account, friend, chat, room invitation, password reset, Android forced-mobile layout, avatar upload, voice playback recovery, voice auto-reconnect, closed-room history fixes, fixed chat scrolling, reply references, and structured dice check result badges.

The app connects to the production service by default:

```text
https://38-76-162-111.sslip.io
wss://voice.38-76-162-111.sslip.io
```

If an older test APK is already installed and Android reports an update failure, uninstall the old APK first, then install `v0.2.5`.

## Verified

- APK signature verified with `apksigner verify`.
- APK metadata: package `com.yehang.paotuan`, versionCode `9`, versionName `0.2.5`.
- Mobile UI screenshots checked for direct chat scrolling, room chat scrolling, reply references, targeted dice checks, and dice success/failure badges.
