# QuickDraw Updates

Public hosting repository for QuickDraw Sparkle updates.

## Purpose

This repo hosts the Sparkle appcast (`appcast.xml`) via GitHub Pages.

Release archives (`.dmg`) are uploaded as GitHub Release assets.

## Sparkle feed URL

`https://mushroom-theory-inc.github.io/quickdraw-app/appcast.xml`

## Release process (high level)

1. Build and notarize new QuickDraw DMG from source repo.
2. Upload DMG to a GitHub Release in this repository.
3. Run Sparkle `generate_appcast` against a local folder of historical archives.
4. Commit updated `appcast.xml` to this repo.
5. Push to `main` (GitHub Pages serves updated feed).

## Files

- `appcast.xml` — Sparkle feed consumed by app clients.
- `release-notes/` — optional markdown/html release notes linked from appcast.
