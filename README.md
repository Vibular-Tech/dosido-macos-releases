# Dosido for macOS — releases

Release builds of the Dosido menu-bar app for macOS, and the Sparkle appcast that installed copies check for updates.

## Install

1. Download the latest `Dosido-x.y.z.dmg` from [Releases](https://github.com/Vibular-Tech/dosido-macos-releases/releases/latest).
2. Open the DMG and drag `Dosido.app` onto the Applications shortcut.
3. Launch Dosido from `/Applications`. Updates arrive automatically after that.

## What's here

- `appcast.xml` — the update feed. Installed copies read it from `https://raw.githubusercontent.com/Vibular-Tech/dosido-macos-releases/main/appcast.xml`. Do not rename this repo or move the file: that URL is compiled into every shipped build.
- Releases — each one carries a notarized DMG (for first installs) and a zip (what Sparkle downloads). Every update is signed with Dosido's EdDSA key and verified by the app before it installs.

This repo is written by the macOS app's release script. Don't edit it by hand.
