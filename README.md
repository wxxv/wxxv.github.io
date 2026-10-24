# Wenxin Xu's Academic Homepage

Source for [wxxv.github.io](https://wxxv.github.io). The page is a static research dashboard adapted from [Chengsong Huang's homepage](https://github.com/Chengsong-Huang/Chengsong-Huang.github.io).

Edit `index.html` to update the bio, news, papers, experience, and awards. Portrait and CV live in `assets/`.

## Local preview

```bash
python -m http.server 8000
```

Then open http://localhost:8000/.

## Publishing

GitHub Pages serves the `gh-pages` branch. Pushing to `main` runs `.github/workflows/deploy.yml`, which publishes `index.html`, the portrait, and the CV.

`scripts/update_citations.py` refreshes the Google Scholar citation count, h-index, and per-paper counts. A daily workflow commits any change and republishes the site. Optional: add a `SERPAPI_KEY` repository secret if Google Scholar blocks the free fetch.
