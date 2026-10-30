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

## Browser and layout review checklist

This is a checklist for future review, not a report of completed browser testing or verified results.

- Open `index.html` in current versions of browsers relevant to the page's intended audience. Also review it through the local server above, so relative asset paths are checked in a served-page context.
- Inspect the browser console for errors while the page loads and while the bloom animation runs. Investigate errors that could affect the page rather than assuming the visual result is sufficient.
- Inspect the Network panel for failed requests. Check that local assets added to the page resolve at their referenced paths; the root file list contains no separate asset directory. Review any remote requests added to the page and confirm they are intentional.
- Check the invitation, dark backdrop, and sunflower at a narrow phone-sized viewport and a wide desktop-sized viewport. Look for clipping, overflow, and layout changes that make the invitation or flower hard to see.
- Observe the existing bloom animation. If your change introduces an interaction, try it in the browser.
- If you add media, review its dimensions and file size for its use. Before removing an asset, check that no page or style still refers to it.

## Accessibility review checklist

Use these as future review steps, not as claims of verified accessibility.

- If the page has interactive elements, try to reach and operate each one using only the keyboard. Check that the bloom or other interaction does not depend on pointer input alone.
- Check that keyboard focus is visible against the dark backdrop and remains easy to track.
- Review the invitation and any control text for clear meaning. If controls are added, check that each has a meaningful accessible name.
- Check the contrast of the invitation and any other text against the dark background, including after color changes.
- If you add an image, check whether it communicates meaningful content and needs a text alternative; keep decorative imagery from creating redundant announcements.
- Check the bloom animation with reduced motion requested. Consider reducing or stopping nonessential motion in that case.