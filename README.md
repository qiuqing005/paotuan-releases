# 夜航跑团桌发布包

这个仓库只用于发布用户可直接安装的客户端包和说明文档，不包含项目源码。

## 当前版本

- 版本：`v0.1.2`
- 服务地址：`https://38-76-162-111.sslip.io`
- 语音地址：`wss://voice.38-76-162-111.sslip.io`
- 适用：10 人以内跑团内测

## 下载

- Android APK：[yehang-paotuan-android-v0.1.2.apk](https://github.com/qiuqing005/paotuan-releases/releases/download/v0.1.2/yehang-paotuan-android-v0.1.2.apk)
- Windows EXE：[yehang-paotuan-windows-v0.1.2.exe](https://github.com/qiuqing005/paotuan-releases/releases/download/v0.1.2/yehang-paotuan-windows-v0.1.2.exe)

## v0.1.2 改动

- Android APK 内置编译后的前端资源，不再是远程网页壳。
- Android 端实测修复系统状态栏遮挡、聊天输入框被底部导航挤出的问题。
- 移动端拆成地图、聊天、角色三个二级页面，地图保留棋子移动和 HP / SAN 快捷操作。
- 聊天页提供 `1d100`、`1d20`、`2d6`、`1d6+1` 和自定义骰子公式，掷骰结果写入团内记录。
- 语音面板接入 LiveKit / WebRTC，已连接后支持静音和断开，质量状态改为中文显示。
- Windows EXE 重新打包为 `v0.1.2`，连接同一个线上 HTTPS 服务。

## 已验证

- HTTPS 应用健康检查返回 200
- LiveKit token 返回 `configured=true`，语音 URL 为 `wss://voice.38-76-162-111.sslip.io`
- Android APK 已签名并通过 `apksigner verify`
- APK 内确认包含 `assets/www/index.html`、JS 和 CSS
- Android 15 x86_64 模拟器已安装并实际打开 APK
- 已截图检查 Android 地图、聊天掷骰、角色页和 LiveKit 语音连接
- Windows EXE 已由 Electron Builder 生成 NSIS 安装器
