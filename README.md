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

Use these actions to review a change. This is a checklist, not a report of completed checks or measured performance.

- Open `index.html` in a browser, or visit `http://localhost:8000` after starting the local server above.
- Check the invitation text, dark backdrop, and sunflower at both a narrow phone-sized viewport and a wide desktop-sized viewport.
- Observe the existing bloom animation. If your change introduces an interaction, try it in the browser.
- Check local image, audio, and font references added to `index.html` against files that exist at those paths. The root file list contains no separate asset directory.
- If you add media, review whether its dimensions and file size suit its use; avoid keeping oversized or unused files. Before removing an asset, check that no page or style still refers to it.
- Review any external font or script references you add. Keep them only when intentional and used, and consider how the page should render if an external font cannot load.

## Accessibility review checklist

Use these as future review steps, not as claims of verified accessibility.

- If the page has interactive elements, try to reach and operate each one using only the keyboard. Check that the bloom or any other interaction does not depend on pointer input alone.
- Check that keyboard focus is visible against the dark backdrop and remains easy to track.
- Review the invitation and any control text for clear meaning. If controls are added, check that each has a meaningful accessible name.
- Check the contrast of the invitation and any other text against the dark background, including after color changes.
- If you add an image, check whether it communicates meaningful content and needs a text alternative; keep decorative imagery from creating redundant announcements.
- Check the bloom animation with reduced motion requested. Consider reducing or stopping nonessential motion in that case.