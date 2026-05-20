# Yehang Paotuan Releases

This repository contains install notes for user-installable packages. It does not contain project source code.

## Current Packages

- Android APK: [yehang-paotuan-android-v0.2.3.apk](https://github.com/qiuqing005/paotuan-releases/releases/download/v0.2.3/yehang-paotuan-android-v0.2.3.apk)
- Windows EXE: [yehang-paotuan-windows-v0.2.3.exe](https://github.com/qiuqing005/paotuan-releases/releases/download/v0.2.3/yehang-paotuan-windows-v0.2.3.exe)

## Default Server

```text
https://38-76-162-111.sslip.io
wss://voice.38-76-162-111.sslip.io
```

## v0.2.3

- Adds login/register password visibility controls and email-code password reset.
- Moves friend management under Account, changes Social to Chat, and adds direct-message UI.
- Adds room friend invitation, realtime room list refresh, and visible close time for closed rooms.
- Replaces the room-header sign-out control with room invitation.
- Adds LiveKit audio playback recovery for Android/WebView autoplay blocking.
- Forces Android APK WebView into mobile layout, including larger-screen devices.
- Keeps Android avatar upload through the native image picker.

## Verified

- `npm run lint` passed.
- `npm run build` passed.
- `npm --workspace apps/server run test` passed.
- `npm --workspace apps/web run test` passed.
- `npm run smoke` passed.
- APK signed and verified with `apksigner verify`.
- Browser screenshots checked for mobile auth, mobile lobby, account, chat, room voice, and desktop lobby.
