# Panel Auto Hide

Automatically hides the panel (terminal, output, problems) when you switch to an editor tab.

## The problem

If you prefer working with the panel in only two states — **fully maximized** or **completely hidden** — VS Code gets you halfway there with:

```json
"workbench.panel.opensMaximized": "always"
```

This ensures the panel always opens maximized. But there are cases where the panel still ends up minimized (half-height) instead of fully hidden:

- Opening a file from the Explorer while the panel is visible
- Clicking a file link in the terminal output
- Various other editor focus changes

In all these cases VS Code minimizes the panel to half-height instead of hiding it completely. You end up with a useless half-panel covering your code, and have to manually close it.

## The solution

This extension listens for editor focus changes and automatically **closes the panel completely** whenever you switch to a different editor tab. No more half-height panel state — it's either fullscreen or gone.

## Settings

| Setting | Default | Description |
|---|---|---|
| `panelAutoHide.enabled` | `true` | Enable or disable automatic panel hiding |

## Recommended setup

```json
"workbench.panel.opensMaximized": "always"
```

## License

MIT
