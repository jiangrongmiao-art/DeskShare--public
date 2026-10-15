# DeskShare · macOS 高性能局域网桌面推流与全功能远程控制套件

[![Platform](https://img.shields.io/badge/Platform-macOS%2011.0%2B-blue.svg)](https://apple.com)
[![Architecture](https://img.shields.io/badge/Architecture-Apple%20Silicon%20(ARM64)-black.svg)](https://apple.com)
[![Engine](https://img.shields.io/badge/Engine-ScreenCaptureKit%20%2B%20CoreGraphics-orange.svg)]()
[![Zero Dependency](https://img.shields.io/badge/Dependency-Zero%20pip%20packages-success.svg)]()
[![Security](https://img.shields.io/badge/Security-Hardware--Bound%20%7C%20End--to--End%20Direct-brightgreen.svg)]()

> **DeskShare** 是一款专为 macOS 深度定制的极速局域网屏幕推流与全功能远程控制工具。采用 Apple 原生 ScreenCaptureKit 录屏加速与 CoreGraphics 亚像素事件注入，无需安装任何额外依赖，局域网内任意设备（Windows PC、iPad、Mac、手机浏览器）即开即控。

---

## 🌟 核心特性

- ⚡ **极致帧率与超低延迟**：集成 ScreenCaptureKit 原生采集引擎，全档位稳定 30fps 高清高速推流，画面不黑屏、不掉帧、CPU 占用极低。
- 🖱️ **亚像素级远程控制**：CoreGraphics 原生驱动鼠标平滑移动、点击、拖拽、平滑连续滚轮、Cmd/Ctrl/Alt Mac 专属快捷键与跨平台文本直接注入。
- 🌐 **跨平台 Web 免客户端**：无需在操控端安装任何客户端软件，局域网内任意设备浏览器直接打开专属链接即可实时低延迟操控。
- 🔒 **一机一密专属私密访问路径**：每台受控端设备开机基于硬件指纹生成持久固定的专属随机私密路径（`/s/<SECRET>`），设备重启关机永不变更，主机无需重复发送新链接，杜绝局域网代码进程反查与恶意端口扫描。
- 🍏 **原生 MenuBar 状态栏托盘**：常驻屏幕右上角菜单栏，随时查看在线设备、一键复制访问链接、无感热升级续期、一键开启紧急锁定。
- 🛡️ **安全零侵入与可选纯 IP 访问**：客户端默认 100% 运行在普通用户空间，绝不强行索要管理员密码（root），不擅自修改系统底层；同时支持托盘自选开启纯 IP 免端口模式（`http://<IP>/s/<SECRET>`）。
- 🎯 **卡密全自动在线兑换与秒级绑定**：支持闲鱼/发卡平台 16 位高熵卡密（`DS-ACT-XXXX-XXXX-XXXX`）一键兑换，云端秒级绑定硬件，无需繁琐报备机器码，随开随用。

---

## 📦 下载与安装 (Download)

请前往本仓库右侧的 **[Releases (发布页面)](../../releases)** 下载最新编译的正式安装包：

1. 下载 **`DeskShare_macOS_App.zip`**；
2. 双击解压得到 **`DeskShare.app`**；
3. 将 `DeskShare.app` 拖入「应用程序」文件夹（或放置在桌面直接双击运行）。

---

## 🔑 软件激活与使用指南

### 1. 极速全自动激活（推荐）
1. 双击运行 `DeskShare.app`，未授权时将自动弹出【商业授权激活】对话框；
2. 将购买后收到的 16 位卡密（格式形如 `DS-ACT-XXXX-XXXX-XXXX`）直接按 `⌘ + V` 粘贴到输入框中；
3. 点击 **【立即激活】**，云端边缘节点全自动完成一机一码绑定与数字签名，**软件直接启动进入推流，无需重启 App！**
4. *(离线备用方式)*：若管理员直接向您发放了完整授权码（`DS-LIC-V2...`）或 `license.key` 文件，直接粘贴或放置在 App 同级目录重新打开亦会自动识别。

### 2. 系统权限配置（仅需首次运行配置一次）
由于 macOS 安全防护机制，首次启动需在 **「系统设置」→「隐私与安全性」** 中允许两项权限：
- **屏幕录制 (Screen Recording)**：勾选 `DeskShare`（用于屏幕流捕获，缺少会导致画面黑屏）；
- **辅助功能 (Accessibility)**：勾选 `DeskShare`（用于鼠标键盘控制，缺少会导致无法远程点击）。

### 3. 局域网连接与远程操控
1. 启动后，受控端 Mac 屏幕右上角菜单栏将常驻 DeskShare 图标；
2. 系统已自动在剪贴板生成您的专属安全访问链接，形如：  
   `http://<受控Mac的局域网IP>:<安全端口>/s/<开机固定随机密钥>`  
   *(若开启了纯 IP 直连优化，则为：`http://<受控Mac的局域网IP>/s/<私密路径>`)*
3. 局域网内任意手机、平板、电脑直接打开该链接即可秒级操控！

---

## 📖 详细使用与排错手册

更多进阶设置、随行换码工具使用、网络配置、常见故障排查（如权限重置、黑屏解决）请查阅：  
👉 **[完整用户操作手册 (MANUAL.md)](./MANUAL.md)**

---

## 💬 获取授权与技术支持

如需获取商业授权许可码（License Key）、企业定制或技术支持，请联系管理员或提交 Issue：
- 📬 **GitHub Issues**：[提交工单反馈](../../issues)
- 💼 **商业授权咨询**：请联系软件提供方获取专属卡密激活凭据。

---

## ⚖️ 免责声明与合规使用条款 (Disclaimer & Compliance)

1. **合法用途**：本软件仅供个人多设备协同互联、家庭局域网管理以及获得明确授权的企业内部 IT 运维与技术支持使用。
2. **严禁滥用**：严禁将本软件用于任何未经目标主机所有者明确授权的远程监控、网络偷窥、侵犯个人隐私或从事任何危害计算机网络安全的行为。因违反本条款产生的法律后果均由使用者自行承担。
3. **隐私保障**：本软件推流与远程控制 100% 运行于本地局域网（P2P 直连），所有音画数据及按键鼠标指令绝不经由任何第三方公网服务器中转或存储，充分保障用户与企业的数据资产安全。
