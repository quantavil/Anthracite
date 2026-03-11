# Anthracite

A dark, elegant Obsidian theme with gradient accents and refined typography.

## Features

- **Dual Theme Support**: Dark and light mode with cohesive color schemes
- **Gradient Typography**: Beautiful gradient headings and styled bold/italic text
- **Custom Syntax Highlighting**: Dracula-inspired code syntax colors
- **Refined UI Elements**: Custom scrollbars, checkboxes with animations, decorative horizontal rules
- **Blockquote Styling**: Elegant blockquotes with gradient backgrounds and nested support

## Installation

### From Obsidian Community Themes
1. Open Settings > Appearance
2. Click "Manage" next to Themes
3. Search for "Anthracite"
4. Click "Install and use"

### Manual Installation
1. Download `theme.css` and `manifest.json`
2. Create a folder named `Anthracite` in your vault's `.obsidian/themes/` directory
3. Move both files into the folder
4. Open Settings > Appearance and select "Anthracite" from the Theme dropdown

## Customization

The theme uses CSS custom properties for easy customization. Key variables are defined at the top of `theme.css`:

### Color Variables
```css
--text-accent: #0fb6d6;      /* Primary accent color (cyan) */
--text-sub-accent: #f4569d;  /* Secondary accent color (pink) */
--interactive-accent-rgb: 14 210 247;  /* RGB values for transparency */
```

### Typography
```css
--default-font: 'Rubik', sans-serif;
--code-mono-font: 'OperatorMonoSSmLig-Book', monospace;
--default-font-size: 18px;
```

### Border Radius
```css
--radius-s: 4px;
--radius-m: 8px;
--radius-l: 12px;
--radius-xl: 16px;
```

## Screenshots

<!-- Add screenshots here -->

## Credits & References

This theme was developed with inspiration from:
- **[Iridium](https://github.com/philphilphil/obsidian-iridium-theme)** - For advanced color system and component styling
- **[Museifu Basic](https://github.com/museifu/obsidian-museifu)** - For custom backgrounds and Kanban styling

## Changelog

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
