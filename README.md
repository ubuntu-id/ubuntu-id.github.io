## Ubuntu Indonesia Community

Website of the Ubuntu Indonesia Community, live at <https://ubuntu-id.org>. Built with [Hugo](https://gohugo.io) and a [Vanilla Framework](https://vanillaframework.io) theme (`themes/ubuntukr`) derived from the [ubuntu-kr](https://ubuntu-kr.org) site.

## Build locally

You need:

- Hugo **extended** 0.147.9 (the version CI uses)
- Dart Sass 1.89.2 on your `PATH` as `sass` (Hugo calls it to build the theme CSS)
- Node.js and npm, to install the theme's dependencies

```bash
cd themes/ubuntukr && npm ci && cd ../..
hugo server        # live preview at http://localhost:1313
hugo --minify      # production build into public/
```

The build prints many Dart Sass deprecation warnings from `vanilla-framework` 3.4.0. They are harmless for now.

## Content

The site has two languages: Indonesian (default, served at `/`) and English (served at `/en/`). Each page is a folder under `content/` with two files:

- `index.md`: Indonesian
- `index.en.md`: English

Keep both in sync when you edit a page. Images referenced by the `image` front matter key live in the same folder as the page.

## Deploy

Pushing to `main` runs `.github/workflows/hugo.yml`, which builds the site and publishes it to the `gh-pages` branch (GitHub Pages, custom domain `ubuntu-id.org`). Pull requests run the same build without deploying. `main` is protected: changes go through a pull request with the `deploy` check passing.

## Credits and license

The theme comes from the ubuntu-kr community site, which is MIT licensed. Please keep this credit. Website source code is MIT licensed (see `LICENSE`). Content is licensed under CC BY-SA 4.0. Ubuntu and Canonical are registered trademarks of Canonical Ltd.
