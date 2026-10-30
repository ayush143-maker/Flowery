# Flowery

A small animated sunflower-themed static page built around the invitation “Have a flower.” The top-level `index.html` presents a dark backdrop and a central blooming flower.

## Preview locally

No package installation is needed. Open `index.html` in a browser, or serve the repository directory:

```sh
python -m http.server 8000
```

Then visit http://localhost:8000. No deployment configuration is documented.

## Personalizing the page

The root files list only `index.html` and this README, so begin by locating the existing invitation text and the styles for the dark backdrop and sunflower in `index.html`. Change the wording or colors there. If you introduce an external image or another asset, add it deliberately and update its reference in `index.html` to match its actual path; no separate asset directory is listed at the repository root.

## Manual review checklist

Use these actions to review a change; they are not verified results.

- Open the known entry page, `index.html`, in a browser, or open `http://localhost:8000` after starting the local server above.
- Check the invitation text, dark backdrop, and sunflower at both a narrow phone-sized viewport and a wide desktop-sized viewport.
- Observe the existing bloom animation. If your change introduces an interaction, try it in the browser.
- Check any referenced image or media paths after adding or changing assets, and confirm that the page points to their actual locations.
