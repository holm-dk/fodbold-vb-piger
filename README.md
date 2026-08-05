# VB U14 Piger

Jekyll site with practical info for players and parents of VB U14 Piger
(Vejgaard Boldspilklub), served via GitHub Pages at
<https://vb2014p.barnbaek.dk>.

## Structure

- `index.md` — all page content
- `_layouts/default.html` — page layout (header, nav, footer, favicon)
- `_includes/` — card components used by `index.md`
- `assets/css/style.css` — the design (plain CSS, no theme gem)
- `_config.yml` — site title/description
- `CNAME` — custom domain (managed by GitHub Pages, don't remove)

Never edit anything under `_site/` — it's generated build output and gets
overwritten on every build.

## Serve locally

Requires the Ruby version in [`.ruby-version`](.ruby-version) (managed with rbenv):

```sh
rbenv install        # installs the version from .ruby-version, if missing
gem install jekyll
```

Then start the dev server from the repo root:

```sh
jekyll serve --livereload
```

The site is available at <http://127.0.0.1:4000> and rebuilds automatically
when files change — except `_config.yml`, which requires a server restart.

## Deploy

Push to `main` — GitHub Pages builds and publishes the site automatically.
The stylesheet URL is versioned with the build timestamp, so CSS changes
reach visitors without cache issues.
