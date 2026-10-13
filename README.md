# DeskShare · macOS 高性能局域网桌面推流与全功能远程控制套件

[![Platform](https://img.shields.io/badge/Platform-macOS%2011.0%2B-blue.svg)](https://apple.com)
[![Architecture](https://img.shields.io/badge/Architecture-Apple%20Silicon%20(ARM64)-black.svg)](https://apple.com)
[![Engine](https://img.shields.io/badge/Engine-ScreenCaptureKit%20%2B%20CoreGraphics-orange.svg)]()
[![Zero Dependency](https://img.shields.io/badge/Dependency-Zero%20pip%20packages-success.svg)]()
[![Security](https://img.shields.io/badge/Security-Zero--Source--Leak%20%7C%20Ed25519%20%2B%20HMAC-brightgreen.svg)]()

> **DeskShare** 是一款专为 macOS 设计的极速局域网屏幕推流与全功能远程控制工具。采用 Apple 原生 ScreenCaptureKit 录屏加速与 CoreGraphics 亚像素事件注入，无需安装任何额外依赖，局域网内任意设备（Windows、iPad、Mac、手机浏览器）即开即控。

---

## 🌟 核心特性

- ⚡ **极致帧率与超低延迟**：集成 ScreenCaptureKit 原生采集引擎，全档位稳定 30fps 高速推流，画面不黑屏、不掉帧、CPU 占用极低。
- 🖱️ **亚像素级远程控制**：CoreGraphics 原生驱动鼠标平滑移动、点击、拖拽、平滑滚轮、Cmd/Ctrl/Alt 快捷键组合与文本注入。
- 🌐 **跨平台 Web 免客户端**：无需在操控端安装任何软件，局域网内浏览器直接打开链接即可实时观看与操控。
- 🍏 **原生 MenuBar 状态栏托盘**：常驻屏幕右上角菜单栏，随时查看在线设备、切换画质、一键锁定与退出。
- 🎯 **小白级极简激活交互**：支持智能剪贴板预填、一键复制机器码、直接粘贴激活码，一键激活并立即使用，无需重启。

---

## 📦 下载与安装 (Download)

请前往本仓库右侧的 **[Releases (发布页面)](../../releases)** 下载最新编译的正式安装包：

1. 下载 **`DeskShare_macOS_App.zip`**；
2. 双击解压得到 **`DeskShare.app`**；
3. 将 `DeskShare.app` 拖入「应用程序」文件夹（或直接双击运行）。

---

## 🔑 软件激活与使用指南

### 1. 极速三步激活
1. 双击运行 `DeskShare.app`，未授权时将自动弹出【商业授权激活】对话框；
2. **此时您的本机专属机器码已自动复制到剪贴板**，请将机器码发送给管理员获取专属激活码；
3. 复制管理员发放的激活码（以 `DS-LIC-V2.` 或 `DS-LIC.` 开头），切换回激活窗口，直接按 `⌘ + V` 粘贴并点击 **【立即激活】**；
4. 提示激活成功，**软件自动启动，无需重启 App！**

### 2. 系统权限配置（仅需首次运行配置）
由于 macOS 安全防护机制，首次启动需在 **「系统设置」→「隐私与安全性」** 中允许两项权限：
- **屏幕录制**：勾选 `DeskShare`（用于屏幕流捕获，缺少会导致画面黑屏）；
- **辅助功能**：勾选 `DeskShare`（用于鼠标键盘控制，缺少会导致无法远程点击）。

### 3. 局域网观看与控制
启动后，受控端 Mac 屏幕右上角菜单栏将常驻 DeskShare 图标。  
局域网内任意设备用浏览器打开控制地址即可使用：  
`http://<受控Mac的局域网IP>:8288`

---

## 📖 详细使用与排错手册

更多进阶设置、网络配置、常见故障排查（如权限重置、黑屏解决）请查阅：  
👉 **[完整用户操作手册 (MANUAL.md)](./MANUAL.md)**

---

## 💬 获取授权与技术支持

如需获取商业授权许可码（License Key）、企业定制或技术支持，请联系管理员或提交 Issue：
- 📬 **GitHub Issues**：[提交工单反馈](../../issues)
- 💼 **商业授权咨询**：请联系软件提供方获取专属机器码激活凭据。
