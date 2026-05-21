# Public Task Screenshots

This repository stores public, non-sensitive screenshots and small image artifacts used as evidence in Kaneo comments, GitHub pull requests, issues, and CI/debugging notes.

## Public Data Warning

Everything committed here is public on the internet. Do not upload secrets, tokens, API keys, private chats, customer or user data, internal admin panels, credentials, browser sessions, billing pages, private infrastructure details, or screenshots that could expose sensitive information.

If a screenshot contains any private or ambiguous content, redact it before upload or do not upload it here.

## Upload Policy

Uploads should be made through the Home Server API-only uploader. Do not clone this repository for routine uploads.

Default policy:

- Max file size: 10 MB before processing.
- Metadata is stripped before upload.
- PNG screenshots may be converted or optimized to WebP/JPEG when appropriate.
- Uploads require an explicit `--public-ok` flag.
- Paths should be deterministic and contextual, for example:
  - `kaneo/<task-id>/<YYYY-MM-DD-HHMMSS>-<slug>.webp`
  - `prs/<owner>/<repo>/<pr-number>/<YYYY-MM-DD-HHMMSS>-<slug>.webp`

## Rotation Policy

Keep this repository under roughly 5 GB. When it grows too large, rotate by year or by source repository, for example `task-screenshots-2027` or `task-screenshots-home-server`, instead of rewriting history.
