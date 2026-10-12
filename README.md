<p align="center"><img src="icon.png" width="128" alt="Hopover"></p>
<h1 align="center">Hopover</h1>
<p align="center"><b>一张桌子，两台电脑。</b> One desk, two computers.<br>
Mac 和 Windows 共用一套键盘鼠标，文件直接拖进另一台电脑的任意文件夹。<br>
<a href="https://hopover.pages.dev">官网 hopover.pages.dev</a> · <a href="https://github.com/zuiho-kai/hopover/releases/latest">下载 Download</a></p>

---

## 它能做什么

- **鼠标划过屏幕边缘就到了另一台电脑**，键盘跟着过去。在 Mac 上双击 ⌃ Control 开关。
- **拖着文件过边界，直接放进对面的文件夹**——不是先传到「下载」再去找。千兆局域网实测约 110 MB/s。
- **只想传文件也行**：把文件拖到屏幕边缘，对面出一张卡片，点一下打开所在位置。不需要任何权限。
- **配对一次就好**：Windows 自动找到 Mac，两边核对同一个 6 位数字。不填 IP、不注册账号、不经过云。
- **安全**：配对用 ECDH + 数字比对，密钥不在网络上传输；键鼠通道 TLS 双向证书校验。

## 安装（预览版）

| | 要求 | 安装 |
|---|---|---|
| Mac | Apple 芯片，macOS 14+ | 打开 `.dmg`，把 Hopover 拖进「应用程序」再打开。提示无法验证开发者时：系统设置 → 隐私与安全性 → **仍要打开** |
| Windows | Windows 10/11 64 位 | 解压 `.zip` 到固定位置，双击 `Hopover.exe`。提示「已保护你的电脑」时：**更多信息 → 仍要运行** |

然后：Windows 会弹出配对窗口 → 选中你的 Mac → 选这台电脑在 Mac 的左边还是右边 → 两边核对 6 位数字都点确认。
在 Mac 上双击 ⌃ Control 打开鼠标跨屏，第一次会请你打开「辅助功能」权限，照提示做即可。

> 预览版还没有苹果公证和 Windows 代码签名，所以第一次打开要手动放行一次。

### 当前限制
- 一台 Mac + 一台 Windows，键盘鼠标接在 Mac 上，两台在同一局域网。
- Intel Mac、键鼠接在 Windows 上的用法在计划中。
- Windows 端以普通权限运行，无法操作「以管理员身份运行」的窗口和 UAC 弹窗。

## 反馈

遇到问题请开 [Issue](https://github.com/zuiho-kai/hopover/issues)，附上日志：
Mac `~/Library/Logs/Hopover/hopover.log`，Windows `%APPDATA%\Hopover\hopover.log`。

## English

Hopover shares one mouse and keyboard between a Mac and a Windows PC, and lets you drag a file across the screen
edge straight into any folder on the other machine. Pair once with a 6-digit code; no accounts, no cloud.
Preview builds are unsigned: on macOS use *System Settings → Privacy & Security → Open Anyway*, on Windows
*More info → Run anyway*. Requires an Apple Silicon Mac (macOS 14+) and Windows 10/11 x64 on the same LAN.

## 许可 License

Hopover 预览版免费使用。Hopover itself is proprietary freeware during the preview.

Hopover 内置未修改的 [Deskflow](https://github.com/deskflow/deskflow) 1.27.0（GPL-2.0），以独立进程运行，负责键鼠共享。
对应版本的完整源码随每个 Release 附带（`deskflow-1.27.0-source.tar.gz`），许可证见安装包内 `LICENSE-GPL-2.0.txt`。
Hopover bundles unmodified Deskflow 1.27.0 (GPL-2.0) as a separate program; its source is attached to every release.
