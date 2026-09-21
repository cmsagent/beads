# Our Bead Shop

The homepage is built automatically by GitHub Pages from the `main` branch. The currently configured custom domain is **hama.stevensnetwork.co.uk** (see `CNAME`).

## Add a photo

1. Add your photo to `assets/` in this repository.
2. Give it a descriptive filename, such as `rainbow-star.jpg`.
3. Commit and push to `main` (or use GitHub’s Upload files button).

When the Pages deployment finishes, the photo appears automatically with a title from its filename: `rainbow-star.jpg` becomes **Rainbow star**. Supported formats: JPG, JPEG, PNG, WebP, GIF and AVIF, including uppercase extensions. Images in subfolders of `assets/` are also included. Convert HEIC photos to one of these formats first.

The six original designs stay first in their original order. New photos follow in path order. Removing an image removes its card on the next build. Replacing an image updates the existing card.

## Optional custom labels

Edit `_data/products.json` to add a title, caption or alt text keyed by the photo’s path (for example `/assets/rainbow-star.jpg`). No metadata is required for new photos.

## Publishing

GitHub Pages processes the Liquid templates in `index.html` and `_includes/` using Jekyll. Keep the YAML front matter at the top of `index.html` and do not add a `.nojekyll` file. No additional GitHub token or browser API request is needed.

If a separate AWS deployment is used in future, deploy Jekyll’s generated `_site/` output rather than the unprocessed source files. Changing to `beads.stevensnetwork.co.uk` requires updating the custom domain and DNS; this change preserves the current `hama` domain.
