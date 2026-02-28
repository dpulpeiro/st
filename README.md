# st - Simple Terminal

Custom build of st with boxdraw, ligatures, transparency, scrollback, and URL handling patches.

**Terminal mod key:** `Alt` (Mod1)
**Terminal mod + Shift:** `Alt+Shift`

## Keyboard Shortcuts

### Clipboard

| Shortcut | Action |
|---|---|
| `Alt+c` | Copy to clipboard |
| `Alt+v` | Paste from clipboard |
| `Alt+Shift+C` | Copy to clipboard |
| `Alt+Shift+V` | Paste from clipboard |
| `Shift+Insert` | Paste from clipboard / selection |

### Font Size (Zoom)

| Shortcut | Action |
|---|---|
| `Alt+Shift+PageUp` | Zoom in (+1) |
| `Alt+Shift+PageDown` | Zoom out (-1) |
| `Alt+Shift+Home` | Reset zoom |
| `Alt+Shift+Up` | Zoom in (+1) |
| `Alt+Shift+Down` | Zoom out (-1) |
| `Alt+Shift+K` | Zoom in (+1) |
| `Alt+Shift+J` | Zoom out (-1) |
| `Alt+Shift+U` | Zoom in (+2) |
| `Alt+Shift+D` | Zoom out (-2) |

### Scrollback

| Shortcut | Action |
|---|---|
| `Shift+PageUp` | Scroll up (full page) |
| `Shift+PageDown` | Scroll down (full page) |
| `Alt+PageUp` | Scroll up (full page) |
| `Alt+PageDown` | Scroll down (full page) |
| `Alt+k` | Scroll up (1 line) |
| `Alt+j` | Scroll down (1 line) |
| `Alt+Up` | Scroll up (1 line) |
| `Alt+Down` | Scroll down (1 line) |
| `Alt+u` | Scroll up (full page) |
| `Alt+d` | Scroll down (full page) |

### Transparency

| Shortcut | Action |
|---|---|
| `Alt+a` | Increase opacity (+0.05) |
| `Alt+s` | Decrease opacity (-0.05) |

### External Pipes

| Shortcut | Action |
|---|---|
| `Alt+l` | Open URL (st-urlhandler) |
| `Alt+y` | Copy URL (st-urlhandler) |
| `Alt+o` | Copy output (st-copyout) |

### Printer

| Shortcut | Action |
|---|---|
| `Ctrl+PrintScreen` | Toggle printer |
| `Shift+PrintScreen` | Print screen |
| `PrintScreen` | Print selection |

### Other

| Shortcut | Action |
|---|---|
| `Break` | Send break |
| `Alt+Shift+NumLock` | Toggle numlock |

## Mouse Shortcuts

| Button | Modifier | Action |
|---|---|---|
| Scroll Up | - | Scroll up (1 line) |
| Scroll Down | - | Scroll down (1 line) |
| Middle | - | Paste selection |
| Scroll Up | Shift | Send Page Up |
| Scroll Down | Shift | Send Page Down |

## Selection

Hold `Alt` while selecting for rectangular selection mode.

## Configuration

| Setting | Value |
|---|---|
| Font | JetBrains Mono NL Light, size 24 |
| Alt font | NotoColorEmoji, size 24 |
| Opacity | 0.8 (80%) |
| Color scheme | Gruvbox Dark |
| Cursor | Block |
| Tabs | 8 spaces |
| TERM | st-256color |
| Boxdraw | Enabled |
| Bell | Disabled |

## Patches

- **Boxdraw**: Pixel-perfect box drawing characters
- **Ligatures**: Font ligature support (requires libharfbuzz)
- **Alpha/Transparency**: Configurable background opacity
- **Scrollback**: Keyboard and mouse scrollback
- **Externalpipe**: Pipe terminal contents to external scripts
- **font2**: Secondary font for emoji/special characters
- Xresources support (pywal compatible)

## Installation

```
sudo make install
```

Requires `libharfbuzz` for ligatures and a composite manager (`picom`, `xcompmgr`) for transparency.
