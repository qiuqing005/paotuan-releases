# Yehang Paotuan Releases

This repository contains install notes for user-installable packages. It does not contain project source code.

## Current Packages

- Android APK: [yehang-paotuan-android-v0.2.5.apk](https://github.com/qiuqing005/paotuan-releases/releases/download/v0.2.5/yehang-paotuan-android-v0.2.5.apk)
- Windows EXE: [yehang-paotuan-windows-v0.2.5.exe](https://github.com/qiuqing005/paotuan-releases/releases/download/v0.2.5/yehang-paotuan-windows-v0.2.5.exe)

## Default Server

```text
https://38-76-162-111.sslip.io
wss://voice.38-76-162-111.sslip.io
```

## v0.2.5

- Adds fixed-scroll chat layouts for direct messages and room chat, keeping the input box pinned while only the message list scrolls.
- Adds quick return-to-bottom buttons when reading older direct or room messages.
- Adds room-message reply references, clickable reply navigation, and selected-message actions for reply and targeted dice checks.
- Adds structured dice check results with success and failure badges beside the message author.
- Removes the unclear per-message arrow icon from room chat.

## v0.2.4

- Adds LiveKit voice auto-reconnect for network fluctuations, including token refresh, browser online/offline retry, and playback-state recovery after reconnect.
- Keeps ghost and empty rooms out of the default lobby while preserving closed rooms as personal history.
- Adds the closed-room list tab; previous participants can reopen closed rooms, ordinary players can remove only their own history, and room owners can delete the room.
- Moves room creation to the lobby header plus button and opens the existing creation flow in a dialog.
- Includes the latest mobile lobby and room-list UI fixes.

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
- Browser screenshots checked for direct chat scrolling, room chat scrolling, reply references, targeted dice checks, and dice success/failure badges.
