# Delixon Labs Scoop bucket

Scoop manifests for [QiloBack](https://qiloback.dev) on Windows.

## Install QiloBack

```powershell
scoop bucket add delixon-labs https://github.com/delixon-labs/scoop-bucket
scoop install qiloback
```

## Update

```powershell
scoop update qiloback
```

## Remove

```powershell
scoop uninstall qiloback
scoop bucket rm delixon-labs   # optional
```

## How this bucket is maintained

Manifests here are auto-updated by the
[`release-package-managers.yaml`](https://github.com/delixon-labs/qiloback-core/blob/main/.github/workflows/release-package-managers.yaml)
workflow on every `v*.*.*` tag push. Workflow steps:

1. Build the Windows x64 binary.
2. Compute its SHA-256.
3. Rewrite `bucket/qiloback.json` with the new version + sha256 +
   asset URL.
4. Open a PR (or push directly under release branch protection).

Do not edit manifests by hand — the next release overwrites them.

## Reporting issues

The CLI lives at
[`delixon-labs/delixon-qiloback`](https://github.com/delixon-labs/delixon-qiloback).
File issues there.

## License

[FSL-1.1-ALv2](https://github.com/delixon-labs/delixon-qiloback/blob/main/LICENSE).
