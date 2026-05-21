# Yehang Paotuan Releases

This repository contains install notes for user-installable packages. It does not contain project source code.

## Current Packages

- Android APK: [yehang-paotuan-android-v0.2.8.apk](https://github.com/qiuqing005/paotuan-releases/releases/download/v0.2.8/yehang-paotuan-android-v0.2.8.apk)
- Windows EXE: [yehang-paotuan-windows-v0.2.8.exe](https://github.com/qiuqing005/paotuan-releases/releases/download/v0.2.8/yehang-paotuan-windows-v0.2.8.exe)

## Default Server

~~~text
https://38-76-162-111.sslip.io
wss://voice.38-76-162-111.sslip.io
~~~

## v0.2.8

- Fixes native URL routing by bundling native-config.js and native-runtime.json into Windows/Android packages.
- Adds native asset validation so packaged clients fail the build if index.html, JS, CSS, or runtime config are missing.
- Fixes room chat sending by waiting for Socket.IO acknowledgements and restoring the draft on failure.
- Keeps room chat available outside the preparation flow by adding a dedicated Flow tab instead of blocking every room tab before play starts.
- Fixes reply targets so invalid replyToId values fail clearly instead of silently sending an unlinked message.
- Improves dice input tolerance for common forms such as /r 1d100, 1d100<=60, and 1d20>=10.
- Fixes direct-message pagination and stale-request races that could overwrite the active conversation.

## v0.2.6

- Reworks the room flow around the real COC7 preparation sequence: module confirmation, module editing, recruitment, character creation, KP review, casting/import, and active play.
- Adds keeper-side character sheet review with notes, approval/rejection, and imported room character data.
- Adds player-side COC7 sheet drafting, saving, submission, review feedback, and script-character selection.
- Imports approved character attributes, derived HP/SAN/MP/MOV/DB/build, and skill totals into room characters and dice checks.
- Adds .ra COC7 checks against imported character attributes or skills, including success/failure result badges.

## Verified

- npm run build passed.
- npm test passed.
- Chat/reply/dice Playwright regression passed.
- Mobile lobby, map toast, room chat selection, floating room, home chat, and desktop lobby screenshots passed.
- APK signed and verified with apksigner verify.
- APK contains bundled assets/www/index.html, native-config.js, JS, and CSS.
- Windows packaged client opened paotuan://app/index.html.