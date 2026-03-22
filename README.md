# Panel Auto Hide

Automatically hides the panel (terminal, output, problems) when you switch to an editor tab.

## Why

VS Code's panel can get in the way — especially on smaller screens. With `"workbench.panel.opensMaximized": "always"`, the panel takes up the entire editor area. This extension closes it automatically when you switch to a file, so you don't have to manually dismiss it every time.

## How it works

When the active text editor changes (you open a file, click a tab, follow a link from terminal), the panel closes automatically.

## Settings

| Setting | Default | Description |
|---|---|---|
| `panelAutoHide.enabled` | `true` | Enable or disable automatic panel hiding |

## Recommended setup

Add this to your `settings.json` for a fullscreen-or-nothing panel experience:

```json
"workbench.panel.opensMaximized": "always"
```

## License

MIT
