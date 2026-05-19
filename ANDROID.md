# Android 安装说明

## 在线安装

1. 用 Android Chrome 打开服务地址。
2. 浏览器菜单中选择“添加到主屏幕”或“安装应用”。
3. 安装后从桌面图标进入。

当前内测地址：

```text
http://38.76.162.111
```

正式使用语音时建议换成 HTTPS 域名，例如：

```text
https://app.example.com
```

## 使用包体自部署

1. 解压 `packages/yehang-paotuan-android-pwa-v0.1.0.zip`。
2. 将 `www/` 目录部署到 Web 服务根目录。
3. Web 服务需要把 `/api/*`、`/health`、`/socket.io/*` 反代到跑团后端。
4. LiveKit 语音需要服务端配置 `LIVEKIT_URL`、`LIVEKIT_API_KEY`、`LIVEKIT_API_SECRET`。

## 限制

当前不是 APK。后续如果要发布 APK，建议用 Capacitor 或 Trusted Web Activity 打包，并配置 Android 签名证书。

