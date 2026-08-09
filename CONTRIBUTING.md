# Maintaining tbdl

Notes for regenerating the store screenshots, not needed to use the theme.

## Screenshots

`screenshot-light.png` / `screenshot-dark.png` are real Obsidian captures, not mockups.

- [`showcase-light.md`](showcase-light.md) → source for `screenshot-light.png`
- [`showcase-dark.md`](showcase-dark.md) → source for `screenshot-dark.png`

To export, for each file:

1. Open the note in Obsidian, in Reading view.
2. Toggle Settings → Appearance → Base color scheme to match the note (**Light** for `showcase-light.md`, **Dark** for `showcase-dark.md`).
3. Resize the Obsidian window (or just the crop) to a **16:9** ratio.
4. Screenshot and crop/scale to exactly **512×288 px**.
5. Save as `screenshot-light.png` / `screenshot-dark.png`.

`screenshot.png` — the main preview in the README and the community catalog submission — combines the two with a diagonal cut, not a plain vertical split: `screenshot-dark.png` as the base, with `screenshot-light.png` masked to a parallelogram covering the upper-right corner (top edge from x≈330 to x=512, bottom edge from x≈460 to x=512, on the 512×288 canvas) and composited on top.

## Releases

Every `manifest.json` version bump needs a matching GitHub release, tagged with the bare version number (`2.0.3`, not `v2.0.3`) — Obsidian's catalog installs assets from the release tagged with that exact version.
