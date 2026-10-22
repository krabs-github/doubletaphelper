# DoubleTap Helper ⚡

A high-performance Windows system tray utility built in C# (.NET 8 WPF) that lets you create **rapid double-press keyboard shortcuts** (tapping any physical key twice within a customizable time window) to trigger standard hotkeys, launch applications, open URLs, run commands, control media/volume, or paste text snippets.

Designed with a modern, stylish Windows 11 Fluent Dark theme.

---

## ✨ Features

- **Double-Tap Detection**: Press any physical key twice rapidly (e.g., `2x CapsLock`, `2x Esc`, `2x F4`, `2x Space`, `2x Q`).
- **Interactive Key Recorder**: Click "Record Key" and simply press any key on your keyboard to instantly capture its Virtual Key code and readable name.
- **Configurable Suppression**: Choose whether the second keypress is consumed/suppressed (ideal for `CapsLock`, `Esc`, function keys) or passed through to the foreground application.
- **Adjustable Speed Threshold**: Visual slider ranging from 150 ms (super fast) to 600 ms (relaxed), defaulting to 300 ms.
- **Rich Action Types**:
  1. **Send Keystroke / Hotkey**: Simulates single or multi-modifier shortcuts (`Ctrl + Shift + Esc`, `Win + Shift + S`, etc.) via Win32 `SendInput`.
  2. **Launch Application**: Open executables with custom parameters and working directories.
  3. **Open URL / Document**: Opens websites or local documents in default system handlers.
  4. **Run Shell Command**: Executes terminal commands or scripts silently in the background.
  5. **System Controls**: Quick hardware toggles (Mute/Unmute, Volume Up/Down, Media Play/Pause, Next/Prev Track, Lock Workstation).
  6. **Insert Text Snippet**: Instantly injects snippet templates without corrupting the Windows clipboard.
- **System Tray Native**:
  - Minimizes cleanly to the Windows Notification Area.
  - Context menu with quick toggles (Open, Pause Shortcuts, Gaming Mode, Exit).
  - Closing the main window keeps the application running smoothly in the background.
- **Gaming Mode**: Automatically suppresses double-tap triggers whenever a full-screen game or app is active to avoid accidental triggers during gameplay.
- **Subtle On-Screen Display (OSD)**: Sleek, floating dark HUD badge that briefly appears to confirm shortcut activation.
- **Auto-Start with Windows**: Native toggle configuring `HKCU\Software\Microsoft\Windows\CurrentVersion\Run` with automated path self-healing.
- **Single-Instance Protection**: Named mutex ensures only one hook instance is running at any time.

---

## ⚖️ License
Proprietary Freeware License. Free for personal and commercial use. Redistribution, reselling, mirroring, and reverse engineering are strictly prohibited. See [LICENSE](file:///C:/Users/Krabs/Downloads/Development/Gitea-Repositories/Krabs-Labs/Misc/DoubleTapHelper/LICENSE) for full terms.

© 2026 Krabs. All rights reserved.
