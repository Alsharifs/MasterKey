# MasterKey

A CapsLock-powered toolbox for Windows. Press **CapsLock+Space** anywhere for a menu of 27 built-in utilities, and add your own in a single `.py` file.

**[⬇ Download the latest version](https://github.com/Alsharifs/MasterKey/releases/latest)**: portable, nothing to install, Windows 10/11 64-bit.

## Getting started

1. Download `MasterKey-v8.5-portable-win64.zip` from the [latest release](https://github.com/Alsharifs/MasterKey/releases/latest).
2. Extract it to a folder (for example `C:\Tools\MasterKey`). Don't run it from inside the zip.
3. Double-click **MasterKey.exe**. It appears in the system tray.

| Shortcut | What it does |
| --- | --- |
| CapsLock+Space | Open the menu |
| CapsLock+P | Quick Search |
| CapsLock+M | Settings Manager |
| CapsLock+Esc | Reload MasterKey |

## Built-in utilities

Advanced To-Do List · Clipboard History · End Work Session · Flying Scratchpad · Insomnia Mode · Language Converter · Monitor Dimmer · Remove Taskbar Search Box · Screen Ruler · Screen Text Grabber · Settings Manager · Show/Hide Hidden Files · Shutdown · Smart Alarm · Smart Deleter · Smart Launcher · Smart Multi-Paster · Snipping Tool · Task Manager · Text Backup · Text Transformer · Toggle Always On Top · Toggle Run at Startup · Turn Off Monitor · View Text Backups · Window Layouts · Window Switcher

## Add your own utility

Tray icon → **Add a Utility…** opens the `Utilities` folder. Copy `_template.py`, rename it (e.g. `type_date.py`), edit it in Notepad and press **CapsLock+Esc**. It shows up in the menu, in Quick Search and on its own CapsLock key. The folder's `How to add a utility.txt` explains everything.

## Good to know

- **"Windows protected your PC"**: the first time you start it, click **More info → Run anyway**. The exe isn't code-signed yet.
- **Antivirus:** MasterKey uses a keyboard and mouse hook so its CapsLock shortcuts work in every app, so some antivirus tools may be cautious about it. What you type is only kept briefly in memory to spot your hotstrings, written to disk only when you use the step recorder or Text Backup yourself, and never sent anywhere.
- **Your data** (settings, notes, to-do list, log) is saved in a **Master Config** folder next to `MasterKey.exe`. Copy the whole folder to move MasterKey to another PC. `Settings.ini` stores passwords as plain text, so keep it private.
- **Internet:** the only internet use is downloading website icons for the menu. Offline, they show a globe icon.

## Checking your download

Each release includes a `.sha256` file. In PowerShell:

```powershell
Get-FileHash .\MasterKey-v8.5-portable-win64.zip -Algorithm SHA256
```

The result should match the hash in the `.sha256` file.

---

MasterKey is distributed as a ready-to-run download; the source code is not published in this repository. Icons are from [Lucide](https://lucide.dev) (ISC license, included in the download as `ICONS-LICENSE.txt`).
