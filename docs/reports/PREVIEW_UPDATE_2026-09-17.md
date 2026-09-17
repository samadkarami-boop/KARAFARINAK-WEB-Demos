# KARAFARINAK Preview Update — 2026-09-17

## Current state
- Preview repository: `samadkarami-boop/KARAFARINAK-WEB-Demos` (public).
- Homepage: `theme-preview/index.html`.
- Styles: `theme-preview/style.css`.
- Preview Hero asset remains the configured repository asset; canonical WordPress Hero JPG is tracked separately.

## Forms QA update
The freelance project request form was corrected and verified in the Preview source.

### Project Request form
- Email field is explicitly required and marked with `*`.
- Email uses `type="email"` and `inputmode="email"`.
- Custom email-format validation is active.
- Required-field errors are shown in English only.
- Invalid email error is shown in English only: `Please enter a valid email address.`
- Submit validation error is shown in English only: `Please correct the highlighted fields and try again.`
- Successful demo submission message is shown in English only: `Your project request has been submitted successfully.`
- Submit button uses `type="submit"`.
- The Preview remains a static demo; this success message does not represent real email delivery.

### Verification
- The updated `theme-preview/project-request.html` was written to the `main` branch.
- Final commit: `458b52287602118c2617f78d64a814b90b3e3c0c`.
- Final content SHA: `3f170b1b3967214771dff5f08e87350bd43836f6`.
- The source was re-read after the update to confirm the changes.

## Website Templates page — approved visual state
The page `theme-preview/website-templates.html` was refined and then approved by the user.

### Applied changes
- Removed the old `KARAFARINAK WEB TEMPLATES` eyebrow from the page.
- Kept the main heading `قالب‌های آماده سایت`.
- Both Static and Dynamic feature lists are right-aligned and each line has a green check mark.
- Feature text was made slightly darker/bolder so it does not look washed out.
- Green check marks were made slightly stronger.
- The two green price/position lines at the bottom of the Static and Dynamic sections were aligned to the same vertical level.
- The two bottom action cards/buttons were aligned to the same vertical level.
- Static and Dynamic action cards remain the only clickable areas in the two main sections.
- No change was made to the shared `style.css` for this adjustment; the alignment/contrast refinements are isolated to `website-templates.html`.

### Current code state
- `theme-preview/website-templates.html`
- Commit before backup: `689d77eb9a26eedba5b2462ecd5318d18fb269a3`
- Current content SHA before the backup commit: `ce8eba2dffeb4e8db99d630f617a98447323c991`
- The source was re-read after the update and verified.

## Backup / restore point
Because the user wants an immutable restore point before further visual edits, an exact backup of the approved `website-templates.html` was created:

- Backup file: `docs/backups/website-templates-2026-09-17-approved.html`
- Backup commit: `63a8d305953d227d71cfabc1e3712620cff552a8`
- This backup contains the exact approved HTML/CSS inline state of the page at the time of approval.
- Future edits to this page should be made only after fetching the current file and should not overwrite this backup.
- If a later design change makes the page worse, this backup is the restore reference.

## Live-test limitation
The Preview is static GitHub Pages content. It can test client-side validation and visible layout/source changes, but GitHub connector verification does not provide browser-level visual confirmation. The website-templates source itself was re-read after the latest change. GitHub Pages deployment status was not independently confirmed for commit `689d77eb9a26eedba5b2462ecd5318d18fb269a3` through the available commit-workflow endpoint.
