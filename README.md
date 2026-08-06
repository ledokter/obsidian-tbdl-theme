# tbdl — Obsidian theme

An editorial news-magazine theme for Obsidian. Serif body type (Merriweather), condensed sans headings (Oswald), a signature yellow accent, a drop-cap on the first paragraph, styled lists, blockquotes, code, tables and callouts. Ships with the Google Material Icons font for use in notes, plus a dark variant.

## Features

- **Typography**: Merriweather for the body, Oswald for headings and the UI.
- **Editorial accents**: yellow (`#FFE200`) rules under H1, left bar on H2, blue H3, drop-cap on the first paragraph.
- **Lists**: square yellow bullet markers, Oswald blue ordered-list numerals.
- **Blockquotes**: yellow left bar on a soft cream background.
- **Code & tables**: styled code blocks, yellow header rows, themed frontmatter and callouts.
- **Material Icons**: the Google Material Icons font is loaded; use `<span class="material-icons">home</span>` in notes and callouts. Sizes (`.mi-sm`/`.mi-lg`/`.mi-xl`) and colors (`.mi-yellow`/`.mi-blue`/`.mi-muted`/`.mi-accent`) are provided.
- **Dark mode**: dedicated dark palette.
- **Editor gutter** colors via `--line-number-color` / `--gutter-background` (for the note's line-number gutter).

## Install

### From the community directory
1. Settings → Appearance → Themes → Manage → Browse community themes → search **tbdl** → install.
2. Select **tbdl** as the theme.

### Manually
Copy `manifest.json` and `theme.css` into `<vault>/.obsidian/themes/tbdl/`, then select the theme in Appearance.

## Showcase / screenshot

Open [`showcase.md`](showcase.md) in Obsidian (Reading view) to see every styled element at a glance — headings, drop-cap, lists, blockquote, callout, table, code, tags and Material Icons. It's the intended source for the store screenshot: set the window to ~512×288 (or screenshot and crop to 512×288) and replace `screenshot.png`.

## Recommended companion: line numbers in code blocks

Obsidian does not number lines inside code blocks natively. To get **copy-safe line numbers** (numbers that are not included when you copy the code), install the **[Codeblock Customizer](https://github.com/mugiwara85/CodeblockCustomizer)** plugin and enable its **"Enable line numbers"** option. Its gutter is non-selectable, so copying code never includes the numbers.

Suggested gutter colors to match this theme (set them in Codeblock Customizer → Appearance & Styling):

| Color | Light | Dark |
|---|---|---|
| Gutter text | `#b9b9b0` | `#5f5f5a` |
| Gutter active line | `#1d3566` | `#ffd84d` |
| Gutter background | `#f7f7f4` | `#1b1f23` |

This theme works on its own without any plugin; Codeblock Customizer is only needed for line numbers in code blocks.

## Material Icons usage

```html
<span class="material-icons">home</span>
<span class="material-icons mi-yellow mi-lg">star</span>
<span class="material-icons mi-blue">push_pin</span>
```

Icon names come from the [Material Icons catalog](https://mui.com/material-ui/material-icons/). The font loads from Google Fonts (cached after first load).

## License

MIT © ledokter