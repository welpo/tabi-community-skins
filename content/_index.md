+++
title = "tabi community skins"
description = "Browse and discover community-contributed skins for the tabi Zola theme."

[extra]
copy_button = true
+++

Welcome to the tabi community skins showcase. Here you'll find custom color schemes and styling variations contributed by the tabi community.

## How to use a skin

1. **Download:** Click the download button next to the skin you like
2. **Place:** Add the downloaded file to your site, in one of these locations:
   - `sass/skins/`
   - `themes/tabi/sass/skins/`
3. **Enable:** Set `skin = "skin-name"` in `config.toml` (without the file extension)

**Note:** You may need to create the `sass/skins/` directory first.

---

{{ display_all_skins() }}

---

## Contributing

Want to share your own tabi skin? We'd love to have your contribution!

To contribute a skin:

1. **Fork** the [tabi-community-skins repository](https://github.com/welpo/tabi-community-skins)
2. **Create a folder** in `static/skins/` with your skin name (e.g. `my-awesome-skin/`)
3. **Add your files**:
   - `skin.scss`: The SCSS code for your skin. Recommended: use tabi's mixin format (see [tabi's docs](https://welpo.github.io/tabi/blog/customise-tabi/#create-your-own-skin))
   - **Screenshots**:
     - If your skin supports both light and dark themes: `screenshot-light.webp` and `screenshot-dark.webp` (also supports `png` and `jpg`)
     - If your skin supports only one theme: `screenshot.webp` (also supports `png` and `jpg`)
   - Optional: `about.md` for attribution, accessibility concerns, description, or any additional information (rendered as markdown)
4. **Add your skin folder name** to the `skin_folders` list in `templates/shortcodes/display_all_skins.html`
5. **Submit a pull request**
