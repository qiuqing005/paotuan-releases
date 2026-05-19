# 夜航跑团桌发布包

这个仓库只用于发布用户可直接安装的客户端包和说明文档，不包含项目源码。

## 当前版本

- 版本：`v0.1.0`
- 服务地址：`https://38-76-162-111.sslip.io`
- 语音地址：`wss://voice.38-76-162-111.sslip.io`
- 适用：10 人以内跑团内测

## 下载

- Android APK：[yehang-paotuan-android-v0.1.0.apk](https://github.com/qiuqing005/paotuan-releases/releases/download/v0.1.0/yehang-paotuan-android-v0.1.0.apk)
- Windows EXE：[yehang-paotuan-windows-v0.1.0.exe](https://github.com/qiuqing005/paotuan-releases/releases/download/v0.1.0/yehang-paotuan-windows-v0.1.0.exe)

## 功能

- 账号注册、登录、会话恢复
- 房间列表与创建
- 地图、地形、棋子选择与移动
- 角色 HP / SAN 状态管理
- 团内聊天记录
- LiveKit / WebRTC 高清语音接入
- Android 移动端三页结构：地图、聊天、角色
- Windows 桌面宽屏布局

## 已验证

- HTTPS 应用健康检查返回 200
- LiveKit token 返回 `configured=true`，语音 URL 为 `wss://voice.38-76-162-111.sslip.io`
- Android APK 已签名并通过 `apksigner verify`
- Windows EXE 已由 Electron Builder 生成 NSIS 安装器
- 已截图检查桌面端与移动端地图、聊天、角色、语音浮层 UI
