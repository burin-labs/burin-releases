# Burin Code releases

Signed downloads for [Burin Code](https://burincode.com/). This repository holds release
assets and nothing else: no source code, and no issue tracker.

## Install

macOS, with Homebrew:

```sh
brew tap burin-labs/burin
brew install --cask burin-code   # the macOS app
brew install burin               # the terminal UI
```

Or download the assets for your platform from the
[latest release](https://github.com/burin-labs/burin-releases/releases/latest).

## What each release contains

- `Burin.Code.dmg`: the macOS app, signed with a Developer ID and notarized by Apple.
- `burin-<target>.tar.gz`: the terminal UI for macOS (Apple silicon and Intel) and
  Linux (x86_64 and arm64).
- `release.json`: the manifest. It lists every asset with its SHA-256 and size.

## Verify a download

Compare the file's SHA-256 with the value `release.json` lists for it:

```sh
shasum -a 256 Burin.Code.dmg
```

## License

The binaries are proprietary. Use of them is governed by [LICENSE](LICENSE).
