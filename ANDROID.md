# Android 安装说明

## 安装包

下载并安装：

```text
https://github.com/qiuqing005/paotuan-releases/releases/download/v0.1.1/yehang-paotuan-android-v0.1.1.apk
```

## 安装步骤

1. 把 APK 下载到 Android 手机。
2. 点开 APK。如果系统提示来源未知，允许当前浏览器或文件管理器安装未知来源应用。
3. 安装后从桌面图标打开“夜航跑团桌”。
4. 首次加入语音时，允许麦克风权限。

## 说明

`v0.1.1` APK 已内置编译后的前端资源，不再只是远程 WebView 壳。应用内界面通过安全本地 HTTPS 资产加载，数据、同步和语音连接到线上服务：

```text
https://38-76-162-111.sslip.io
wss://voice.38-76-162-111.sslip.io
```

如果手机无法加入语音，优先检查系统麦克风权限、Android System WebView 版本、网络是否屏蔽 UDP 或 WebRTC。
