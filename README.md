# Rosé Pine Icons for Zed

A port of the [Rosé Pine VSCode icon theme](https://github.com/rose-pine/vscode) to [Zed](https://zed.dev). Minimalist by design: every file gets the same generic icon; folders share one open and one closed glyph.

## Install

### From the Zed extension registry

(Once published) Open the Extensions panel (`cmd+shift+x`), search for `Rosé Pine Icons`, click Install. Then in Settings → File Icon Theme, choose "Rosé Pine Icons".

### As a development extension

```bash
git clone https://github.com/ldakhoa/zed-rose-pine-icons.git
```

Then in Zed: Extensions panel → `Install Dev Extension` → select the cloned directory. Set the icon theme via Settings → File Icon Theme.

## Deviations from upstream

- **Chevrons remain visible.** The VSCode theme uses `hidesExplorerArrows: true`; Zed has no equivalent flag. If you want them gone, a follow-up release could ship transparent chevron SVGs.
- **`fileExtensions` map dropped.** Every entry in upstream's `fileExtensions` map points at the default file icon, so re-encoding them as Zed `file_suffixes` adds no information.

## Credit & license

- Original icon theme: [rose-pine/vscode](https://github.com/rose-pine/vscode)
- Zed port: ldakhoa1308
- License: MIT (see `LICENSE`)
