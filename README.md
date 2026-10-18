# jejak releases

macOS builds of [Jejak](https://github.com/sakti/jejak), a desktop viewer for
OpenTelemetry traces, metrics and logs, and a Homebrew tap to install them.

## Install with Homebrew

```bash
brew tap sakti/jejak-release https://github.com/sakti/jejak-release
brew install sakti/jejak-release/jejak
jejak --demo
```

Upgrade with `brew upgrade jejak`.

## Download

Each [release](https://github.com/sakti/jejak-release/releases) has a
`.tar.gz` archive for Apple silicon (`aarch64-apple-darwin`) and Intel
(`x86_64-apple-darwin`) Macs, and a `SHA256SUMS` file.

The binaries are not notarized. If you download an archive with a browser,
macOS quarantines it; remove the quarantine before the first run:

```bash
xattr -d com.apple.quarantine jejak
```

Homebrew installs do not need this step.

This repository is updated automatically when a version is tagged in the
Jejak source repository. Do not edit `Formula/jejak.rb` by hand.
