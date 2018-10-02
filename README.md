# Golin Timber-Webpack starter WordPress theme

A Timber theme with Webpack SCSS compilation, JS bundling, and Browsersync preview, plus some default templates and functions for an Advanced Custom Fields Flexible Content-based CMS config.

## Installation and usage

- Set up a WordPress install with the Timber plugin
- Clone this repo's contents into `wp-content/themes/[your-desired-theme-name]`
- Do two bulk find-and-replaces in the repo (in file names *and* contents) 
    + Replace `golin-redesign` with your lowercase theme name, using hyphens for spaces.
    + Replace `golin_redesign` the same way, using underscores for spaces.
- Rename `example.env.config.js` to `env.config.js` and change `PROXY_TARGET` to your local dev site's URL
- Create your new theme's git repo with `git init`
- `npm run start` to develop locally
- `npm run build` to generate the final theme

The actual, usable WordPress theme is the contents of the `build` folder. Upload it to your live site.

Be careful not to delete or overwrite the `acf-json` folder on the server; this folder should be manually downloaded to the root of your local repo whenever you change ACF configuration, but it should never exist in the `build` folder. The live version of this folder is canonical.
