# QA Scout

Desktop health-check for a live website. Scout crawls a URL, runs Playwright gates, and exports a short client PDF plus a developer zip.

Gates include pages, SEO, accessibility, visual, headers, and links. After one crawl, selected gates can run in parallel.

## Download

**macOS, Apple Silicon:** [Releases](https://github.com/asxyw/qa-scout-app/releases)

Current build: **0.1.70**.

## Install on Mac

1. Download `QA-Scout-0.1.70-mac-arm64.zip` and unzip it.
2. Move `QA Scout.app` to Applications, or run it from Downloads.
3. First launch: **right-click → Open**. macOS will warn because this build is not Apple-notarized yet. Confirm Open.
4. Sign in, or start a **3-run trial** on this Mac.

Intel Macs are not in this release.

## Starter access

Paid login is not self-serve yet. You can [request a Starter](https://scout-api.win) (30 days, 20 runs a month). Reply goes to the email you give.

Or message Telegram [@asxyw](https://t.me/asxyw).

## License

Trial: **3 runs** per computer. A new account does not give another trial on the same Mac.

Crawl data, screenshots, and PDFs stay on your Mac.

## What you get

- Catalog of pass / fail / skip per gate
- Client PDF in plain language (no locators)
- Developer zip: `developers.md`, `findings.json`, evidence

Accessibility findings in the developer zip name the element (for example which image is missing `alt`). The client PDF stays short.

## Requirements

- macOS on Apple Silicon
- Network access to the site you scan

This repository is the download page. It does not contain product source.

## Author

[asxyw](https://github.com/asxyw)
