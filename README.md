# portfolio

Personal site for Ahlam Tarik — AI engineer & researcher.
Live at **https://theahlamtarik.github.io/portfolio/**

Single static page, no build step, no dependencies. Everything lives in `index.html`.

## Deploy

Already wired to `origin`. To publish an update:

```bash
git add -A && git commit -m "Update" && git push
```

GitHub Pages is served from **`main` / `/ (root)`** — set under **Settings → Pages**.
A push goes live in about a minute.

> Renaming the repo to `theahlamtarik.github.io` would move the site to the bare
> `https://theahlamtarik.github.io` with no `/portfolio/` subpath. Nothing in the page uses
> absolute paths, so it works either way with no code changes.

## Editing

- All content is plain HTML inside `index.html` — edit the text directly.
- Colors are CSS variables at the top (`--bg`, `--ink`, `--accent`, …), with a dark-mode block
  right below that follows the visitor's system theme.
- `cv.pdf` is the file linked from the header — replace it to update the CV.
- The hero animation is the small script at the bottom: an ECG trace over an audio envelope.
  Delete the `<canvas>` and the `<script>` to remove it. It's disabled automatically for
  visitors with reduced-motion enabled.
