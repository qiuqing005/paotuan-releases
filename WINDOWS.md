# Windows Install Notes

## Latest EXE

~~~text
https://github.com/qiuqing005/paotuan-releases/blob/main/packages/yehang-paotuan-windows-v0.2.8.exe?raw=1
~~~

## Install Steps

1. Download and run the EXE installer.
2. Choose an install directory and complete installation.
3. Open Yehang Paotuan from the Start menu or desktop shortcut.
4. Allow microphone permission when entering voice features.

## Notes

v0.2.8 is an Electron desktop client with the compiled frontend bundled inside. It opens the bundled paotuan://app/index.html renderer and uses the bundled native runtime config for the production service.

~~~text
https://38-76-162-111.sslip.io
wss://voice.38-76-162-111.sslip.io
~~~

To use a self-hosted backend, click Server on the login/register page, enter the backend URL, and save it.

This installer is not signed with a commercial publisher certificate, so Windows SmartScreen may show an unknown-publisher warning.

## Verified

- Windows EXE generated as an NSIS x64 installer with Electron Builder.
- Packaged client opened paotuan://app/index.html in verification.
- Desktop screenshot checked after launch.