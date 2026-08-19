# QA Scout — report

- URL: https://www.saucedemo.com
- Date: 2026-08-19
- Scout version: 0.1.73

## Result

1 of 6 checks found problems.

## How the checks went

- Pages: passed 5 of 5
- SEO: passed 1 of 1
- API: not in this scan
- Source: not in this scan
- CI: not in this scan
- CD: not in this scan
- Accessibility: failed 1 of 1
- Visual: passed 3 of 3
- Headers: passed 2 of 2
- Links: passed 2 of 2
- GraphQL: not in this scan

## What we found

- Accessibility did not pass.
- SEO volume (descriptions / sitemap orphans) is summarized below, not here.

## Fix first

- Select element must have an accessible name (www.saucedemo.com/inventory.html)
- Missing Strict-Transport-Security (www.saucedemo.com)
- Missing Content-Security-Policy (www.saucedemo.com)

## Appendix

SEO volume — real, but not the same as a broken link.

- 1 page: title outside 10–70 characters
- 1 page: description outside 50–170 characters

Technical detail for your developers is in `developers.md` and `findings.json`.

## Screenshots

Visual pass (compared to baseline).

![390 × 844; Mobile](screenshots/visual-baseline-390x844-1.png)

![768 × 1024; Tablet](screenshots/visual-baseline-768x1024-2.png)

![1280 × 800; Desktop](screenshots/visual-baseline-1280x800-3.png)

![a11y · failed gate](screenshots/a11y-failed.png)
