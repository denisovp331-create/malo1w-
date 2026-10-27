# DM RANK

A community leaderboard front-end for RIVALS DM.

## Current prototype
- Responsive dark purple esports layout.
- Player leaderboard, search, filters, statistics cards.
- Screenshot upload and browser-side OCR via Tesseract.js.
- Submission validation and demo storage in browser localStorage.

## Important limitations
This is a front-end prototype. Submissions are currently stored only in the submitting browser and are not visible to other visitors. OCR extracts text but does not verify screenshot authenticity. Do not treat browser-stored entries as an official global leaderboard.

To make this a real public service, connect a dedicated backend/database (e.g. a separate Supabase project), add secure submission storage, duplicate detection, moderator review, and appropriate row-level security. Do not put service-role keys in frontend code.

## Deployment
A GitHub Actions workflow is included in `.github/workflows/pages.yml`. Configure the repository's Pages source to GitHub Actions if GitHub has not enabled it automatically.
