# Windows 安装说明

## 安装包

下载并运行：

```text
https://github.com/qiuqing005/paotuan-releases/releases/download/v0.1.0/yehang-paotuan-windows-v0.1.0.exe
```

## 安装步骤

1. 双击 EXE 安装器。
2. 选择安装目录并完成安装。
3. 从开始菜单或桌面快捷方式打开“夜航跑团桌”。
4. 首次加入语音时，允许麦克风权限。

## 说明

这个 Windows 客户端是 Electron 桌面壳，直接连接线上 HTTPS 跑团服务：

```text
https://38-76-162-111.sslip.io
```

语音使用 LiveKit / WebRTC：

```text
wss://voice.38-76-162-111.sslip.io
```

因为当前包没有商业代码签名证书，Windows SmartScreen 可能提示未知发布者。确认文件来自本仓库后，可以在提示里选择继续运行。
