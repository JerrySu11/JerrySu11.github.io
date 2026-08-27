# JerrySu11.github.io

Personal academic/professional website for Zihao Su — live at
<https://jerrysu11.github.io>.

Plain static HTML and CSS. No build step, no dependencies: GitHub Pages serves
this repository's `main` branch as-is, so a push is a deploy.

## Layout

| Path | Purpose |
|------|---------|
| `index.html` | Landing page — positioning, research threads, selected papers, news |
| `research.html` | The research narrative in prose |
| `publications.html` | Full publication list with metrics |
| `cv.html` | Web CV |
| `assets/css/style.css` | The entire stylesheet |
| `assets/img/` | Favicon, and a headshot if one is added |
| `assets/files/` | Downloadable PDFs (CV) — currently empty |
| `.nojekyll` | Tells Pages to serve files as-is |

Site chrome (header nav, footer) is duplicated in each page. With four pages
that is cheaper than adding a build step — when editing the nav, change all
four.

## Local preview

```sh
python3 -m http.server 8000   # then open http://localhost:8000
```

## Content source of truth

Facts here are mirrored from the private `career_planning` repo, of which this
repo is a submodule (`website/`). When publications, awards, or grants change,
update `career_planning/profile/` first, then reflect the change here.

## Things marked for later

- No headshot yet (`assets/img/`).
- No downloadable CV PDF yet — the existing resume PDF carries a phone number;
  add a scrubbed copy to `assets/files/` and uncomment the link in `cv.html`.
- Papers under double-blind review are listed without full titles on purpose;
  see the comment in `publications.html`.
