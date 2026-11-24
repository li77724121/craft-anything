# macOS installer

`craft-anything-0.6.1-macos-aarch64.dmg` is the Apple silicon installer for Craft Anything 0.6.1.

## Verify

From this directory, run:

```sh
shasum -a 256 -c SHA256SUMS.txt
```

## Build and signing

Built from this repository's Craft Anything 0.6.1 source with `packaging/macos/package.sh --arch aarch64`.
The bundle uses an ad-hoc signature because no Developer ID signing credentials were available; it is not notarized. macOS Gatekeeper may warn or block it when opened. This artifact is provided as a locally built installer, not as a Developer ID signed release.
