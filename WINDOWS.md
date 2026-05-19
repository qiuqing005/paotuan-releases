# Windows 安装说明

## 在线安装

1. 用 Microsoft Edge 或 Chrome 打开服务地址。
2. 在地址栏或浏览器菜单中选择“安装此站点为应用”。
3. 安装后可以从开始菜单或桌面快捷方式进入。

当前内测地址：

```text
http://38.76.162.111
```

正式使用语音时建议换成 HTTPS 域名。

## 使用包体自部署

1. 解压 `packages/yehang-paotuan-windows-pwa-v0.1.0.zip`。
2. 将 `www/` 目录部署到 Web 服务根目录。
3. Web 服务需要把 `/api/*`、`/health`、`/socket.io/*` 反代到跑团后端。
4. 用户用 Edge/Chrome 打开部署地址后安装 PWA。

## 限制

当前不是 EXE/MSIX。后续如果要做真正 Windows 客户端，可以用 WebView2、Electron 或 Tauri 包装当前 PWA。

