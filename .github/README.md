# MHGU Recomp for iPad

This is a fork of [morerokk/MHGURecomp](https://github.com/morerokk/MHGURecomp), the native PC port of Monster Hunter
Generations Ultimate, that builds and releases it for **iPad**. It renders at the screen's real resolution, with the
whole HUD visible on a 4:3 screen.

Every upstream release is merged in and built here automatically. Upstream's features and settings stay as they are,
and only what iPadOS needs is added. Touch controls are not included: play with a controller.

No game data is included in this repository. You need your own dump of MHGU 1.4.0.

## Download

[Releases](https://github.com/cerroverb/MHGURecomp-iPad/releases): `MHGURecomp-iPad.<version>.ipa`. The version is
upstream's plus one more number: `0.14.0.1` is upstream 0.14.0. Releases are pre-releases until they have been
played on an iPad.

## Install

1. Sideload the IPA with a tool such as [iloader](https://github.com/nab138/iloader). Use a separate Apple Account.
2. Start the app once so it creates its folders.
3. In the Files app, put the game's `exefs` and `romfs` folders (MHGU 1.4.0) in `MHGURecomp/data`.

The settings menu opens with Plus + Minus on a controller. Everything else works as described in
[upstream's README](https://github.com/morerokk/MHGURecomp#readme).

## Requirements

- An Apple Silicon iPad on iPadOS 15 or newer
- A controller
- A sideloading tool and an Apple Account

## What differs from upstream

- Mach-O and iOS support: a host layer for iPadOS, MoltenVK, a game code library linked into the app
- the game folder in the app's Documents, and the system text box for names
- the screen's size in pixels, and pictures as narrow as 5:4

The branch with these changes is [`ipad`](https://github.com/cerroverb/MHGURecomp-iPad/tree/ipad).

## Problems

iPad-specific problems: open an issue here. Everything else is upstream's: please report it
[there](https://github.com/morerokk/MHGURecomp/issues).

## Credits and license

All credit for MHGU Recomp goes to morerokk and its contributors. The iOS layer builds on
[WiseManChris/MHGURecomp-iOS](https://github.com/WiseManChris/MHGURecomp-iOS),
[Kamisorara/MHGURecomp-iOS](https://github.com/Kamisorara/MHGURecomp-iOS) and mhvuze's macOS port. MIT license, as
upstream (`LICENSE`). LLM assistance was used to port and maintain the iPad build.
