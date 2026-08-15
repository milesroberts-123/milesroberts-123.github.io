# AGENTS.md

## Build & deploy

Source content lives in `docs/*.md`. Built HTML is committed to the repo root
for GitHub Pages. Never edit the root HTML files directly — they are generated.

```bash
mkdocs build          # generates site/ from docs/
cp -r site/* .        # copy output to repo root
rm -rf site/          # clean up (site/ is gitignored)
```

## Branch

The default branch is `master`, not `main`.

## Content

- `docs/*.md` — source Markdown pages
- `mkdocs.yml` — site config (theme: `simple-blog`, dark mode)
- `docs/stylesheets/extra.css` — custom CSS (also copied to `stylesheets/` at root)
- `docs/img/` — images

## Editing

Only edit files under `docs/`. Everything else at the repo root (except
`mkdocs.yml`, `.gitignore`, `README.md`) is built output from MkDocs.
