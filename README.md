# Thivanka Chiranjeeva — portfolio site (Minimal CV + Minima Projects)

This site merges two GitHub Pages themes into one repo:

- **`minimal` theme** → the homepage (`/`), used as a CV / personal
  details page.
- **`minima` theme** → the `/projects/` section. Each project is a normal
  Jekyll *post*, which `minima`'s home layout automatically lists — click
  "View My Projects →" on the homepage to get there.

They're kept side by side without conflicting:
- The homepage loads `assets/css/style.css` (Minimal's stylesheet).
- Everything under `/projects/` loads `assets/css/minima-style.css`
  (Minima's stylesheet, renamed so it doesn't overwrite Minimal's).
- Each theme's layouts, includes, and Sass partials are namespaced or
  distinctly named so nothing overwrites the other.

## What's already filled in

- `index.md` — full CV: summary, contact, skills, experience at Vega
  Innovations, education, certifications.
- `_posts/` — 10 projects pulled from the CV and project portfolio PDF,
  four of them (EV Charger Controller, RGB LED Controller, Equine Wearable
  Tracker, IoT Controller) with the real board photos/layouts extracted
  from the portfolio PDF, in `assets/img/projects/`.
- `_config.yml` — name, email, GitHub, and LinkedIn links.

## Still worth doing

- Add board photos for the other 6 projects (Power Input Protection,
  Thermal Protection Device, Network Controller Module, 24V SMPS, Real-Time
  Energy Monitoring, Medi Box) if you have them — drop them in
  `assets/img/projects/` and reference with an `<img>` tag like the
  existing posts.
- Push each project's actual repo to GitHub and link it from the matching
  post, the way a "View source" link works on a personal project.
- Double check the phone number and links in `index.md` before publishing,
  since a CV page is public.

## Run it locally (optional, needs Ruby + Bundler)

```bash
bundle install
bundle exec jekyll serve
```

Then open `http://localhost:4000`.

## Deploy to GitHub Pages

1. Create a repo named `tchiranjeeva.github.io` (for a user site — this
   exact name is required for a `https://tchiranjeeva.github.io` URL).
2. Push this whole folder to it:
   ```bash
   git init
   git add .
   git commit -m "Initial site"
   git branch -M main
   git remote add origin https://github.com/tchiranjeeva/tchiranjeeva.github.io.git
   git push -u origin main
   ```
3. On GitHub: **Settings → Pages → Source → Deploy from a branch**,
   branch `main`, folder `/ (root)`. Save, then wait a minute for it to
   build — GitHub Pages runs Jekyll automatically, no build step needed
   from you.

## Adding a new project later

Add a new file to `_posts/`, named `YYYY-MM-DD-project-slug.md`, with:

```markdown
---
layout: post
title: "Project Name"
date: 2026-09-01
---

Short intro paragraph (shown as the excerpt on the projects list).

<!--more-->

Full write-up here.
```

It'll automatically appear at the top of `/projects/` — no other file
needs editing.
