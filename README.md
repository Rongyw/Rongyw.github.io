# Rong (Rosina) Yuwen — academic website

Source for <https://rongyw.github.io>, built with the [al-folio](https://github.com/alshedivat/al-folio) Jekyll starter (MIT license) and deployed by GitHub Actions to the `gh-pages` branch.

## Where things live

| What | File |
|---|---|
| Name, site URL, site-wide settings | `_config.yml` |
| Home page (bio, job market paper, "Outside research" photo) | `_pages/about.md` |
| Address under the photo | `profile.more_info` in `_pages/about.md` |
| Sidebar icons (row 1: CV, email, LinkedIn; row 2: Scholar, SSRN, GitHub) | `_data/socials.yml` |
| Research page: papers, coauthors, abstracts, links | `_bibliography/papers.bib` |
| Research page sections | `category` field in each `.bib` entry: `publication`, `working`, `progress` |
| Teaching page | `_pages/teaching.md` |
| CV PDF | Not posted yet. Add it as `assets/pdf/CV_Rong_Yuwen.pdf`, then follow the comment in `_pages/cv.md` |
| Photos | `assets/img/profile.jpg`; "Outside research" photos `assets/img/garden.jpg`, `assets/img/photo_*.jpg` (resized to 1600 px on the long side) |
| Layout and style tweaks | `_layouts/about.liquid`, `_sass/_custom.scss` (keep `assets/_sass/_custom.scss` identical) |

## Updating

Edit the files above and push to `main`. The "Deploy site" workflow rebuilds the site in a few minutes.
