# tabi Community Skins

Community-contributed skins for the [tabi](https://github.com/welpo/tabi) Zola theme.

## Contributing

We welcome contributions from the community! Here's how to add your skin:

### Requirements

Each skin must include:

1. **Folder**: Create a folder in `skins/` with your skin name (use lowercase and hyphens)
2. **Screenshot**: `screenshot.webp` - Preview image. If it supports light and dark modes, please add `screenshot-light.webp` and `screenshot-dark.webp`. `jpg` and `png` images are also supported
3. **CSS**: `skin.scss` - The SCSS code using tabi's skin format. See [tabi docs](https://welpo.github.io/tabi/blog/customise-tabi/#create-your-own-skin)
4. **About** (optional): `about.md` - Markdown file for attribution, description, accessibility concerns…

### Folder structure

```
skins/
└── my-awesome-skin/
    ├── screenshot.webp    # Required: Preview image
    ├── skin.scss          # Required: CSS code
    └── about.md           # Optional: Author attribution
```

### Contribution Process

1. **Fork** this repository
2. **Create a folder** in `static/skins/` with your skin name (e.g. `my-awesome-skin/`)
3. **Add your files**:
   - `skin.scss`: The SCSS code for your skin. Recommended: use tabi's mixin format (see [tabi's docs](https://welpo.github.io/tabi/blog/customise-tabi/#create-your-own-skin))
   - **Screenshots**:
     - If your skin supports both light and dark themes: `screenshot-light.webp` and `screenshot-dark.webp` (also supports `png` and `jpg`)
     - If your skin supports only one theme: `screenshot.webp` (also supports `png` and `jpg`)
   - Optional: `about.md` for attribution, accessibility concerns, description, or any additional information (rendered as markdown)
4. **Add your skin folder name** to the `skin_folders` list in `templates/shortcodes/display_all_skins.html`
5. **Submit a pull request**

## License

The code is available under the [MIT license](./LICENSE). By contributing a skin, you agree to license your code under the MIT license.
