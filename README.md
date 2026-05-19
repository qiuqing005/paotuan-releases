# 夜航跑团桌发布包

这个仓库只用于发布 Android / Windows 可安装 PWA 包和说明文档，不包含项目源码。

## 当前版本

- 版本：`v0.1.0`
- 形态：PWA Web 包
- 内测地址：`http://38.76.162.111`
- 适用：10 人以内跑团内测

## 包体

- `packages/yehang-paotuan-android-pwa-v0.1.0.zip`
- `packages/yehang-paotuan-windows-pwa-v0.1.0.zip`

两份包体都基于同一套已编译 Web/PWA 产物，里面只有 `www/` 静态文件和平台安装说明，不含 TypeScript、React、Node 服务端、Docker 部署脚本等源码。

## 功能

- 账号注册、登录、会话恢复
- 房间列表与创建
- 地图、地形、棋子选择与移动
- 角色 HP / SAN 状态
- 团内聊天
- LiveKit / WebRTC 高清语音接入
- Android 三页结构：地图 / 聊天 / 角色
- Windows 桌面宽屏布局

## 重要说明

当前包是 PWA 包，不是原生 APK 或 EXE。Android 需要用 Chrome 安装 PWA，Windows 需要用 Edge/Chrome 安装 PWA。

浏览器麦克风权限和正式语音体验需要 HTTPS。当前 IP 内测地址可验证页面、接口和 LiveKit token；正式给玩家使用时建议绑定域名并启用 HTTPS。

