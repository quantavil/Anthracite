# Anthracite

A dark, elegant Obsidian theme with gradient accents and refined typography.

## Features

- **Dual Theme Support**: Dark and light mode with cohesive color schemes
- **Gradient Typography**: Beautiful gradient headings and styled bold/italic text
- **Custom Syntax Highlighting**: Dracula-inspired code syntax colors
- **Refined UI Elements**: Custom scrollbars, checkboxes with animations, decorative horizontal rules
- **Blockquote Styling**: Elegant blockquotes with gradient backgrounds and nested support

## Installation

### Via BRAT (Recommended for Beta updates)
1. Install and enable the **BRAT** plugin from Obsidian's Community Plugins.
2. Go to `Settings` > `BRAT` > scroll down to the **Themes** section.
3. Click **Add Beta Theme** and enter: `quantavil/Anthracite`.
4. Once downloaded, go to `Settings` > `Appearance` and select **Anthracite** from the theme list.

### Manual Installation
1. Download `theme.css` and `manifest.json`.
2. Create a folder named `Anthracite` in your vault's `.obsidian/themes/` directory.
3. Move both files into the folder.
4. Open `Settings` > `Appearance` and select **Anthracite** from the Theme dropdown.

## Customization

The theme uses CSS custom properties for easy customization. Key variables are defined at the top of `theme.css`:

### Color Variables
```css
--text-accent: #0fb6d6;      /* Primary accent color (cyan) */
--text-sub-accent: #f4569d;  /* Secondary accent color (pink) */
--interactive-accent: #0fb6d6;  /* Primary interactive accent */
```

### Border Radius
```css
--radius-s: 4px;             /* Small corner radius */
--radius-m: 8px;             /* Medium corner radius */
--radius-round: 999px;       /* Circular elements */
```

## Screenshots

<!-- Add screenshots here -->

## Credits & References

This theme was developed with inspiration from:
- **[Iridium](https://github.com/philphilphil/obsidian-iridium-theme)** - For advanced color system and component styling
- **[Museifu Basic](https://github.com/museifu/obsidian-museifu)** - For custom backgrounds and Kanban styling

## Changelog

### v1.0.4
- Fixed checkbox alignment and text overlap in Live Preview (Editor).
- Replaced custom CSS checkmark with a clean, vector-sharp SVG checkmark.
- Cleaned up unused design tokens, line-number structures, and height limit classes.
- Resolved CM6 syntax highlighting operator color mappings and callouts RGB formatting.

### v1.0.2
- Initial release

## License

See [LICENSE](LICENSE) file for details.

## Author

**@quantavil**
- GitHub: [https://github.com/quantavil](https://github.com/quantavil)

## Contributing

Found a bug or have a suggestion? Please open an issue on GitHub.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/improvement`)
3. Commit your changes (`git commit -m 'Add some improvement'`)
4. Push to the branch (`git push origin feature/improvement`)
5. Open a Pull Request
