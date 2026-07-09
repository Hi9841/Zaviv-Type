# zaviv type

Resident text expander for Windows, branded with the **zaviv** design system.

A lean Rust core watches the keyboard; a SolidJS tray panel manages snippets.
Same product shape as HyperType — warm cream/ink UI, terracotta accents, and
the zʌviv wordmark instead of purple OLED chrome.

## What it does

- Type a short trigger (e.g. `gm`) → expand to a longer phrase anywhere in Windows
- Optional global shortcuts (e.g. `Ctrl+Shift+V`) that paste a snippet
- Runs from the system tray; frameless 480×854 manager window
- Insert modes: Auto / Paste / Type-out
- Import / export snippets as JSON

## Brand

| Item | Value |
|------|-------|
| Product name | **zaviv type** (UI wordmark: `zʌviv type`) |
| Package | `zaviv-type` |
| Bundle id | `ai.zaviv.type` |
| Data dir | `%APPDATA%\zaviv-type\` |
| Design source | `zaviv-design-system` (warm cream / dark, terracotta `#d97757`) |

## Stack

- **Frontend:** SolidJS + Vite + TypeScript
- **Shell:** Tauri 2 (tray, frameless window, autostart)
- **Core:** Rust keyboard hook + expansion engine (Windows)
