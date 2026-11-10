# ubuntu-id.github.io

Website of the Ubuntu Indonesia Community, live at https://ubuntu-id.org. Hugo with the `themes/ubuntukr` theme (Vanilla Framework, derived from the ubuntu-kr site). Default branch `main`. Remote: `ubuntu-id/ubuntu-id.github.io`.

## Stack

- Hugo extended **0.147.9** and Dart Sass **1.89.2**, pinned in `.github/workflows/hugo.yml`. Use the same versions locally.
- The theme uses `css.Sass` (not `resources.ToCSS`, removed in Hugo 0.128) with the `dartsass` transpiler, so the `sass` binary must be on `PATH`. The npm `sass` package does not work with Hugo.
- Theme dependency: `vanilla-framework` 3.4.0 through `themes/ubuntukr/package-lock.json`. Run `npm ci` in `themes/ubuntukr` before building.
- Two languages: Indonesian (default, at `/`) and English (at `/en/`). Every page has an `index.md` and an `index.en.md`.

## Build and test

```bash
cd themes/ubuntukr && npm ci && cd ../..
hugo --minify -d /tmp/out     # must finish without ERROR
```

About 590 Dart Sass deprecation warnings from `vanilla-framework` are normal. Check the built output, not just the exit code:

- every local `<img src>` points to a file that exists in the output (including under `/en/`);
- `404.html` and `en/404.html` are built;
- no link to a dead host (see below).

For UI checks, serve the output and drive it with Playwright at 1280 px and 390 px. Build with `--baseURL http://127.0.0.1:<port>/`, because the stylesheet link uses the absolute `Permalink` and would otherwise load the production CSS. Wait about 1.3 s after load: the hero columns fade in over 1 s and look faded in earlier screenshots. Let the page load the Ubuntu font from `assets.ubuntu.com`, otherwise widths differ from production.

CI (`hugo.yml`): a push to `main` builds and deploys to the `gh-pages` branch with `peaceiris/actions-gh-pages`; a pull request only builds (the check is named `deploy`). Downloading Hugo from github.com sometimes fails (`wget` exit 4): rerun the job.

## Conventions

- Change a page in both languages. `*.en.md` files must be English, not leftover Korean from the ubuntu-kr template.
- Page images are referenced by `image:` and `backgroundImage:` in the front matter and fetched with `.Resources.Get` in templates. Do not build URLs with `{{ .RelPermalink }}{{ .Params.image }}` or put the raw front matter value in CSS: that breaks under `/en/` and for pages without an image.
- Inside `{{ with }}` the dot changes. Store values you still need (for example `{{ $title := .Title }}`) before the `with`.
- `hugo --minify` removes the whitespace between sibling inline elements, so inline lists cannot wrap. Use flex with `flex-wrap` (see the footer list in `theme.scss`).
- Page title, description, canonical URL, `hreflang` and Open Graph tags come from `themes/ubuntukr/layouts/partials/head.html`. The 404 page is deliberately `noindex`.
- ISO mirror links on the download page are only for mirrors whose ISO path is verified to exist and to hold the latest releases. "Up to date" on Launchpad rates the package archive, not the ISOs, so open the directory.
- The Ubuntu versions on the download page (`ubuntuVersions` in the front matter of `content/download/`) need updating every April and October. Release notes live at `documentation.ubuntu.com/release-notes/<version>/`.

## Dependencies

- Dependabot (`.github/dependabot.yml`) opens at most one grouped pull request per ecosystem each week: one for GitHub Actions and one for the theme's npm packages. Merge that single PR instead of many.
- Do not upgrade `vanilla-framework` beyond 3.4.x yet. From 3.15 it loads a variable Ubuntu font from `assets.ubuntu.com` whose `Content-Disposition` header has an unquoted filename containing a comma. Chromium rejects it (`ERR_RESPONSE_HEADERS_MULTIPLE_CONTENT_DISPOSITION`), so Chrome and Edge fall back to a wider system font: pages get taller and about 42 px wider on phones. Dependabot is told to skip minor and major Vanilla updates. Test in Chromium before lifting that.
- `package-lock.json` cannot be merged by hand when several Dependabot branches touch it. Merge one grouped update, or apply per-package changes and let `npm ci` in CI validate.

## Links that must not be used again

`forum.ubuntu-id.org`, `events.ubuntu-id.org` and `event.ubuntu-id.org` (no DNS), the YouTube channel `user/ubuntuindonesia`, `ubuntulinux.or.id`, and anything under `ubuntu-kr`. Replacements in use: the forum goes to the Ubuntu Indonesia Discourse category (`discourse.ubuntu.com/c/community/circles/ubuntu-id/133`), events go to `events.canonical.com`.

## Repository settings

`main` is protected: changes need a pull request and a passing `deploy` check, and force pushes and deletion are blocked (admins can override). Dependabot alerts, security updates, secret scanning and push protection are on. Branches are deleted automatically after merge.

## Open questions

- `gimpscape.org` (sponsors page) fails TLS: it is not confirmed whether the sponsor is still active.
- `content/bylaws/akta.pdf` (21.9 MB) is deliberately left in the repo.
- The Indico feed at `events.canonical.com` has no Ubuntu Indonesia category yet, so an event list cannot be pulled at build time.
- The stylesheet link uses the absolute `Permalink`, so local and staging builds load the production CSS. Switching to `RelPermalink` would fix it.
