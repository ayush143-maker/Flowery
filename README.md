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

## Deployment-readiness checklist

This repository contains a static HTML page and documents no build or deployment configuration. Before publishing:

- [ ] Use the repository root as the page's document root; it contains the top-level `index.html`.
- [ ] Include `index.html` and any assets added for the page in the published files. No separate asset directory is listed at the repository root.
- [ ] Check every asset reference in `index.html` against the asset's actual location. Prefer paths that remain valid from the page's location, and update references if files move.
- [ ] No environment-variable template is listed, so no environment configuration is indicated by this repository.
- [ ] After publishing, open the resulting page in a browser. Review the invitation, sunflower, and bloom animation at narrow phone-sized and wide desktop-sized viewports, checking for clipping or overflow.
- [ ] If an interaction or asset was added, verify it in that final browser preview. These are recommended checks, not claims that publishing or testing has already occurred.

## Contributor handoff

Keep changes scoped to the relevant content or styling in `index.html`. Preserve the filename and any existing relative references unless a change requires updating them; if you add or move an asset, update its page reference too. In the handoff, briefly describe what changed and identify the affected file or page area.

Before publishing, manually open the page and review the invitation, sunflower, and bloom animation. Check a narrow phone-sized viewport and a wide desktop-sized viewport for clipping or overflow. If you add an interaction, try it in the browser. This is a review checklist, not a report of completed testing or verified results.

## Final release review

- Open `index.html` from the published location and confirm the page loads as expected.
- Review the published result once on a narrow screen and once on a wider screen; treat this as a release check, not an automated test report.
