# FlightLog Privacy & Help Site

This repo hosts the public web pages for **FlightLog**, an offline-first RC flight
logbook app for heli, plane, and drone pilots. It's a small set of static HTML
pages — no build step — served via [GitHub Pages](https://pages.github.com/),
covering the app's landing page, an interactive help walkthrough, and the
privacy policy referenced from the app and its Play Store listing.

## Pages

| | English | Deutsch |
|---|---|---|
| Home | [index.html](https://riedlp.github.io/flightlog-privacy/) | [index.de.html](https://riedlp.github.io/flightlog-privacy/index.de.html) |
| Help | [help.html](https://riedlp.github.io/flightlog-privacy/help.html) | [help.de.html](https://riedlp.github.io/flightlog-privacy/help.de.html) |
| Privacy Policy | [privacy.html](https://riedlp.github.io/flightlog-privacy/privacy.html) | *(English only for now)* |

Each language pair links to the other via the flag badge below the nav on the
Home and Help pages.

## Structure

- Every page is self-contained — its own inline `<style>` block, no shared
  CSS file, no dependencies.
- [help.html](help.html) / [help.de.html](help.de.html) include an interactive
  screenshot walkthrough: numbered pins overlay each screenshot and reveal a
  step's explanation on tap (or in a side-by-side list on desktop). The pin
  numbers map to the position of each `<li>` in that screen's list, so the two
  language versions must always keep matching item counts and order.
- `assets/` holds shared images and the intro video, referenced by all pages.

## Editing

There's no build process — edit the HTML directly and commit. When changing
one language version of a page, mirror the change in the other language
version to keep them in sync.
