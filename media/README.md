# Media replacement guide

The website reads these files directly. Preserve filenames to replace media without changing code.

## Video posters

Folders: `films/`, `experimental/`, `commercials/`, `live/`

Recommended: JPG, 16:9, at least 1280 × 720. The YouTube link and duration label are configured in `src/content/siteContent.js`.

## Photography

Folder: `photography/`

Files are `photo-01.avif` through `photo-28.avif`. Any image dimensions are accepted; the collage uses `object-fit: cover`, so a different aspect ratio may crop. For exact control, edit the relevant `x`, `y`, `width`, and `height` values in `gallerySections` inside `src/content/siteContent.js`.

## Graphic design

Folder: `design/`

Files are `design-01.avif` through `design-13.avif`. The same collage rules apply as photography.

## Branding

- `branding/logo.avif`: centered blue header symbol, transparent background preferred.
- `branding/signature.avif`: small mark beside the photography credit.

## Formats

If you change a file extension, update its path in `src/content/siteContent.js` and `scripts/check-media.mjs`. Keeping the existing extension is the simplest workflow.
