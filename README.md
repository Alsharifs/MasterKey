# MasterKey

A CapsLock-powered toolbox for Windows. Press **CapsLock+Space** anywhere for a menu of 35 built-in utilities, and add your own in a single `.py` file.

**[⬇ Download the latest version](https://github.com/Alsharifs/MasterKey/releases/latest)**: portable, nothing to install, Windows 10/11 64-bit.

## Getting started

1. Download `MasterKey-v9.0-portable-win64.zip` from the [latest release](https://github.com/Alsharifs/MasterKey/releases/latest).
2. Extract it to a folder (for example `C:\Tools\MasterKey`). Don't run it from inside the zip.
3. Double-click **MasterKey.exe**. It appears in the system tray.

**Have Node.js?** Run `npx @alsharif/masterkey` instead. It downloads the latest release, checks its checksum and starts it.

| Shortcut | What it does |
| --- | --- |
| CapsLock+Space | Open the menu |
| CapsLock+P | Quick Search |
| CapsLock+M | Settings Manager |
| CapsLock+Esc | Reload MasterKey |

## Built-in utilities

**Text:** Text Transformer (83 changes: case, lists & tables, numbers & time, find & extract, encode) · Clipboard History · Smart Multi-Paster · Paster Shape · Language Converter · Text Backup · View Text Backups · Flying Scratchpad

**Screen:** Snipping Tool · Screenshot + Annotate · Screen Text Grabber · Screen Ruler · Monitor Dimmer · Turn Off Monitor

**Windows & apps:** Window Switcher · Window Layouts · Toggle Always On Top · Smart Launcher · Task Manager · Commander (run your saved .cmd/.bat/.ps1/.reg scripts)

**Work:** Outlook Templates · Table Formatter · Advanced To-Do List · Quick Capture Inbox · Unit & Date Calculator · Start Time Get · Smart Alarm · End Work Session

**System:** Settings Manager · Insomnia Mode · Show/Hide Hidden Files · Smart Deleter · Remove Taskbar Search Box · Toggle Run at Startup · Shutdown

## Add your own utility

Tray icon → **Add a Utility…** opens the `Utilities` folder. Copy `_template.py`, rename it (e.g. `type_date.py`), edit it in Notepad and press **CapsLock+Esc**. It shows up in the menu, in Quick Search and on its own CapsLock key. The folder's `How to add a utility.txt` explains everything.

## Good to know

- **"Windows protected your PC"**: the first time you start it, click **More info → Run anyway**. The exe isn't code-signed yet.
- **Antivirus:** MasterKey uses a keyboard and mouse hook so its CapsLock shortcuts work in every app, so some antivirus tools may be cautious about it. What you type is only kept briefly in memory to spot your hotstrings, written to disk only when you use the step recorder or Text Backup yourself, and never sent anywhere.
- **Your data** (settings, notes, to-do list, scripts, log) is saved in a **Master Config** folder next to `MasterKey.exe`. Copy the whole folder to move MasterKey to another PC. Saved passwords are encrypted for your Windows account, so on another PC or account type them again in CapsLock+M.
- **Internet:** the only internet use is downloading website icons for the menu. Offline, they show a globe icon.

## Checking your download

Each release includes a `.sha256` file. In PowerShell:

```powershell
Get-FileHash .\MasterKey-v9.0-portable-win64.zip -Algorithm SHA256
```

The result should match the hash in the `.sha256` file.

---

MasterKey is distributed as a ready-to-run download; the source code is not published in this repository. Icons are from [Lucide](https://lucide.dev) (ISC license, included in the download as `ICONS-LICENSE.txt`).
