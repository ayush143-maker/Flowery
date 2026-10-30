# Flowery

Flowery is a small animated, sunflower-themed static page built around the invitation “Have a flower.” The top-level `index.html` presents a dark backdrop and a central blooming flower.

## Preview locally

No package installation is needed. Open `index.html` in a browser, or serve the repository directory:

```sh
python -m http.server 8000
```

Then visit [http://localhost:8000](http://localhost:8000). No deployment configuration or build step is documented.

## Editing the page

The invitation text, styles, and bloom are in `index.html`. Locate the existing content and styling before editing. The repository root lists only `index.html` and this README, with no separate asset directory. If you add an image or another asset, choose its location deliberately and make the reference in `index.html` match its actual path.

For a static publication, serve the repository root so the top-level `index.html` is the page entry point. Include any assets added to the page and verify that their paths resolve from the published page. No environment-variable template or environment configuration is indicated by the listed files.

## Repository map

- `index.html` — page entry point, invitation, styling, and bloom.

After making changes, preview the page in a browser at narrow and wide viewport sizes. Check the invitation, flower, and animation for clipping or overflow; try any interaction added to the page. These are review suggestions, not reports of completed checks.