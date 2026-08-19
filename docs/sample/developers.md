# QA Scout — report

- URL: https://www.saucedemo.com
- Date: 2026-08-19
- Scout version: 0.1.73
- Slots run: url, seo, a11y, visual, headers, links
- Slots skip: api, source, ci, cd, graphql
- Slots baseline: —

## Gates

- url (URL / E2E): pass 5/5
- seo (SEO): pass 1/1
- api (API): skip — no context
- source (Source): skip — no context
- ci (CI): skip — no context
- cd (CD): skip — no context
- a11y (A11y): fail 1/1 — select-name
- visual (Visual): pass 3/3
- headers (Headers): pass 2/2
- links (Links): pass 2/2
- graphql (GraphQL): skip — no context

## Findings

Findings are not a Scout failure. Gates (the spec) are separate.

- S2/P2 `a11y-select-name` (https://www.saucedemo.com/inventory.html): Select element must have an accessible name
  - `select` — `<select class="product_sort_container" data-test="product-sort-container"><option value="az">Name (A to Z)</option><option value="za">Name (Z to A)</option><option value="lohi">Pri`
- S2/P2 `headers-missing-hsts` (https://www.saucedemo.com/): Missing Strict-Transport-Security — Hardening finding, not a broken suite
- S3/P3 `headers-missing-csp` (https://www.saucedemo.com/): Missing Content-Security-Policy

## Appendix

SEO volume — real, but not the same as a broken link.

- 1 page: title outside 10–70 characters
- 1 page: description outside 50–170 characters

Per page:

- S4/P4 `seo-title-length` (https://www.saucedemo.com/inventory.html): Title length outside 10–70 characters — 9 chars
- S4/P4 `seo-description-length` (https://www.saucedemo.com/inventory.html): Meta description length outside 50–170 characters — 24 chars

## Other

Honest S3/S4 — not hidden, not equal to P2.

- S3/P3 `seo-missing-h1` (https://www.saucedemo.com/inventory.html): No h1 in crawl snapshot
- S3/P3 `headers-missing-clickjacking` (https://www.saucedemo.com/): No X-Frame-Options or CSP frame-ancestors
- S4/P4 `headers-missing-referrer-policy` (https://www.saucedemo.com/): Missing Referrer-Policy
- S3/P3 `headers-missing-x-content-type-options` (https://www.saucedemo.com/): Missing X-Content-Type-Options — nosniff not set — passive WSTG

## Visual

Visual pass (compared to baseline).

![390 × 844; Mobile](screenshots/visual-baseline-390x844-1.png)

![768 × 1024; Tablet](screenshots/visual-baseline-768x1024-2.png)

![1280 × 800; Desktop](screenshots/visual-baseline-1280x800-3.png)

## Gate screenshots

![a11y · failed gate](screenshots/a11y-failed.png)
