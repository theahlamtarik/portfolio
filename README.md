# theahlamtarik.github.io

Personal site for Ahlam Tarik — AI engineer & researcher.

Single static page, no build step, no dependencies. Everything lives in `index.html`.

## Deploy to GitHub Pages

1. Create a repo named **`theahlamtarik.github.io`** on GitHub (that exact name gives you
   `https://theahlamtarik.github.io` with no subpath).
2. From this folder:

```bash
git init && git add . && git commit -m "portfolio" && git branch -M main && git remote add origin https://github.com/theahlamtarik/theahlamtarik.github.io.git && git push -u origin main
```

3. On GitHub: **Settings → Pages → Source: Deploy from a branch → `main` / `root`**. Live in ~1 minute.

> Using a differently-named repo instead (e.g. `portfolio`) works too — the URL just becomes
> `https://theahlamtarik.github.io/portfolio/`. Nothing in the page uses absolute paths, so it works either way.

## Editing

- All content is plain HTML inside `index.html` — edit the text directly.
- Colors are CSS variables at the top (`--bg`, `--ink`, `--accent`, …), with a dark-mode block
  right below that follows the visitor's system theme.
- `cv.pdf` is the file linked from the header — replace it to update the CV.
- The hero animation is the small script at the bottom: an ECG trace over an audio envelope.
  Delete the `<canvas>` and the `<script>` to remove it. It's disabled automatically for
  visitors with reduced-motion enabled.
