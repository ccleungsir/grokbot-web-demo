# grokbot-web-demo

Grok Bot 喺 2026 年 9 月即場建立嘅公開單頁示範網站。

This repository hosts a small static welcome page. It exists to prove that the assistant can write a webpage, publish it to GitHub, and provide a working public URL.

## Public site

- Official GitHub Pages: https://ccleungsir.github.io/grokbot-web-demo/
- Repository: https://github.com/ccleungsir/grokbot-web-demo
- Public HTML preview (served from `main`): https://raw.githack.com/ccleungsir/grokbot-web-demo/main/index.html

The page is Traditional Chinese first, with supporting English. There is no build step: open `index.html`, or let GitHub Pages serve the files from `main`.

## Enable GitHub Pages

GitHub App / Actions tokens cannot create a Pages site for the first time. The owner needs one click:

1. Open [Settings → Pages](https://github.com/ccleungsir/grokbot-web-demo/settings/pages)
2. Choose either:
   - **GitHub Actions**, then re-run the **Deploy GitHub Pages** workflow
   - or **Deploy from a branch**: branch `main`, folder `/` (root)

The site URL stays https://ccleungsir.github.io/grokbot-web-demo/

## What is in the repo

- `index.html` — single-page welcome
- `styles.css` — responsive layout and visual design
- `script.js` — light interaction for in-page links
- `.github/workflows/deploy-pages.yml` — GitHub Actions deploy to Pages

## Local preview

```bash
python3 -m http.server 8080
```

Then open http://127.0.0.1:8080
