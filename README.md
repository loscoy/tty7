# Settings nested-scroll regression screenshots

Actual macOS application screenshots from the `fix/nested-scroll-conflict` working tree, based on upstream `d3887cd5f201220e268ff53b7dcd62f4a5245880`, before the unchanged fix was rebased onto upstream `4d33021c` as `c527c3be`.

- Page: Settings → Integrations; Simplified Chinese; light theme.
- Window: 960 × 700 points; screenshots: 1920 × 1400 pixels (Retina).
- Isolated development configuration; no agent hooks installed or modified.
- `list-boundary.png`: the list is at the bottom and the settings page has scrolled to show the command-line section.
- `button-shadow.png`: filtered list with the Install button shadow visible outside the original list edge.

The screenshots verify appearance; automated GPUI event-dispatch tests separately verify boundary handoff and that a single event never scrolls both containers.
