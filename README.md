# Horizon Free — All Platforms

An independent distribution of Horizon Free maintained by
[parthdongre](https://github.com/parthdongre), with a native **macOS Apple Silicon
launcher** and links to the original Windows and Linux builds.

**Credit to [0CYBER](https://github.com/0CYBER): creator of the original
[Horizon Free repository](https://github.com/0CYBER/horizon-free) and its
Windows/Linux launcher builds.** This project builds on that fork.
The Horizon game and original launcher were created by
[Ludovic Marie and the Horizon contributors](https://github.com/horizon-rust/horizon).

## Download

| Platform | Download | Build creator |
| --- | --- | --- |
| macOS Apple Silicon (M1 and newer) | [DMG installer](https://github.com/parthdongre/horizon-free-all-platforms/releases/latest/download/horizon-launcher-macos-arm64.dmg) · [ZIP](https://github.com/parthdongre/horizon-free-all-platforms/releases/latest/download/horizon-launcher-macos-arm64.zip) | parthdongre, based on Horizon Free |
| Windows x64 | [0CYBER's releases](https://github.com/0CYBER/horizon-free/releases/latest) | 0CYBER |
| Linux x86-64 | [0CYBER's releases](https://github.com/0CYBER/horizon-free/releases/latest) | 0CYBER |

[Release notes and checksums](https://github.com/parthdongre/horizon-free-all-platforms/releases/latest)

This repository currently publishes macOS Apple Silicon binaries. Windows and
Linux downloads above are the original packages published by 0CYBER. An Intel
macOS binary has not been built or tested for this distribution.

## Install on macOS

1. Download the DMG, open it, and drag **Horizon** into **Applications**.
2. Open Horizon. The app is signed ad hoc, not Apple-notarized. If macOS blocks
   it, attempt to open it once, then use **System Settings → Privacy & Security
   → Open Anyway**.
3. Select your existing Minecraft installation in **Settings → Minecraft
   folder**, install a Horizon game version, and prepare its resources.

Requires macOS 12 or later and Apple Silicon. Minecraft game files, assets,
and worlds are not included. Use your own matching Minecraft installation.
Horizon is a native Rust game; TLauncher can provide the existing Minecraft
files for preparation. See the [macOS setup and build guide](MACOS-BUILD.md)
for directory layouts and renamed Fabric profiles.

The launcher retains Horizon Free's existing offline-account behavior.
Authenticated multiplayer still depends on the server's account requirements.
Launcher updates come from this repository; native game releases come from
[horizon-rust/horizon](https://github.com/horizon-rust/horizon).

## Build and contribute

- [Build and verify on macOS](MACOS-BUILD.md)
- [Contributing](CONTRIBUTING.md)
- [Launcher architecture and CLI](launcher/README.md)
- [Upstream technical documentation](docs/README.md)

The full source tree is retained so the launcher and game remain buildable.
Inherited upstream workflows reference upstream release infrastructure; they
are not required for the local macOS build described here.

## Credits and license

See [CREDITS.md](CREDITS.md), [LICENSE](LICENSE), and
[THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md). The source is MIT-licensed;
original copyright and dependency notices are preserved.

Not an official Minecraft product. Not affiliated with or endorsed by Mojang,
Microsoft, 0CYBER, or the upstream Horizon maintainers.
