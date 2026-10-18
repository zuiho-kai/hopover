<p align="center"><img src="icon.png" width="112" alt="Hopover"></p>
<h1 align="center">Hopover</h1>

<p align="center">
  <b>One keyboard and mouse for your Mac and your Windows PC — and drag files right across the screen edge.</b><br>
  <sub>English · <a href="README.zh.md">中文</a></sub>
</p>

<p align="center">
  <a href="https://github.com/zuiho-kai/hopover/releases/latest"><img alt="Download" src="https://img.shields.io/github/v/release/zuiho-kai/hopover?label=download&color=2f80ed"></a>
  <img alt="macOS 14+" src="https://img.shields.io/badge/macOS-14%2B%20Apple%20Silicon-555">
  <img alt="Windows 10/11" src="https://img.shields.io/badge/Windows-10%20%2F%2011-555">
  <img alt="Free preview" src="https://img.shields.io/badge/preview-free-1a7f37">
</p>

<p align="center"><img src="docs/hero.jpg" width="820" alt="The cursor carries a file from the Mac screen into a folder on the Windows screen"></p>

A Mac and a Windows PC on the same desk? Hopover makes them feel like two screens of one computer:

- Move the mouse past the screen edge and you are on the other computer. The keyboard follows.
- Drag a file past the edge and drop it into **any folder** over there, not into Downloads for you to find later.
- The two computers talk directly over your local network. No account, no cloud.

<p align="center">
  <a href="https://github.com/zuiho-kai/hopover/releases/latest"><b>⬇ Download the latest release</b></a> ·
  <a href="https://hopover.pages.dev">Website</a> ·
  <a href="#get-started-in-three-steps">Get started</a> ·
  <a href="#how-it-compares">Compare</a> ·
  <a href="#faq">FAQ</a>
</p>

---

## What it does

### One keyboard and mouse, two computers

**Double-tap ⌃ Control** on the Mac to turn sharing on: move the Mac's mouse past the edge and you are on Windows, keyboard included. Double-tap again to turn it off so the cursor never wanders over by accident. Locking the screen turns it off too.

**A mouse on each computer works too** (0.9.2 and later): push the Windows mouse off the screen toward the Mac and it carries on there, files included. Touch the Mac's mouse and the Windows mouse goes back to Windows only.

### Drag a file over, drop it in any folder

<table>
  <tr>
    <td align="center" width="50%"><img src="docs/mac-dropzone.png" width="230" alt="Drop panel at the Mac screen edge"></td>
    <td align="center" width="50%"><img src="docs/win-card.png" width="380" alt="Inbox card on Windows"></td>
  </tr>
  <tr>
    <td align="center">Drag a file toward the edge and a drop panel appears.<br>Keep pushing and the file follows the cursor across.</td>
    <td align="center">Let go in any folder on the other side.<br>Didn't find a spot? The file waits on a card.</td>
  </tr>
</table>

- Works both ways: Mac → Windows and Windows → Mac.
- About **110 MB/s** on gigabit Ethernet. Dragging a big file to Windows: if you let go before it has arrived, you see the progress and it drops when done.
- Changed your mind? Drag it back without letting go.

### Just send a file

With sharing off, drop a file on the panel at the screen edge and a card pops up at the edge of the other screen: click it to show the file, or drag the card into any folder. This needs **no system permissions** at all.

<p align="center"><img src="docs/mac-card-receiving.png" width="380" alt="A card receiving a file, with progress"></p>

---

## Get started in three steps

**1. Install on both**

| | Requires | Install |
|---|---|---|
| **Mac** | Apple Silicon, macOS 14 or later | Open `Hopover-…-macos-arm64.dmg`, drag Hopover into Applications, open it |
| **Windows** | Windows 10 / 11, 64-bit | Unzip `Hopover-…-windows-x64.zip` to a permanent place, run `Hopover.exe` |

> Preview builds are not notarized or code-signed yet, so the system stops them once:
> on the Mac use **System Settings → Privacy & Security → Open Anyway**; on Windows **More info → Run anyway**.

**2. Pair once**

<img align="right" src="docs/win-pair-2.png" width="300" alt="Pairing window on Windows showing a 6-digit code">

On first launch Windows opens the pairing window and finds the Mac on your network:

