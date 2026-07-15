# Project: Anthracite

## Overview
Anthracite is an Obsidian theme designed for visual consistency across light and dark modes. It features a dark mode with deep space surfaces, cyan/rose accents, and Dracula-inspired code syntax, and a light mode with warm linen surfaces, teal/rose accents, and earthy code syntax. It integrates with Obsidian's Style Settings plugin and targets both Markdown Reading Mode and Live Preview (CodeMirror 6).

## Structure
Anthracite
├── theme.css            # Main stylesheet containing all CSS variables, themes, layouts, and overrides.
└── manifest.json        # Theme metadata (name, version, author, compatibility constraints).

## Conventions
- **Obsidian Compatibility:** Must support both Reading Mode (rendered HTML blocks) and Live Preview (CodeMirror 6/CM6 `.cm-line` elements).
- **Styling System:** Standard CSS using CSS Variables (Custom Properties) compatible with Obsidian's internal theme variables.
- **Simplicity:** Minimize over-engineered selectors and avoid remote font loading or legacy CSS conventions.

## Dependencies & Setup
- Built for Obsidian v1.1.0+ (requires modern Chromium/Electron runtime supporting modern features like `:has()`).
- Optional integration: Style Settings plugin (used via class-toggles declared in CSS comments).

## Critical Information
- **Obsidian Theme Variables:** Obsidian variables like `--callout-color` are comma-separated RGB triplets (`R, G, B`) rather than standard CSS color values. They must be wrapped in `rgb(var(--callout-color))` or `rgba(var(--callout-color), opacity)`.
- **Live Preview DOM (CM6):** Live Preview uses CodeMirror 6, where lines are formatted as `div.cm-line` under `.markdown-source-view.mod-cm6`. CM5 selectors like `pre.HyperMD-...` or `div.HyperMD-...-bg` are legacy and do not match the CM6 DOM.
- **Scrollbars:** Custom scrollbars use standard `::-webkit-scrollbar` pseudo-elements. Avoid setting standard `scrollbar-width` globally on `*` as it breaks custom WebKit scrollbars on Chromium.
- **Hitboxes:** Ensure absolutely positioned hitboxes (like task list checkboxes) match their visual representations to avoid dead click zones.

## Insights
- None.

## Blunders
- 2026-07-15 invalid tool call on MEMORY.md creation -> Tried using ArtifactMetadata on a non-artifact workspace file -> ArtifactMetadata should only be provided for files in the appDataDir brain directory.
