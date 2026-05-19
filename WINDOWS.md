# Windows 安装说明

## 安装包

下载并运行：

```text
https://github.com/qiuqing005/paotuan-releases/releases/download/v0.2.0/yehang-paotuan-windows-v0.2.0.exe
```

## 安装步骤

1. 双击 EXE 安装器。
2. 选择安装目录并完成安装。
3. 从开始菜单或桌面快捷方式打开“夜航跑团桌”。
4. 首次进入语音页时，允许麦克风权限。

## 说明

`v0.2.0` Windows 客户端是 Electron 桌面应用，内置编译后的前端资源，默认连接线上 HTTPS 跑团服务：

```text
https://38-76-162-111.sslip.io
wss://voice.38-76-162-111.sslip.io
```

如果你要连接自建服务器，在登录/注册页点“服务器”，填入自建后端地址后保存。正式使用建议配置 HTTPS；局域网临时内测可使用 HTTP。

当前安装包没有商业代码签名证书，Windows SmartScreen 可能提示未知发布者。确认文件来自本仓库后，可以在提示里选择继续运行。

## 已实测

- Windows EXE 已由 Electron Builder 生成 NSIS x64 安装器。
- 桌面端大厅、剧本编辑器、房间地图和语音页已截图检查。
