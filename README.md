# Fodbold VB Piger

Simple Jekyll site served via GitHub Pages at
<https://holm-dk.github.io/fodbold-vb-piger/>.

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
when files change.

## Deploy

Push to `main` — GitHub Pages builds and publishes the site automatically.
