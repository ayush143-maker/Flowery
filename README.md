# Flowery

A small animated sunflower-themed static page built around the invitation “Have a flower.” The top-level `index.html` presents a dark backdrop and a central blooming flower. The repository root lists only `index.html` and this README.

## Preview locally

No package installation is needed. Open `index.html` in a browser, or serve the repository directory:

```sh
python -m http.server 8000
```

Then visit http://localhost:8000. No deployment configuration is documented.

## Editing the page

The invitation text, styles, and bloom are in `index.html`. Locate the existing content and styling before changing them. No separate asset directory is listed at the repository root. If you add an image or another asset, place it deliberately and make the reference in `index.html` match its actual path.

## Contributor handoff

Keep changes scoped to the relevant content or styling in `index.html`. Preserve the filename and any existing relative references unless a change requires updating them; if you add or move an asset, update its page reference too. In the handoff, briefly describe what changed and identify the affected file or page area.

Before publishing, manually open the page and review the invitation, sunflower, and bloom animation. Check a narrow phone-sized viewport and a wide desktop-sized viewport for clipping or overflow. If you add an interaction, try it in the browser. This is a review checklist, not a report of completed testing or verified results.