1. Pick your Mac.
2. Say whether this PC sits to the left or the right of the Mac.
3. Both screens show the same 6-digit number. Check it matches and confirm on both.

No IP addresses, no sign-up. From then on both sides reconnect on their own.

<br clear="right">

**3. Use it**

- **Double-tap ⌃ Control** on the Mac to turn sharing on. The first time, macOS asks for Accessibility access; follow the prompt and Hopover picks up as soon as it is granted.
- Move over to Windows and work as usual. Drag files across the edge into any folder.
- Double-tap Ctrl on Windows, or ⌃ on the Mac, to turn sharing off.

---

## How it compares

| | Hopover | ShareMouse | Deskflow | Logitech Flow |
|---|---|---|---|---|
| Drag a file across the screen edge | **Yes, into any folder, both ways** | Standard / Pro editions only, not Free ([shop](https://www.sharemouse.com/shop/)) | No, removed in v1.22.0, May 2025 ([release notes](https://github.com/deskflow/deskflow/releases/tag/v1.22.0)) | Copy on one, paste on the other ([Flow](https://www.logitech.com/en-us/software/flow.html)) |
| Needs a specific mouse | **No** | No ([features](https://www.sharemouse.com/features/transfer-files-between-computers/)) | not listed | Yes, a Flow-supported Logitech mouse ([Flow](https://www.logitech.com/en-us/software/flow.html)) |
| Price | **Free during the preview** | Free edition / one-time license ([shop](https://www.sharemouse.com/shop/)) | Free, open source ([README](https://github.com/deskflow/deskflow#readme)) | not listed |

Synergy, the commercial distribution built on Deskflow, does not list file drag and drop on its [features page](https://symless.com/synergy/features). The full table, with a source link for every cell, is on the website: **[Hopover vs ShareMouse vs Deskflow vs Synergy vs Logitech Flow](https://hopover.pages.dev/compare/)**.

---

## FAQ

<details>
<summary><b>How do I drag files from Mac to Windows?</b></summary>

Install Hopover on both computers and pair them once. Double-tap ⌃ Control on the Mac to turn on sharing, drag the file past the screen edge onto Windows and let go in any folder. Windows → Mac works the same way. With sharing off, drop the file on the panel at the screen edge and it arrives as a card.
</details>

<details>
<summary><b>Does Deskflow support file drag and drop?</b></summary>

No. Deskflow removed drag and drop in [v1.22.0](https://github.com/deskflow/deskflow/releases/tag/v1.22.0) (May 2025) because it was broken on every platform. Hopover bundles Deskflow for the keyboard and mouse and adds its own file drag and drop on top.
</details>

<details>
<summary><b>Is there a free ShareMouse alternative with file drag and drop?</b></summary>

Hopover is free during the preview and includes dragging files into any folder on the other computer. In ShareMouse, File Drag & Drop is part of the paid Standard and Professional editions ([shop](https://www.sharemouse.com/shop/)). Hopover currently supports one Mac and one Windows PC.
</details>

<details>
<summary><b>Do I need a Logitech mouse, like Logitech Flow?</b></summary>

No, any mouse and keyboard work. Logitech Flow needs a Flow-supported Logitech mouse and moves files by copy and paste.
</details>

More questions are answered on the [website FAQ](https://hopover.pages.dev/#faq).

<details>
<summary><b>Why does it need Accessibility access?</b></summary>

Capturing the keyboard and mouse, sending them to the other computer, and holding a file for you during a drag all require macOS Accessibility access. Sending files with cards alone does not.
</details>

<details>
<summary><b>The cursor freezes over an administrator window on Windows?</b></summary>

Windows blocks normal programs from controlling windows that run as administrator. In the Windows tray menu choose **"让鼠标也能操作管理员窗口…"** (let the mouse control admin windows) and approve once (0.9.1 and later).
</details>

<details>
<summary><b>Is it safe?</b></summary>

- Pairing uses an ECDH key exchange plus a 6-digit comparison on both screens; the key never crosses the network.
- The keyboard and mouse channel uses TLS, and each side checks the other's certificate fingerprint, so passwords you type on Windows never cross the LAN in clear text.
- The file channel only accepts connections with the token derived at pairing, and refuses paths such as `..`.
</details>

<details>
<summary><b>Where do files go?</b></summary>

Into the folder where you let go. Files not dropped into a folder land in Downloads and show a card. You can change the receive folder from the menu bar / tray menu.
</details>

<details>
<summary><b>How do I report a problem?</b></summary>

Open an [issue](https://github.com/zuiho-kai/hopover/issues) and attach the logs from both sides:

- Mac: `~/Library/Logs/Hopover/hopover.log`, `deskflow.log`
- Windows: `%APPDATA%\Hopover\hopover.log`, `%APPDATA%\Hopover\deskflow\client.log`
</details>

### Current limits

- One Mac and one Windows PC on the same local network.
- Only the Mac's keyboard crosses over; the Windows mouse works on the Mac, the Windows keyboard not yet.
- Apple Silicon Macs only. Intel Macs are planned.

---

## Changelog

**0.9.3**
- Fixed (Windows): holding the mouse button against the edge (selecting text, dragging a slider) popped up the send panel; it now appears only for a file drag.
- Fixed (Windows): an occasional background-process crash stalled input and paused sharing for about 10 seconds (0.9.2 known issue).
- Fixed (Windows): Deskflow was sometimes not restarted after it exited.
- The Mac build only changes the version number.

**0.9.2**
- New: the Windows mouse can move onto the Mac and drag files straight into any Mac folder.
- Fixed: quitting Hopover on Windows left the mouse shared.
- Fixed: pushing a file into the edge with the Windows mouse did nothing; it now sends right away.
- Fixed: dragging to Windows and back to the Mac without letting go left a drag stuck on Windows.
- Improved: snappier edge crossing (250 ms → 100 ms); logs rotate at 1 MB.

**0.9.1**
- Fixed: on the Mac, turning sharing on sometimes did nothing until you tried again (the bundled Deskflow crashed at random on macOS 27).
- Fixed: a file dragged from the Mac to Windows sometimes bounced back to the Mac; with a fast hand, the drag could also turn into a click on another Windows app.
- Fixed: dragging to Windows and back to the Mac without letting go left a drag stuck to the cursor on Windows.
- New: the mouse can control administrator windows on Windows (turn it on in the tray menu).
- Improved: crossing the edge feels snappier (edge delay cut from 250 ms to 100 ms).
- Improved: logs rotate at 1 MB.

**0.9.0** — first public preview.

---

## Technical details

<p align="center"><img src="docs/how-it-works.en.svg" width="860" alt="Hopover architecture"></p>

- **Keyboard and mouse** are handled by the bundled [Deskflow](https://github.com/deskflow/deskflow) (GPL-2.0), run as a separate process: server on the Mac, client on Windows. Hopover generates its configuration and certificates, starts it when sharing turns on and stops it when sharing turns off.
- **Files** use Hopover's own TCP protocol (port 47820): a header first, the receiver answers `READY`, then the bytes go into `*.hopover-part` files that are renamed when complete.
- **Seamless drag**: Deskflow captures the mouse at the very front of the input pipeline, so the other computer never learns that the button is held. The moment the cursor arrives, Hopover injects one real button press and starts a native system drag; it ends when you really let go over there. OLE drag-and-drop on Windows, an AppKit dragging session on the Mac.
- **Pairing**: Windows broadcasts on UDP 47821 to find the Mac; both run ECDH P-256 with a commitment first; the 6-digit number is SHA-256(shared secret ‖ both messages), truncated and reduced; the token is an HMAC of the shared secret. Each side generates its own TLS certificate and only fingerprints are exchanged.
- **Administrator windows** (Windows): UIPI blocks input from normal programs. When enabled, a scheduled task runs an elevated helper that hosts the Deskflow client and injects input on Hopover's behalf; Hopover itself stays at normal integrity so dragging into Explorer keeps working.

## License

Hopover is free during the preview. Hopover itself is not open source.

Hopover bundles [Deskflow](https://github.com/deskflow/deskflow) 1.27.0 (GPL-2.0) as a separate program:

- **Windows** ships unmodified Deskflow.
- **Mac** ships a `deskflow-core` with one patch: every input-source (TIS/TSM) call runs on the main thread, fixing random crashes on macOS 27.

The complete source (`deskflow-1.27.0-source.tar.gz`) and the patch (`deskflow-1.27.0-tis-main-thread.patch`) are attached to every release; the full license text is `LICENSE-GPL-2.0.txt` inside each package.
