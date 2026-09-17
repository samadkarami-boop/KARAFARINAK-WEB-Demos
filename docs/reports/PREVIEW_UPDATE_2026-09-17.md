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

## Live-test limitation
The Preview is static GitHub Pages content. It can test client-side validation and the visible success/error messages, but it cannot verify actual WordPress email delivery. Real delivery must be tested on the WordPress site with active `wp_mail`/SMTP configuration.
