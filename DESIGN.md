# zaviv type — UI design notes

Adapted from the HyperType instrument-panel layout, re-skinned with the
**zaviv design system** (`../zaviv-design-system`).

## Principles

1. **Warm dark shell** — not pure OLED black; Zaviv dark `#1a1715` with raised
   cards `#23201d` and soft fields `#2a2622`.
2. **Monochrome primary actions** — Add / commit buttons are cream on dark;
   terracotta is reserved for switches-on, focus rings, live status, and chords.
3. **Flat sections** — hairline separators, no heavy card chrome (keeps the
   phone-portrait 480×854 density).
4. **Wordmark** — lowercase `zʌviv type`, medium weight, `letter-spacing: 0.065em`.

## Tokens (CSS)

Mapped in `src/styles.css`:

| Role | Value |
|------|--------|
| `--bg` | `#1a1715` |
| `--raise` / `--field` | `#23201d` / `#2a2622` |
| `--ink` / `--ink-2` | `#f4f1eb` / `#b6aea2` |
| `--accent` | `#d97757` |
| `--accent-ink` | `#e5a081` |
| `--primary` | `#f4f1eb` (button fill) |
| `--danger` | `#ec6a6a` |

Canonical tokens also live in `src/tokens.css` (copied from the design system).

## Logo

| Asset | Use |
|-------|-----|
| `zaviv-default.svg` | Canonical mark: white `zʌviv` on `#0f1115` rounded tile |
| `src/assets/logo.svg` | Titlebar (copy of `zaviv-default.svg`) |
| `src-tauri/icons/*` | Tray, window, NSIS installer (rasterized from the same mark) |

## Window

- 480 × 854, non-resizable, frameless
- Pre-paint background `#1a1715` (matches `main.rs` / `index.html`)
