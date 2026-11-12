# Apple Liquid Glass — Discord Theme

An **Apple Liquid Glass** (iOS 26 / visionOS / macOS Tahoe inspired) theme for **BetterDiscord** and **Vencord**.

It combines separated floating islands with multi-layered optical glass bevels, chromatic edge dispersion, floating capsule toolbars, and iMessage-style compact message bubbles.

---

## Credits & Base Theme

This theme is built on top of the [**Midnight**](https://github.com/refact0r/midnight-discord) layout base by [**refact0r**](https://github.com/refact0r), which handles panel separation, macOS-style window controls, and Discord Visual Refresh layout structure.

* **Original Midnight repository:** [https://github.com/refact0r/midnight-discord](https://github.com/refact0r/midnight-discord)

---

## Features

* **3-Step Optical Liquid Glass Bevel:** Specular outer rim, dark refractive optical trough, and soft inward glass gradient on panels, buttons, and popouts.
* **Chromatic Edge Dispersion (`--chromatic-glass`):** Optional cyan/magenta/violet prismatic refraction along panel edges while keeping the center crystal clear.
* **Compact Message Bubbles (`--compact-messages`):** Fit-content message bubbles (similar to iMessage / Telegram) or full-width merged message groups.
* **Floating Input Capsule (`--floating-bars`):** The bottom message bar floats over scrolling messages with real-time backdrop blur.
* **Custom Parallax SVG Home Icon:** A two-layer counter-rotating Apple Liquid Prism icon in the top-left corner (with built-in 1-line presets for the classic Apple logo or a Liquid Glass Droplet).
* **Full Window Transparency Support:** Designed to work with transparent window enabled in BetterDiscord / Vencord so your desktop or wallpaper refracts through Discord.

---

## Installation

1. Download [`LiquidGlass.theme.css`](./LiquidGlass.theme.css) from this repository.
2. Place the file into your client's `themes` folder:
   * **BetterDiscord:** `Settings` → `Themes` → `Open Themes Folder`
   * **Vencord:** `Settings` → `Vencord` → `Themes` → `Open Themes Folder` (or paste the raw GitHub URL into `Online Themes`)
3. *(Recommended)* For true desktop blur-through, enable **Enable Transparency** in your client settings (`Settings` → `BetterDiscord` / `Vencord` → `Window Preferences` → `Enable Transparency`) and restart Discord.

---

## Customization

All visual settings and feature switches are documented right inside [`LiquidGlass.theme.css`](./LiquidGlass.theme.css) under the `body` and `:root` sections at the top of the file:

```css
body {
    --compact-messages: on;      /* on: fit-content bubbles | off: wide merged groups */
    --floating-bars: on;         /* on: floating bottom chatbar over messages */
    --floating-top-bar: off;     /* on: floating top channel header */
    --dynamic-glass-hover: on;   /* on: subtle micro-lift on hover */
    --toolbar-glass-islands: on; /* on: glass capsule around chatbar buttons */
    --chromatic-glass: on;       /* on: cyan/magenta chromatic dispersion on glass edges */
}
```

You can also adjust glass opacity (`--window-frost-opacity`, `--panel-glass-opacity`, `--message-glass-opacity`), blur strength (`--blur-strength`), edge glow intensity (`--glass-edge-glow`), corner radii, and switch the top-left Home icon directly in the file.

---

## License

Released under the [MIT License / Unlicense](./LICENSE) — free for anyone to use, modify, and redistribute for any purpose.
