# Personal website

A dependency-free static academic site for Fall 2027 CS PhD applications.

## Preview locally

From this directory:

```bash
python3 -m http.server 8000
```

Open <http://localhost:8000>. The site includes a copy of `academic_cv.pdf` so its CV link works from this directory. After updating the parent CV, replace this copy before publishing.

## Update content

1. Update factual information in `../source_of_truth.md` first.
2. Update CV, publication statuses, and this site together.
3. Test on a narrow browser width before publishing.

## Deploy

### GitHub Pages

Push this directory’s contents (not the parent directory) to the branch or repository configured for Pages. In the repository settings, set Pages to deploy from that branch/root. The site requires no build step.

### Vercel

Import the repository, set the root directory to `phd_application_materials/personal_website`, and deploy as a static site. No build command is necessary.

Review factual accuracy, links, and publication statuses before publishing.
