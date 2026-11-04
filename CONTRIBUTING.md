# Contributing

This is parthdongre's independent distribution of
[0CYBER's Horizon Free](https://github.com/0CYBER/horizon-free), based on
[Horizon](https://github.com/horizon-rust/horizon). See [CREDITS.md](CREDITS.md)
for authorship and platform-build attribution.

Open issues and pull requests in
[parthdongre/horizon-free-all-platforms](https://github.com/parthdongre/horizon-free-all-platforms).
Do not claim upstream issues or contact upstream maintainers on behalf of this fork.

## Build and validate

Follow [MACOS-BUILD.md](MACOS-BUILD.md). Use Rust 1.99.1 for this launcher
revision and the `gpui_platform/runtime_shaders` feature on macOS when the
optional Metal compiler is absent.

Before sending a change:

```sh
python3 tools/check_public_tree.py
cargo +1.99.1 fmt --manifest-path launcher/Cargo.toml -- --check
```

Run the tests relevant to the change. For gameplay changes, retain upstream's
vanilla parity tests and read [the parity workflow](docs/parity-workflow.md).
Test app launches with fresh temporary game and launcher homes, as described
in AGENTS.md, so existing player worlds and accounts are not touched.

Never commit Minecraft jars, assets, prepared resources, credentials, local
logs, or build outputs. Keep these in ignored local folders. Attach launcher
installers to GitHub Releases rather than adding binaries to Git history.

Preserve the MIT copyright, 0CYBER's Horizon Free attribution, and third-party
notices. Describe what changed, why, which platforms were verified, and any
remaining limitations in your pull request.
