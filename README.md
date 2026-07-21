# spenbert02.github.io

Personal website — built with Jekyll on the [Academic Pages](https://academicpages.github.io/) theme (a fork of [Minimal Mistakes](https://mmistakes.github.io/minimal-mistakes/), © 2016 Michael Rose, MIT License; see `LICENSE`).

## Running locally

```
bundle install
bundle exec jekyll serve -l -H localhost
```

Then visit `http://localhost:4000/`.

## Structure

- `_pages/` — standalone pages (about, projects, papers, tutoring)
- `_portfolio/`, `_publications/`, `_talks/`, `_patents/` — content collections
- `_data/navigation.yml` — main nav links
- `images/` — site images
- `_sass/`, `_layouts/`, `_includes/`, `assets/` — theme files
