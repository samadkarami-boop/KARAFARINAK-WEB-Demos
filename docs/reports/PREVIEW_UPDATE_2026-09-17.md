# KARAFARINAK Preview Update — 2026-09-17

## Current state
- Preview repository: `samadkarami-boop/KARAFARINAK-WEB-Demos` (public).
- Homepage: `theme-preview/index.html`.
- Styles: `theme-preview/style.css`.
- Current Preview Hero asset is `theme-preview/hero-robots.svg`.
- The main WordPress repository contains the canonical Hero image `assets/images/hero-robots.jpg` (about 617 KB), and the WordPress CSS references that JPG directly.

## Verification performed
- Confirmed the Preview homepage contains the four compact cards and their four SVG card illustrations.
- Confirmed the Preview CSS currently references `hero-robots.svg`.
- Confirmed the SVG exists in the Preview repository.
- Confirmed the canonical JPG exists in the private WordPress repository.
- Confirmed the Preview repository has a GitHub Pages deployment workflow at `.github/workflows/static.yml`.

## Important constraint
The connected GitHub file API can read the private JPG, but the binary blob cannot be written into the public Preview repository through the available UTF-8 file-update operation. The raw binary fetch also cannot be passed directly as a binary file between the two repositories. Therefore the canonical JPG has **not** been replaced by a redesigned/conversion substitute.

## Required next step
To complete the requested visual test with the exact canonical JPG, the original `hero-robots.jpg` must first be made available to the public Preview repository (or to a public asset URL) without converting/redesigning it. After that:
1. Point `theme-preview/style.css` to the real JPG.
2. Trigger GitHub Pages deployment.
3. Open the live Preview and verify the Hero image actually loads.
4. Verify desktop/mobile Hero proportions and the four-card layout.
5. Record the successful deployment/test commit here.

## Do not do
- Do not replace the canonical JPG with `hero-robots.svg` for the final test.
- Do not redesign or regenerate the Hero image while claiming it is the original asset.
