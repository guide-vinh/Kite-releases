# Kite

Kite is a lightweight, native macOS IDE for working with Claude Code and Codex: a file tree, a fast terminal, git
review and commit, and a light code viewer and editor. It stays small and fast on purpose: no LSP, no debugger,
no plugins, no indexing.

This repository holds Kite's published builds and its update feed. The source code is not here.

## Download

Get **Kite-x.y.z.zip** from the [latest release](https://github.com/guide-vinh/Kite-releases/releases/latest).

Requirements: macOS 14 Sonoma or later.

## Install

1. Unzip the download.
2. Drag **Kite.app** into your **Applications** folder.
3. Open Kite. The app is signed with a Developer ID and notarized by Apple, so it opens without a security warning.

## Updates

Kite updates itself through [Sparkle](https://sparkle-project.org):

- **Kite → Check for Updates…** checks right away.
- Automatic checks can be turned on or off in **Settings → General**.
- Every update is checked against Kite's signing key before it installs.

The feed Kite reads is [`appcast.xml`](appcast.xml) in this repository.

## Privacy

Kite sends no telemetry and makes no network calls of its own. The only exception is the update check: it reads
`appcast.xml` from this repository and downloads the update zip when you install one.

## What's in this repository

| Path | What it is |
| --- | --- |
| [Releases](https://github.com/guide-vinh/Kite-releases/releases) | One release per version, each with the notarized `Kite-x.y.z.zip` |
| `appcast.xml` | The Sparkle update feed: version, build number, download link and signature of each release |

The release script updates `appcast.xml` automatically. Please do not edit it by hand: a wrong entry breaks updates
for everyone.
