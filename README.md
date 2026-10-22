# Gideon Portfolio Site — Publish Guide

This folder contains a static portfolio website and an Early Access source preview ZIP. It is designed for GitHub Pages and does not require a server or a build step.

## Preview it locally

Double-click `index.html` to preview the site in your browser. The screenshot and download link use relative paths, so keep `assets/` and `downloads/` alongside `index.html`.

## Publish with GitHub Pages

1. Sign in to GitHub and create a new repository named `gideon-portfolio` (or another name you like).
2. Extract this site ZIP. Upload `index.html`, `assets/`, `downloads/`, and this `README.md` to the repository's root. Do **not** upload your working app's `.venv`, private database, or personal conversation records.
3. In the repository, open **Settings → Pages**.
4. Under the build/deployment source, choose **Deploy from a branch**, then select branch `main` and folder `/ (root)`. Save.
5. Wait for the Pages deployment to finish. GitHub will show the published URL in **Settings → Pages**. A project site URL usually follows `https://YOUR-USERNAME.github.io/gideon-portfolio/`.

Official instructions: https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site

## What visitors can download

The website button downloads `downloads/Gideon-Early-Access-Source.zip`. That is a source/setup preview, **not** the eventual one-click Windows installer. It requires Windows, Python 3.14, Ollama, and a separate `qwen2.5:7b` model download. The website says this before download so visitors are not misled.

When a tested Windows installer exists, upload it as a release asset (GitHub Releases is designed for distributing release files) and update the button + instructions accordingly: https://docs.github.com/en/repositories/releasing-projects-on-github/about-releases

## Edit the site

- Update the title, introduction, feature descriptions, and project links in `index.html`.
- Replace `assets/gideon-app-preview.png` with a newer screenshot if the UI changes.
- Change the download filename/link in `index.html` if the source package name changes.
- Update version/readiness language when the actual installable release is ready.

## Public publishing reminder

GitHub Pages sites are public. Inspect all files before uploading. Never publish database files, personal conversations, `.venv`, credentials, environment files, API keys, or private local paths. The source package deliberately does not include your personal database.
