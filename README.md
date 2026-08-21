<p align="center">
  <img src="icon.png" width="160" height="160" alt="QA Scout">
</p>

<h1 align="center">QA Scout</h1>

<p align="center"><strong>One QA system. One verdict. One report.</strong></p>

<p align="center">
  <a href="https://github.com/asxyw/qa-scout-app/releases"><img src="https://img.shields.io/github/v/release/asxyw/qa-scout-app" alt="GitHub release"></a>
  <img src="https://img.shields.io/badge/macOS-Apple%20Silicon-lightgrey" alt="macOS Apple Silicon">
  <img src="https://img.shields.io/badge/Windows-x64-lightgrey" alt="Windows x64">
  <img src="https://img.shields.io/badge/status-early%20access-blue" alt="early access">
</p>

## Overview

QA Scout is a desktop app for **macOS (Apple Silicon)** and **Windows (x64)**. It crawls a website, runs pages, SEO, accessibility, visual, headers, and links in one pass, and returns a single verdict: a short client PDF plus a developer zip.

After you sign in, the same account data (runs left, time remaining, Scout ID) is on this computer, on the website, and in the Telegram bot. You get those from the app and the welcome email - this page is the download.

## Screenshots

Sample project: [Sauce Demo](https://www.saucedemo.com) (Sauce Labs' public test store, not a real shop).

### Setup

<img src="docs/sample/screenshots/app-setup.png" width="720" alt="QA Scout Setup - Chromium ready">

### Project

<img src="docs/sample/screenshots/app-project.png" width="720" alt="QA Scout Project - Sauce Demo">

### Catalog

<img src="docs/sample/screenshots/app-catalog.png" width="720" alt="QA Scout Catalog - Sauce Demo run list and details">

### Run

<img src="docs/sample/screenshots/app-run.png" width="720" alt="QA Scout Run - Sauce Demo">

## Sample scan

Standard gates on Sauce Demo: pages, SEO, accessibility, visual, headers, links. Sampled 5 pages (max 15, depth 2). API / Source / CI / CD / GraphQL had no context in this scan (skip, not a fake pass).

2 of 6 checks found problems: accessibility (`select-name`) and missing security headers (HSTS / CSP). Pages, visual, and links passed.

<img src="docs/sample/screenshots/report-cover.png" width="720" alt="QA Scout report cover for saucedemo.com">

<details>
<summary>More scan results</summary>

<br>

**Client PDF:** [report.pdf](docs/sample/report.pdf)  |  [report.md](docs/sample/report.md)

**Full pack:** [qa-scout-report.zip](docs/sample/qa-scout-report.zip)  |  [developers.md](docs/sample/developers.md)  |  [findings.json](docs/sample/findings.json)

Visual baselines (mobile, tablet, desktop) and the accessibility fail:

<img src="docs/sample/screenshots/visual-mobile.png" width="280" alt="Sauce Demo inventory, mobile visual baseline">
<img src="docs/sample/screenshots/visual-tablet.png" width="360" alt="Sauce Demo inventory, tablet visual baseline">
<img src="docs/sample/screenshots/visual-desktop.png" width="720" alt="Sauce Demo inventory, desktop visual baseline">

<img src="docs/sample/screenshots/a11y-fail.png" width="720" alt="Accessibility fail on Sauce Demo inventory">

</details>

## Download

Pick your OS. Same release, two zips.

**macOS, Apple Silicon:** [QA-Scout-0.1.81-mac-arm64.zip](https://github.com/asxyw/qa-scout-app/releases/download/v0.1.81/QA-Scout-0.1.81-mac-arm64.zip)

**Windows, x64:** [QA-Scout-0.1.81-win-x64.zip](https://github.com/asxyw/qa-scout-app/releases/download/v0.1.81/QA-Scout-0.1.81-win-x64.zip)

Intel Macs and Windows ARM64 are not in this release. All builds: [Releases](https://github.com/asxyw/qa-scout-app/releases).

## Install

### macOS

1. Download `QA-Scout-*-mac-arm64.zip` and unzip it.
2. Move `QA Scout.app` to Applications, or run it from Downloads.
3. First launch: **right-click -> Open**. macOS will warn because this build is not Apple-notarized yet. Confirm Open.
4. Sign in, or start a **3-run trial** on this Mac.

### Windows

1. Download `QA-Scout-*-win-x64.zip` and unzip it.
2. Open the folder and run `QA Scout.exe`.
3. SmartScreen may warn because this build is not signed. **More info -> Run anyway**.
4. Sign in, or start a **3-run trial** on this PC.

First screen is Setup - Chromium on, then you can run.

## Early access

QA Scout is in early access. [Request free beta access](https://scout-api.win) (30 days, 20 runs/mo). Reply goes to the email you give.

Crawl data, screenshots, and PDFs stay on your computer. Trial: **3 runs** per computer. A new account does not give another trial on the same machine.

[Privacy / Datenschutz](https://scout-api.win/privacy/)

## Author

[asxyw](https://github.com/asxyw)
