# Flowery

A small animated sunflower-themed static page built around the invitation “Have a flower.” The top-level `index.html` presents a dark backdrop and a central blooming flower. The repository root lists only `index.html` and this README.

## Preview locally

No package installation is needed. Open `index.html` in a browser, or serve the repository directory:

```sh
python -m http.server 8000
```

Then visit http://localhost:8000. No deployment configuration is documented.

## Personalizing the page

Locate the existing invitation text and the styles for the dark backdrop and sunflower in `index.html` before changing them. If you introduce an external image or another asset, add it deliberately and update its reference in `index.html` to match its actual path; no separate asset directory is listed at the repository root.

## Troubleshooting

Use these as diagnostic steps, not as claims that the page currently has a problem:

1. **Confirm the entry page.** Open the top-level `index.html`, or serve the repository directory and visit its root URL. If you serve a different directory, the page you see may not be this project entry.
2. **Check paths and local files.** Preserve relative paths when moving the page or adding assets. If a local image or other asset fails to load, check that the file is present and that the reference in `index.html` matches its location. The listed root files do not include a separate asset directory.
3. **Inspect browser diagnostics.** Check the console for errors during page load or the bloom animation. Use the Network panel to inspect failed requests and their URLs; this can help distinguish an incorrect local path from another loading failure.
4. **Distinguish external requests.** A missing local file is different from an external resource that cannot be reached over the network. No external resources are identified in the current page references; if you add one, verify that it is intentional and that the page remains understandable when it is unavailable.

## Configuration and data handling

This repository is a static page with no package or backend configuration listed. No `.env.example` is present. Do not add credentials or private values to `index.html` or other tracked files: anything embedded in a static page is delivered to visitors and cannot be secret. The page's text and any added assets are part of the site content, so review personal details and media before sharing or publishing the page.

## Browser and layout review checklist

This is a checklist for future review, not a report of completed browser testing or verified results.

- Open the page in current versions of browsers relevant to its intended audience. Review both a directly opened page and the local-server view if asset paths are relevant to your changes.
- Check the invitation, dark backdrop, and sunflower at a narrow phone-sized viewport and a wide desktop-sized viewport. Look for clipping, overflow, or layout changes that make the invitation or flower hard to see.
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