# ATHIC 2026 presentation

This folder is a self-contained static presentation site. `index.html` is the
ready-to-publish presentation; `jg_ATHIC2026.md` and `heading-case.css` are the
editable source files. Images and the animation video are included beside the
HTML, and Reveal.js is included under `libs/`.

## Preview

Open `index.html` in a browser. For local preview over HTTP, run from this
folder:

```sh
python3 -m http.server 8000
```

Then open `http://localhost:8000`.

## Publish with GitHub Pages

Create an empty repository on GitHub (do not add a README, license, or
`.gitignore` there). On the cluster, change into this folder and run:

```sh
git init -b main
git add .
git commit -m "Publish ATHIC 2026 presentation"
git remote add origin https://github.com/USERNAME/REPOSITORY.git
git push -u origin main
```

Replace `USERNAME` and `REPOSITORY` with the GitHub account and repository
name. If this folder is already a Git repository, skip `git init -b main`.
If `origin` is already configured, skip `git remote add origin ...`.

On GitHub, open **Repository → Settings → Pages**. Under **Build and deployment**,
choose **Deploy from a branch**, select branch `main` and folder `/ (root)`, then
save. The published site URL will be shown on that Pages settings screen. Keep
`index.html` at the repository root for it to load as the home page.

If you publish through a different Git hosting service, push this same folder
to its repository and enable that service's static-site hosting for the root
directory.

## Updating the presentation

The Markdown is the editable source; `index.html` is the published slide deck.
After editing the Markdown, regenerate `index.html` with the presentation build
toolchain before committing so the published slides reflect the edits. Keep the
relative media filenames and `libs/` directory in place.
