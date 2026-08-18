# QA Scout

**QA Scout catches bugs before your users do.**

Automated testing for web pages, accessibility, SEO, visual regressions, APIs, source, and CI/CD — in one desktop pass.

Scout crawls a live URL, runs the gates, and exports a short PDF for the client plus a zip for engineers.

Site gates always run from the URL. Paste a public GitHub repo for source and CI/CD. Attach OpenAPI for API checks.

## Download

**macOS, Apple Silicon:** [Releases](https://github.com/asxyw/qa-scout-app/releases)

Current build: **0.1.70**.

## Install on Mac

1. Download `QA-Scout-0.1.70-mac-arm64.zip` and unzip it.
2. Move `QA Scout.app` to Applications, or run it from Downloads.
3. First launch: **right-click → Open**. macOS will warn because this build is not Apple-notarized yet. Confirm Open.
4. Sign in, or start a **3-run trial** on this Mac.

Intel Macs are not in this release.

## Use it

1. Save a project with the site URL.
2. Run **Standard**. That is pages, SEO, accessibility, visual, headers, and links.
3. Optional: add an **OpenAPI** file for API checks.
4. Optional: paste a **public GitHub URL** and Clone. That turns on Source, CI, and CD (workflows, artifacts, no plaintext secrets). A github.com Base URL stays the website — it is not the repo.
5. Export: short client PDF (plain language) and a developer zip (`developers.md`, `findings.json`, evidence).

No signal on a gate means skip, not a fake pass.

## Starter access

Paid login is not self-serve yet. You can [request a Starter](https://scout-api.win) (30 days, 20 runs a month). Reply goes to the email you give.

Or message Telegram [@asxyw](https://t.me/asxyw).

## License

Trial: **3 runs** per computer. A new account does not give another trial on the same Mac.

Crawl data, screenshots, and PDFs stay on your Mac.

## Requirements

- macOS on Apple Silicon
- Network access to the site you scan

This repository is the download page. It does not contain product source.

## Author

[asxyw](https://github.com/asxyw)
