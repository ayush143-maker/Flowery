# Flowery

A small animated sunflower-themed static page built around the invitation “Have a flower.” The top-level `index.html` presents a dark backdrop and a central blooming flower.

## Preview locally

No package installation is needed. Open `index.html` in a browser, or serve the repository directory:

```sh
python -m http.server 8000
```

Then visit http://localhost:8000. After editing, review the layout at desktop and mobile viewport sizes. No deployment configuration is documented.

## Personalizing the page

The root files list only `index.html` and this README, so begin by locating the existing invitation text and the styles for the dark backdrop and sunflower in `index.html`. Change the wording or colors there, and preview the result at desktop and mobile sizes. If you introduce an external image or another asset, add it deliberately and update its reference in `index.html` to match its actual path; no separate asset directory is listed at the repository root.