# ctran.github.io

Personal site of Cuong Tran, live at https://ctran.github.io.

It is a Jekyll site using the [Minimal Mistakes](https://github.com/mmistakes/minimal-mistakes) theme (via `remote_theme`), built and served by GitHub Pages from the `main` branch. Content is in `index.md` and settings are in `_config.yml`.

## Preview locally

Pushing to `main` publishes the site, so review changes locally first.

### With Docker

No Ruby install needed. Start Docker, then run from the repo root:

```bash
mise run preview
```

This runs the `preview` task defined in `mise.toml`, which is equivalent to:

```bash
docker run --rm --name jekyll-preview -p 4000:4000 -v "$PWD":/srv/jekyll jekyll/jekyll \
  sh -c "gem install jekyll-remote-theme jekyll-include-cache --no-document && \
         jekyll serve --host 0.0.0.0 --destination /tmp/_site"
```

Wait for `Server running...` (the first run installs gems and fetches the theme from GitHub, so it takes a minute), then open http://localhost:4000. The site rebuilds when files change. Stop it with `Ctrl-C`, or `docker rm -f jekyll-preview` if it runs detached (`-d`).

`--host 0.0.0.0` is required, otherwise the server is unreachable from outside the container. `--destination /tmp/_site` keeps build output out of the repo.

### With Ruby and Jekyll

If Ruby and Jekyll are installed (the `jekyll-remote-theme` and `jekyll-include-cache` gems are also required):

```bash
jekyll serve
```

Then open http://localhost:4000.
