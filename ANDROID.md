# Android 安装说明

## 安装包

下载并安装：

```text
https://github.com/qiuqing005/paotuan-releases/releases/download/v0.2.0/yehang-paotuan-android-v0.2.0.apk
```

## 安装步骤

1. 把 APK 下载到 Android 手机。
2. 点开 APK。如果系统提示来源未知，允许当前浏览器或文件管理器安装未知来源应用。
3. 安装后从桌面图标打开“夜航跑团桌”。
4. 首次进入语音页时，允许麦克风权限。

## 说明

`v0.2.0` APK 已签名，包名为 `com.yehang.paotuan`。应用内置编译后的前端资源，默认连接线上服务：

```text
https://38-76-162-111.sslip.io
wss://voice.38-76-162-111.sslip.io
```

如果你要连接自建服务器，在登录/注册页点“服务器”，填入自建后端地址后保存。正式使用建议配置 HTTPS；局域网临时内测可使用 HTTP。语音服务地址由后端返回，客户端不需要单独填写。

如果手机无法加入语音，优先检查麦克风权限、Android System WebView 版本，以及网络是否屏蔽 UDP 或 WebRTC。

如果之前安装过旧测试包且提示更新失败，请先卸载旧版再安装 `v0.2.0`。

## 已实测

- Android 模拟器已安装并启动到登录页。
- APK 已通过 `apksigner verify`。
- 移动端大厅、社交、房间地图和语音页已截图检查。
