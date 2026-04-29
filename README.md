# scoop-bucket

Scoop bucket for Justyn Clark Network CLI tools and apps.

## Current manifests

- `small.json` - SMALL Protocol CLI for Windows via Scoop.

## SMALL manifest status

Current manifest version: `1.0.10`.

The checked-in manifest points at the `v1.0.10` Windows release assets from `justyn-clark/small-protocol`:

- `small-v1.0.10-windows-amd64.zip`
- `small-v1.0.10-windows-arm64.zip`

The SHA-256 hashes are copied from the GitHub release asset digests for `v1.0.10`.

## Install

```powershell
scoop bucket add jcn https://github.com/justyn-clark/scoop-bucket
scoop install small
```

## Maintenance

When SMALL releases a new version:

1. Update `small.json` `version`.
2. Update the architecture URLs and hashes from the matching GitHub release assets.
3. Keep `autoupdate` using the `v$version` release URL pattern.
4. Verify with Scoop locally before publishing when a Windows/Scoop environment is available.
