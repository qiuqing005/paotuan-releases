# 夜航跑团桌发布包

这个仓库只用于发布用户可直接安装的客户端包和说明文档，不包含项目源码。

## 当前版本

- 版本：`v0.1.1`
- 服务地址：`https://38-76-162-111.sslip.io`
- 语音地址：`wss://voice.38-76-162-111.sslip.io`
- 适用：10 人以内跑团内测

## 下载

- Android APK：[yehang-paotuan-android-v0.1.1.apk](https://github.com/qiuqing005/paotuan-releases/releases/download/v0.1.1/yehang-paotuan-android-v0.1.1.apk)
- Windows EXE：[yehang-paotuan-windows-v0.1.1.exe](https://github.com/qiuqing005/paotuan-releases/releases/download/v0.1.1/yehang-paotuan-windows-v0.1.1.exe)

## v0.1.1 改动

- Android APK 不再是 13KB 远程网页壳，已内置编译后的前端资源。
- 移动端新增骰子面板，支持 `1d100`、`1d20`、`2d6`、`1d6+1` 和自定义公式。
- 地图页新增 HP / SAN 快捷加减按钮。
- 房间创建可以填写房间名和规则。
- 修复移动端语音浮层遮挡地图页操作按钮的问题。

## 已验证

- HTTPS 应用健康检查返回 200
- LiveKit token 返回 `configured=true`，语音 URL 为 `wss://voice.38-76-162-111.sslip.io`
- Android APK 已签名并通过 `apksigner verify`
- APK 内确认包含 `assets/www/index.html`、JS 和 CSS
- Windows EXE 已由 Electron Builder 生成 NSIS 安装器
- 已截图检查移动端地图、聊天骰子、角色页 UI
