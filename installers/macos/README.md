# macOS installers

| Version | Installer | Architecture |
| --- | --- | --- |
| 0.6.2 | `craft-anything-0.6.2-macos-aarch64.dmg` | Apple silicon |
| 0.6.1 | `craft-anything-0.6.1-macos-aarch64.dmg` | Apple silicon |

## Verify

From this directory, run:

```sh
shasum -a 256 -c SHA256SUMS.txt
```

## Build and signing

Both installers are locally built from their matching Craft Anything source version using `packaging/macos/package.sh --arch aarch64`.
They use an ad-hoc signature because no Developer ID signing credentials were available; they are not notarized. macOS Gatekeeper may warn or block them when opened. These are local-build installers, not Developer ID signed release artifacts.
