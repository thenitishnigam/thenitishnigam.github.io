# thenitishnigam.github.io

Source for Nitish Nigam's academic website, built with [Quarto](https://quarto.org) and published to GitHub Pages at <https://thenitishnigam.github.io>.

Every push to `master` rebuilds and publishes the site automatically (about two minutes). You can edit everything directly on github.com; you don't need R or Quarto installed.

## Where things live

| To change | Edit |
|---|---|
| Home page bio, research themes, links | `index.qmd` |
| Papers, working papers, cases, chapters | `data/publications.yml` |
| Talks | `data/talks.yml` |
| Policy and consulting | `policy.qmd` |
| Teaching and training | `teaching.qmd` |
| CV | `cv.qmd` |
| Profile photo | add `images/profile.jpg`, then change `images/profile.svg` to `images/profile.jpg` in `index.qmd` |
| Menu, footer, site title | `_quarto.yml` |
| Colours and fonts | `styles/light.scss`, `styles/dark.scss`, `styles/rules.scss` |

## Common tasks

**Add a paper.** Open `data/publications.yml`, copy an existing entry and edit it. `type` decides which section it appears in (`article`, `working`, `case`, `chapter`, `magazine`). Add `featured: true` and a `home-order` number to show it on the home page. To attach a PDF, upload it to `files/papers/` and add `pdf: files/papers/name.pdf`.

**Add a talk.** Copy an entry in `data/talks.yml`. `sortdate` controls the order; `when` is what's shown.

**Write a post.** Copy `writing/_example-post/` to a new folder such as `writing/2026-ev-subsidies/` (no leading underscore) and edit `index.qmd`.

**Add a trip.** Copy `travel/_example-trip/` to a new folder such as `travel/2026-sikkim/`, add photos (about 2000 px on the long side; strip location data), and edit `index.qmd`.

## Preview on your computer (optional)

With Quarto installed, run `quarto preview` in this folder.

## One-time GitHub setup

Repository **Settings → Pages → Build and deployment → Source: GitHub Actions**.
