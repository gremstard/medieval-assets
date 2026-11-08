# Medieval Assets

A collection of medieval and fantasy 3D asset packs — environments, characters,
props, weapons, animations, and audio.

## Where the files are

The archives are **not stored in git**. They live as assets on the
[latest release](../../releases/latest).

Two reasons: GitHub hard-rejects any file over 100 MB (six of these exceed it,
the largest at 320 MB), and these are already-compressed `.zip`/`.rar`
archives — re-compressing them gains nothing measurable. GitHub Releases
allows up to 2 GB per file and doesn't count against repository size.

## Contents

| Release asset | Size | SHA-256 (truncated) |
|---|---:|---|
| `5_free_medieval_village_textures.zip` | 74M | `7cabbe71fe353505…` |
| `Fantasy.Props.MegaKit.Standard.zip` | 148M | `8b6f7e806d222e58…` |
| `Medieval.Village.MegaKit.Standard.zip` | 154M | `e60dea67c10f30dc…` |
| `Modular.Character.Outfits.-.Fantasy.Standard.zip` | 288M | `c3468b18871cc8c8…` |
| `Stylized.Nature.MegaKit.Standard.zip` | 103M | `298f6732b872e4cf…` |
| `Universal.Animation.Library.Standard.zip` | 15M | `cc73fc4e495b8295…` |
| `Universal.Base.Characters.Standard.zip` | 129M | `fdbf1804c90dfc1e…` |
| `Weapons_Shields_Free.zip` | 448K | `f3e838ff7adde8a1…` |
| `medieval_village_clear_pbr_review.zip` | 14M | `302114734653aca4…` |
| `soiTavern_fbx.zip` | 320M | `21e31f5ed0bb91ff…` |
| `WeaponsPack.rar` | 2.7M | `b0df80d07fcb8c64…` |
| `Medieval.Melancholy.ogg` | 1.5M | `b6afc02914c97750…` |

Total payload: 1.19 GB across 12 assets.

Note: GitHub rewrites spaces and brackets in release asset names to dots, so
the names above differ from the original vendor filenames (e.g.
`Fantasy Props MegaKit[Standard].zip` is published as
`Fantasy.Props.MegaKit.Standard.zip`).

## Downloading

Grab individual packs from the [releases page](../../releases/latest), or pull
everything at once with the GitHub CLI:

```bash
gh release download v1.0.0 --repo gremstard/medieval-assets --dir ./assets
```

## Verifying a download

Checksums above are truncated to the first 16 characters for readability.
To verify a file you've downloaded:

```bash
shasum -a 256 "soiTavern_fbx.zip"
```

Compare the leading characters against the table.

## Licensing

These are third-party asset packs, each carrying its own license from its
original vendor — mostly free/standard-license packs. Check the license
bundled inside a given pack before shipping anything built from it
commercially; the terms vary between vendors.
