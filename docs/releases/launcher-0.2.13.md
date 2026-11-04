# Horizon Free launcher 0.2.13 — macOS Apple Silicon

The first macOS launcher release from `parthdongre/horizon-free-all-platforms`.

## Downloads

- `horizon-launcher-macos-arm64.dmg`: open the disk image and drag Horizon to Applications.
- `horizon-launcher-macos-arm64.zip`: the same app as a ZIP archive.
- `SHA256SUMS.txt`: SHA-256 checksums for both downloads.

These macOS builds target Apple Silicon (M1 and newer), require macOS 12 or
later, and are signed ad hoc. They are not Apple-notarized. If macOS blocks a
downloaded copy, use System Settings → Privacy & Security → Open Anyway after
attempting to open it.

The launcher now links to this repository and checks its releases for launcher
updates. Horizon game builds continue to come from `horizon-rust/horizon`.
Minecraft assets are not included: select your existing matching Minecraft
installation and prepare its resources. See [the macOS guide](https://github.com/parthdongre/horizon-free-all-platforms/blob/main/MACOS-BUILD.md).

## Credits and other platforms

**[0CYBER](https://github.com/0CYBER) is the creator of the original
[Horizon Free repository](https://github.com/0CYBER/horizon-free) and its
Windows and Linux launcher builds.** Download those builds from
[0CYBER's releases](https://github.com/0CYBER/horizon-free/releases/latest).
This release adds the macOS Apple Silicon distribution; it does not rebuild
or claim authorship of the Windows/Linux packages.

The Horizon engine and original launcher are by Ludovic Marie and the Horizon
contributors. The app includes the MIT license, credits, and third-party notices.

## Validation

Built natively on Apple M4 with Rust 1.99.1 and runtime Metal shaders. The
launcher window, resource preparation using an existing Minecraft installation,
and a disposable-world launch were tested. Audio and authenticated multiplayer
were not tested. Windows/Linux packages linked above were not retested here.
