# ctran.github.io

Personal site of Cuong Tran, live at https://ctran.github.io.

Jekyll site using the [Minimal Mistakes](https://github.com/mmistakes/minimal-mistakes) theme (via `remote_theme`), published by GitHub Pages from `main`. Content is in `index.md`; settings are in `_config.yml`.

## Preview locally

Pushing to `main` publishes the site, so preview first. With Docker running:

```bash
mise run preview
```

Wait for `Server running...` (the first run takes a minute), then open http://localhost:4000. See the `preview` task in `mise.toml` for details.

Without Docker, `jekyll serve` works if Ruby, Jekyll, and the `jekyll-remote-theme` and `jekyll-include-cache` gems are installed.
