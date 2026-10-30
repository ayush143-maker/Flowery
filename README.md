# Flowery

Flowery is a self-contained animated flower page built around the caption “Have, a flower.” A sunflower blooms against a dark, starry backdrop, with a **regrow** control for replaying the animation. The illustration is generated in the page rather than loaded from image files.

## Preview locally

No package installation is needed. Open `index.html` in a browser, or serve the repository directory:

```sh
python -m http.server 8000
```

Then visit [http://localhost:8000](http://localhost:8000). The top-level `index.html` is the complete page entry point; there is no documented build step or deployment configuration.

## Interacting with the flower

The bloom begins when the page’s load event applies its `play` class. Select **regrow** to remove and reapply that class, restarting the CSS bloom animation. The sequence draws a growing stem, leaves, and petals, followed by a glow and sparkles; the completed flower sways gently. CSS also draws a twinkling star field.

The flower head is an inline SVG. Page JavaScript generates 260 seed circles within it using a Fibonacci-phyllotaxis calculation, so the seed pattern is created at runtime rather than fetched as a separate asset. The rest of the flower and its visual effects are made with HTML, CSS, and generated SVG elements.

## Editing and dependencies

The invitation, button, styling, animation, and SVG generation are all in `index.html`. The repository root contains no separate asset directory, and the page references no external images, APIs, or local storage. To change the caption or interaction, edit the page’s existing markup and script; if you add media, place it deliberately and update the corresponding relative reference.

For static publication, serve the repository root so the top-level `index.html` is available. Since the illustration and animation are part of that file, no separate image assets need to be deployed. The page does not save interaction state: reloading starts the bloom again, and the regrow action only restarts its on-page animation.