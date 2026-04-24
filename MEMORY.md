# Project Memory: Anthracite

## Discoveries
- Theme uses aggressive `-webkit-text-fill-color: transparent` for gradient text on headings, `strong`, and `em`.
- No specific styling for MathJax/LaTeX exists, causing transparency inheritance issues.
- MathJax elements (SVGs/fonts) often ignore `text-decoration: line-through` from parent `<del>` or `.cm-strikethrough` tags.

## Blunders
- [2026-04-24] Missing MathJax resets in gradient-text rules. Root cause: Global `-webkit-text-fill-color: transparent` on `strong/em/hN` made nested math invisible. Fix: Explicitly reset math containers to `currentColor`.

## Structure
- `theme.css`: Core theme styles.
- `manifest.json`: Obsidian theme manifest.
- `README.md`: Documentation and features.
