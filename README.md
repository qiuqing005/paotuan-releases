# 夜航跑团桌发布包

这个仓库只用于发布用户可直接安装的客户端包和说明文档，不包含项目源码。

## 当前版本

- 版本：`v0.2.0`
- 服务地址：`https://38-76-162-111.sslip.io`
- 语音地址：`wss://voice.38-76-162-111.sslip.io`
- 适用：10 人以内跑团内测

## 下载

- Android APK：[yehang-paotuan-android-v0.2.0.apk](https://github.com/qiuqing005/paotuan-releases/releases/download/v0.2.0/yehang-paotuan-android-v0.2.0.apk)
- Windows EXE：[yehang-paotuan-windows-v0.2.0.exe](https://github.com/qiuqing005/paotuan-releases/releases/download/v0.2.0/yehang-paotuan-windows-v0.2.0.exe)

## v0.2.0 改动

- 新增邮箱注册和登录，打开软件后先进入登录/注册页。
- 登录后进入房间大厅，不再默认进入房间。
- 新增公开房/私密房，私密房只有房主好友可加入。
- 新增好友申请、同意和好友列表。
- 新增“我的”页，可修改用户名、头像和密码。
- 新增剧本库、文本剧本上传和剧本编辑器。
- 剧本编辑器支持地图、人物数量和参数、故事文本、骰子公式与概率。
- 房间内拆分为地图、聊天、角色、语音四个二级页。
- 语音页新增发言人系统降噪开关和每人本地收听音量滑条。

## 已验证

- 本地 `npm run build` 通过。
- 本地 `npm run smoke` 通过。
- 公网 `https://38-76-162-111.sslip.io` smoke 通过，LiveKit 返回 `configured=true`。
- Android APK 已签名并通过 `apksigner verify`。
- Android 模拟器已安装并启动到登录页。
- Playwright 已截图检查桌面端大厅、剧本编辑器、房间地图、语音页，以及移动端大厅、社交、房间地图、语音页。
- Windows EXE 已由 Electron Builder 生成 NSIS x64 安装器。
