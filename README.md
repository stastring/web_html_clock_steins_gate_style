# web_html_clock_steins_gate_style
# DIVERGENCE METER // FG-204 (Steins;Gate Nixie Clock)

[简体中文](#简体中文) | [English](#english)

> **"Everything is the choice of Steins Gate. El Psy Kongroo."**  
> 一款零依赖、纯离线运行的《命运石之门》世界线变动率探测仪（辉光管时钟）单文件网页应用。专为桌面常亮摆件设计，完美兼容现代 PC / 安卓平板（如小米平板），并针对 **2012 年初代 iPad mini (A5 芯片 / iOS 8.4.1)** 进行了底层渲染与离线全屏适配。

---

## 简体中文

### 📂 仓库文件说明（点击直达）

| 文件名 | 适用设备 | 说明 |
| :--- | :--- | :--- |
| [`clock_modern.html`](./clock_modern.html) | PC / Mac / 小米平板 / 现代手机 | 完整视觉特效版，支持高帧率渲染与全交互面板 |
| [`clock_old_device.html`](./clock_old_device.html) | 老旧 iPad (iOS 8 ~ iOS 10 / A5 芯片) | 去除现代 CSS 变量，采用静态图层预渲染与 SVG 描边防填充修复，确保老设备流畅运行 |
| [`url.txt`](./url.txt) | 老旧 iOS 设备离线全屏专用 | 已编码的 Base64 `data:` 离线链接，用于绕过老版 Safari 沙盒限制并添加到主屏幕 |

### ✨ 核心功能

* **4 种运行模式**：实时时钟（支持 12H / 24H 切换）、世界线变动率探测仪（内置 `1.048596` 等经典世界线）、日期显示、25 分钟番茄专注钟。
* **4 套灯管配色**：经典辉光管橙红（Nixie Orange）、VFD 荧光青绿（VFD Cyan）、复古琥珀金（Amber）、魔眼猩红（Crimson）。
* **拟真交互与音效**：支持点击灯管触发“世界线变动”随机滚动动画、双击快速切换时钟/世界线模式，内置 Web Audio API 合成的机械继电器滴答音效（默认静音，可在控制栏开启）。
* **3 档夜间亮度遮罩**：底部控制栏支持一键切换 `100%` / `70%` / `40%` 屏幕亮度，适合夜间床头或桌面常亮摆放。

### 📱 老旧 iPad (iOS 8) 零网络全屏部署教程

由于 iOS 8 系统沙盒限制，Safari 无法直接读取本地 HTML 文件。可通过仓库内的 [`url.txt`](./url.txt) 实现永久离线全屏：

1. **传输文件**：通过爱思助手或 iTunes 文件共享，将 [`url.txt`](./url.txt) 导入 iPad 任意文档阅读器（如 *Documents 2*）。
2. **复制链接**：在 iPad 上打开 `url.txt`，**全选并拷贝**整段以 `data:text/html;charset=utf-8;base64,` 开头的文本。
3. **添加到主屏幕**：打开系统自带的 **Safari 浏览器**，在地址栏选择 **「粘贴并前往」**；待辉光管点亮后，点击地址栏旁的 **分享按钮 →「添加到主屏幕」**。
4. **摆件常亮设置**：从桌面点击新生成的图标即可进入无边框全屏；建议下拉/上滑控制中心开启 **「飞行模式」**，并在 **「设置 → 通用 → 自动锁定」** 中设为 **「永不」**。

---

## English

### 📂 Repository Files

| File | Target Devices | Description |
| :--- | :--- | :--- |
| [`clock_modern.html`](./clock_modern.html) | PC / Mac / Xiaomi Pad / Modern Tablets | Full visual effects version with high-FPS animations and interactive control dock |
| [`clock_old_device.html`](./clock_old_device.html) | Legacy iPads (iOS 8–10 / Apple A5 Chip) | Legacy WebKit compatible version using pre-rendered static SVG layers to eliminate lag and rendering bugs |
| [`url.txt`](./url.txt) | Legacy iOS Offline Full-Screen Shortcut | Pre-encoded Base64 `data:` URI to bypass old Safari local file sandboxing |

### ✨ Features

* **4 Display Modes**: Real-time Clock (12H/24H), Divergence Meter (featuring `1.048596` Steins Gate & other world lines), Calendar Date, and a 25-minute Pomodoro Focus Timer.
* **4 Tube Themes**: Classic Nixie Orange, VFD Cyan, Vintage Amber, and Crimson Red.
* **Tactile Feedback & Audio**: Tap the tubes to trigger a world-line scramble animation, double-tap to toggle between Clock and Divergence Meter, and toggle synthesized mechanical relay click sounds via Web Audio API.
* **3-Level Dimmer**: Built-in brightness overlay (`100%` / `70%` / `40%`) for comfortable nightstand or desk use.

### 📱 Deployment Guide for Legacy iPads (iOS 8.4.1)

Old iOS versions restrict Safari from opening local `.html` files directly. Use [`url.txt`](./url.txt) to create a standalone offline Web App:

1. Transfer [`url.txt`](./url.txt) to your iPad using a file manager app (e.g., *Documents*).
2. Open `url.txt` on the iPad, **Select All**, and **Copy** the entire `data:text/html;charset=utf-8;base64,...` string.
3. Open **Safari**, tap the address bar, and select **Paste and Go**.
4. Once the Nixie tubes light up, tap the **Share icon → Add to Home Screen**. Launch from the new Home Screen icon for a borderless full-screen experience (enable **Airplane Mode** and set **Auto-Lock to Never** for 24/7 desk display).

[↑ 返回顶部 / Back to Top](#divergence-meter--fg-204-steinsgate-nixie-clock)
