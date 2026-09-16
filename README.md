# Personal academic website

A dependency-free static site for Fall 2027 CS PhD applications. This directory is deployed as the GitHub Pages site root.

## Preview locally

From this directory:

```bash
python3 -m http.server 8000
```

Open <http://localhost:8000>. The site includes a copy of `academic_cv.pdf` so its CV link works from this directory. After updating the parent CV, replace this copy before publishing.

## Layout

- `index.html`, `styles.css` — the whole site; no build step.
- `academic_cv.pdf` — copy of `../academic_cv.pdf`; replace it whenever the CV is rebuilt, and bump the `?v=` query in every CV link.
- `papers/` — local manuscript copies for review only; this directory is ignored and must not be published without explicit author approval.
- `assets/research/` — figures used by the page. `lpbts-decision.svg` is generated; the illustration JPEGs are 1400 px exports. Full-resolution sources live in `../assets_source/research/` and are deliberately not deployed.

## Update content

1. Update factual information in `../source_of_truth.md` first.
2. Update CV, publication statuses, and this site together.
3. Keep every image under ~250 KB and give each `<img>` its `width`/`height`.
4. Test on a narrow browser width before publishing.
5. Do not add `papers/` to the deployed repository unless the author explicitly approves each file and target venue policy has been checked.

## Deploy

### GitHub Pages

Push this directory’s contents to the branch or repository configured for Pages. The site requires no build step. Review factual accuracy, links, publication status, and manuscript-release scope before publishing.
