<div align="center">

# ✨ JellyThemes ✨

**Transform your Jellyfin into a cinematic experience**

*6 stunning dark themes. One click install. Pure elegance.*

[![GitHub Stars](https://img.shields.io/github/stars/kingchenc/JellyThemes?style=for-the-badge&logo=github&color=9333ea)](https://github.com/kingchenc/JellyThemes/stargazers)
[![jsDelivr Hits](https://img.shields.io/jsdelivr/gh/hm/kingchenc/JellyThemes?style=for-the-badge&logo=jsdelivr&label=jsdelivr%20Hits&color=ff5627)](https://www.jsdelivr.com/package/gh/kingchenc/JellyThemes)
[![License](https://img.shields.io/badge/License-GPL--2.0-blue?style=for-the-badge)](LICENSE)

**Version 2.0** · Jellyfin 10.10, 10.11 and 12

</div>

---

## Themes

| Theme | Color | Description |
|-------|-------|-------------|
| [Obsidian](Themes/Obsidian/) | Purple/Violet | Deep space with elegant violet accents |
| [Solaris](Themes/Solaris/) | Gold/Amber | Warm golden sun tones |
| [Nebula](Themes/Nebula/) | Cyan/Cosmic | Cool cosmic cyan vibes |
| [Ember](Themes/Ember/) | Orange/Fire | Fiery orange warmth |
| [Void](Themes/Void/) | Gray/Minimal | Pure black minimalism |
| [Phantom](Themes/Phantom/) | Slate/Ghost | Ghostly translucent slate |

---

## Quick Install

Go to **Dashboard > Branding > Custom CSS** and paste one of these.
On Jellyfin 10.10 and older, Custom CSS is under **Dashboard > General**.

> [!NOTE]
> The themes work with every display mode of Jellyfin 12: **Auto** (the new interface), **Desktop**, **Mobile** and **TV**. You find it under **User Settings > Display > Display Mode**.

### 🟣 Obsidian (Purple)

```css
@import url("https://cdn.jsdelivr.net/gh/kingchenc/JellyThemes@master/Themes/Obsidian/Obsidian.css");
```

<details>
<summary>📸 Preview</summary>
<br>
<img src="Themes/Obsidian/assets/preview/Obsidian.png" alt="Obsidian home page">
<img src="Themes/Obsidian/assets/preview/Obsidian-details.png" alt="Obsidian movie page">
</details>

---

### 🟡 Solaris (Gold)

```css
@import url("https://cdn.jsdelivr.net/gh/kingchenc/JellyThemes@master/Themes/Solaris/Solaris.css");
```

<details>
<summary>📸 Preview</summary>
<br>
<img src="Themes/Solaris/assets/preview/Solaris.png" alt="Solaris home page">
<img src="Themes/Solaris/assets/preview/Solaris-details.png" alt="Solaris movie page">
</details>

---

### 🔵 Nebula (Cyan)

```css
@import url("https://cdn.jsdelivr.net/gh/kingchenc/JellyThemes@master/Themes/Nebula/Nebula.css");
```

<details>
<summary>📸 Preview</summary>
<br>
<img src="Themes/Nebula/assets/preview/Nebula.png" alt="Nebula home page">
<img src="Themes/Nebula/assets/preview/Nebula-details.png" alt="Nebula movie page">
</details>

---

### 🟠 Ember (Orange)

```css
@import url("https://cdn.jsdelivr.net/gh/kingchenc/JellyThemes@master/Themes/Ember/Ember.css");
```

<details>
<summary>📸 Preview</summary>
<br>
<img src="Themes/Ember/assets/preview/Ember.png" alt="Ember home page">
<img src="Themes/Ember/assets/preview/Ember-details.png" alt="Ember movie page">
</details>

---

### ⚫ Void (Black)

```css
@import url("https://cdn.jsdelivr.net/gh/kingchenc/JellyThemes@master/Themes/Void/Void.css");
```

<details>
<summary>📸 Preview</summary>
<br>
<img src="Themes/Void/assets/preview/Void.png" alt="Void home page">
<img src="Themes/Void/assets/preview/Void-details.png" alt="Void movie page">
</details>

---

### 👻 Phantom (Slate)

```css
@import url("https://cdn.jsdelivr.net/gh/kingchenc/JellyThemes@master/Themes/Phantom/Phantom.css");
```

<details>
<summary>📸 Preview</summary>
<br>
<img src="Themes/Phantom/assets/preview/Phantom.png" alt="Phantom home page">
<img src="Themes/Phantom/assets/preview/Phantom-details.png" alt="Phantom movie page">
</details>

---

## Features

- Dark design with one accent color per theme, also in the dashboard, menus and the new Jellyfin 12 interface
- Floating glass top bar with blur, glowing cards and buttons on hover
- Login page as one glass card, with your own logo if you like
- Play button in the middle of cards, accent progress bars, pill tabs
- Item pages with a fading backdrop and a labelled Play / Resume button in your language
- Small and fast: one file of about 28 KB, no extra downloads
- Works in the browser, the desktop and mobile apps, on iOS and on TVs (Samsung, LG)
- Everything is on by default; anything can be switched off, see [Settings](#settings)

## Settings

Add a `:root { ... }` block **under** the `@import` line in Custom CSS and set what you want to change. For example:

```css
@import url("https://cdn.jsdelivr.net/gh/kingchenc/JellyThemes@master/Themes/Solaris/Solaris.css");

:root {
    --jt-header-backdrop: none;
    --jt-footer: none;
}
```

| Setting | Default | What it does |
|---------|---------|--------------|
| `--jt-header-backdrop` | `blur(14px) saturate(140%)` | Blur under the top bar. `none` turns it off |
| `--jt-header-gap` | `0.6em` | Space around the floating top bar. `0` makes it full width again |
| `--jt-header-radius` | `1em` | Corner radius of the top bar. Use `0` together with `--jt-header-gap: 0` |
| `--jt-glow` | accent glow | Glow around hovered cards. `none` turns it off |
| `--jt-glow-s` | accent glow | Glow of buttons. `none` turns it off |
| `--jt-motion` | `0.2s` | Speed of hover animations. `0s` turns them off |
| `--jt-card-radius` | `0.6em` | Corner radius of cards |
| `--jt-card-extra-buttons` | `flex` | Watched and favourite buttons on hovered cards. `none` hides them |
| `--jt-card-mini-buttons` | `flex` | Small play button on cards on phones. `none` hides it |
| `--jt-library-labels` | `block` | Names under the library cards on the home page. `none` hides them |
| `--jt-original-title` | `block` | Original title on item pages. `none` hides it |
| `--jt-detail-logo` | `block` | Logo on item pages. `none` hides it |
| `--jt-item-title` | `block` | Title on item pages. `none` hides it |
| `--jt-footer` | `block` | Theme name, version and author at the end of each page. `none` hides it |
| `--jt-login-text` | `""` | A heading on the login page, e.g. `"Welcome home"` |
| `--jt-login-bg` | `none` | Background picture of the login page, e.g. `url("https://...")` |
| `--jt-logo` | `normal` | Your own logo instead of Jellyfin's, in the top bar and on the login page, e.g. `url("https://...")`. See [Own logo](#own-logo) |
| `--jt-logo-height` | `1.25em` | Height of your logo in the Jellyfin 12 top bar, e.g. `2em` for a logo with text |
| `--jt-logo-banner` | `contain` | `0` hides Jellyfin's banner behind your logo in the classic layouts |
| `--jt-server-name` | `1` | `0` hides the server name next to the logo in the Jellyfin 12 top bar |

### Own logo

Put your logo somewhere online (as a PNG or SVG with a transparent background) and add:

```css
:root {
    --jt-logo: url("https://example.com/my-logo.png");
    --jt-logo-banner: 0;
}
```

If the logo already shows a name, also add `--jt-server-name: 0;` and make it bigger with `--jt-logo-height: 2em;`. The name next to the logo in Jellyfin 12 is your server name; you can change it under **Dashboard > General**.
### Faster on older TVs

All effects are on by default, also on TVs (Jellyfin's TV display mode). If a TV feels slow (older Samsung and LG models), turn blur, glow and animations off there. This only changes the TV display mode:

```css
:root {
    --jt-tv-blur: none;
    --jt-tv-glow: 0 0 0 3px var(--jt-accent);
    --jt-tv-glow-s: none;
    --jt-tv-motion: 0s;
}
```

### Inter font

The themes use Jellyfin's own font, so nothing extra has to load. For the Inter font, add this line **above** the theme's `@import` line:

```css
@import url("https://cdn.jsdelivr.net/npm/@fontsource-variable/inter@5.1.0/index.css");
```

## Compatibility

### Jellyfin
- Jellyfin 12 (tested on 12.4) in every display mode: Auto, Desktop, Mobile and TV
- Jellyfin 10.11
- Jellyfin 10.10

### Apps
Custom CSS only works in apps that show the Jellyfin web interface:

- Jellyfin Web in any modern browser (Chrome, Firefox, Safari, Edge)
- Jellyfin Media Player / Jellyfin Desktop
- Jellyfin for Android (phones and tablets)
- Jellyfin for iOS
- Jellyfin for LG webOS and Samsung Tizen TVs

Native apps draw their own interface and ignore Custom CSS, so the themes do not show up there. This includes Swiftfin, Jellyfin for Android TV / Fire TV, Findroid and Kodi.

## Contributing

Contributions are welcome! Here's how you can help:

1. **Fork** the repository
2. **Create** a feature branch (`git checkout -b feature/awesome-feature`)
3. **Commit** your changes (`git commit -m 'Add awesome feature'`)
4. **Push** to the branch (`git push origin feature/awesome-feature`)
5. **Open** a Pull Request

### Guidelines
- Test your changes on multiple devices (desktop, mobile, TV)
- Follow the existing code style and variable naming conventions
- Update documentation if needed
- Keep pull requests focused on a single feature or fix

## Feedback

Found a bug? Have a feature request? We'd love to hear from you!

[Open an issue](https://github.com/kingchenc/JellyThemes/issues)

## License

GPL-2.0 - See [LICENSE](LICENSE) for details.

## Star History

[![Star History Chart](https://api.star-history.com/svg?repos=kingchenc/JellyThemes&type=Date)](https://star-history.com/#kingchenc/JellyThemes&Date)

---

<div align="center">

Made with 💜 for the Jellyfin community 🎬✨

</div>
