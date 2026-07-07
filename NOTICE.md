# NOTICE — catalog/

`catalog/` mixes three distinct licensing regimes. The repository-root MPL-2.0
license (`/LICENSE`) does **not** apply uniformly here.

## 1. `catalog/assets/` — proprietary

SUSE brand assets and trademarks (logos, headshots, brand palettes/tokens).
**Proprietary to SUSE — all rights reserved.** NOT licensed under MPL-2.0.
Slated to move to a private repository per the open-sourcing plan (see the root
`README.md` "Open-sourcing plan" and `SOVEREIGNTY.md`).

**Exception — `catalog/assets/suse/music/`:** stock music licensed from
PremiumBeat (Shutterstock) for inclusion in the SUSE catalog and for use as
audio beds in rendered Lolly exports (webm/mp4). The composers retain
ownership — each entry's `description` credits the artist, and the files keep
their original ID3/ISRC metadata. Entries are marked `LicenseRef-PremiumBeat`
in `catalog/assets/index.json`. The licence covers use through the catalog and
app — not re-publishing the tracks as standalone audio elsewhere. These tracks
will be removed from this repository on 2026-08-29 (ahead of the open-sourcing
split; see §1 above).

## 2. `catalog/fonts/` — SIL OFL 1.1

The SUSE and SUSE Mono typefaces are licensed under the **SIL Open Font License,
Version 1.1**. The full license text is in `catalog/fonts/OFL.txt`. Note that
"SUSE" is a trademark of SUSE; the OFL covers the font software, not the mark.

## 3. `catalog/tools/index.json` — generated registry (MPL-2.0)

A generated registry derived from the `tools/` manifests by
`scripts/build-catalog-index.js`. As generated build output of the open-source
toolchain, it is covered by the repository-root **MPL-2.0**. (The underlying
`tools/` content it indexes remains proprietary — see `tools/NOTICE.md`.)
