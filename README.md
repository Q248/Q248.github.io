# Qi Yin — personal website

Built with [al-folio](https://github.com/alshedivat/al-folio) (Jekyll). Published at **https://q248.github.io**.

## One-time setup on GitHub

1. Rename this repository to **`Q248.github.io`** (Settings → General → Repository name).
   GitHub serves a repo with that exact name at the root address `https://q248.github.io`.
2. Settings → Actions → General → Workflow permissions → choose **Read and write permissions** → Save.
3. Push this code to `main`. The **Deploy site** action builds the site (~5 min) and creates a `gh-pages` branch.
4. Settings → Pages → Source: **Deploy from a branch** → Branch: **gh-pages** / **(root)** → Save.

## Where to edit

| What | File |
| --- | --- |
| Bio, photo, address | `_pages/about.md`, `assets/img/prof_pic.jpg` |
| Publications | `_bibliography/papers.bib` (add `selected = {true}` to show on the home page) |
| CV | `_data/cv.yml`; for a PDF button, add `assets/pdf/Qi_Yin_CV.pdf` and uncomment `cv_pdf` in `_pages/cv.md` |
| Projects | `_projects/*.md` |
| News (short items on home page) | `_news/*.md` |
| Blog posts | `_posts/YYYY-MM-DD-title.md` |
| Email, ORCID, Scholar, etc. | `_data/socials.yml` |
| Site name, URL, settings | `_config.yml` |

Every push to `main` rebuilds the site automatically.
