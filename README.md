<p align="center">
  <img src="iterm-kiwi.png" alt="Minimal Kiwi for iTerm2 logo" width="160">
</p>

# Minimal Kiwi for iTerm2

An [iTerm2](https://iterm2.com) color preset ported from the [Minimal Kiwi](https://github.com/pranjal-barnwal/minimal-kiwi) VSCode theme, so your terminal matches your editor

## What's included

- **`Minimal Kiwi.itermcolors`**: an iTerm2 color preset with the 16 ANSI colors plus background, foreground, bold, cursor, selection, link, badge and tab colors.

## Install

1. Get the preset, either by downloading [`Minimal Kiwi.itermcolors`](Minimal%20Kiwi.itermcolors) or by cloning the repo:
   ```sh
   git clone https://github.com/raph2121/minimal-kiwi-iterm.git
   ```
2. In iTerm2, open **Settings → Profiles → Colors**.
3. Click **Color Presets… → Import…** and pick `Minimal Kiwi.itermcolors`.
4. Select **Minimal Kiwi** from **Color Presets…**.

> Tip: double-clicking the `.itermcolors` file also imports it into iTerm2. You still need to select it in step 4.

## Verify

Print the 16 ANSI colors to check the preset is active:

```sh
for i in {0..15}; do printf "\e[48;5;${i}m  "; done; printf "\e[0m\n"
```

## Palette

The ANSI colors come straight from the VSCode theme's `terminal.*` keys, so iTerm2 looks just like VSCode's integrated terminal. Settings that only iTerm2 has, such as bold, links and selected text, use the theme's editor colors. VSCode's semi-transparent selection color (`#61616150`) is blended onto the background, because iTerm2 doesn't support transparent selection colors.

| Role | Normal | Bright |
|---|---|---|
| Black | `#1d1f21` | `#a8b4a8` |
| Red | `#ff6969` | `#ff6969` |
| Green | `#6fc674` | `#6fc674` |
| Yellow | `#ffbb6c` | `#ffbb6c` |
| Blue | `#78dcf3` | `#78dcf3` |
| Magenta | `#a36ac7` | `#a36ac7` |
| Cyan | `#78dcf3` | `#78dcf3` |
| White | `#c5c8c6` | `#ffffff` |

| UI | Color |
|---|---|
| Background | `#191a1b` |
| Foreground | `#c5c8c6` |
| Bold / selected text | `#ecffff` |
| Cursor / cursor text | `#f4d35e` / `#c7ffd9` |
| Selection | `#303031` |
| Links | `#82cd64` |

## Thanks

All credit for the colors goes to [pranjal-barnwal](https://github.com/pranjal-barnwal), the original author of the [Minimal Kiwi](https://github.com/pranjal-barnwal/minimal-kiwi) VSCode theme. This project just carries their palette over to iTerm2. If you like it, go give the original a ⭐.

## License

[MIT](LICENSE)
