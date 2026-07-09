# zaviv type

Instant text expansion for Windows — HyperType’s product, dressed in **zaviv** branding.

Type short triggers and expand them into phrases, addresses, signatures, and more.
Runs in the background from the system tray with a warm dark manager window.

## Stack

- Tauri 2 + SolidJS + Vite
- Rust expansion engine (Windows keyboard hooks)

## Develop

```bash
pnpm install
pnpm tauri dev
```

Frontend-only (mock API in the browser):

```bash
pnpm dev
```

## Build

```bash
pnpm dist
```

Installer output:

- `src-tauri/target/release/bundle/nsis/`

Launch minimized (tray only):

```bash
src-tauri/target/release/zaviv-type.exe --minimized
```

## Tray

Toggle **Enabled**, **Open zaviv type**, **Quit**.

## Data

- Snippets: `%APPDATA%\zaviv-type\snippets.json`
- Settings: `%APPDATA%\zaviv-type\settings.json`
- Log: `%APPDATA%\zaviv-type\zaviv-type.log`

Debug logging: set env `ZAVIV_TYPE_DEBUG=1`.

## Design

UI tokens follow the zaviv design system:

- Background `#1a1715`, cream ink `#f4f1eb`
- Accent terracotta `#d97757` / live `#e5a081`
- Primary buttons monochrome (cream on dark)
- Wordmark: `zʌviv type` with wide tracking
