# Changelog

## 1.1.0 - 2026-09-13

- Core swap: Gen1Online is out, [RBY MMO](https://github.com/alamops/RBYMMOMod)
  1.4.1 is in. Gen1Online's Gen-1 line ended at 0.3.x and its service stopped
  working; RBY MMO hosts from inside the game (dedicated hub optional),
  supports trades and PVP battles on the spot, declares gen1 explicitly, its
  tag matches its manifest, and it needs no undeclared permissions. Pin count
  stays 58.


## 1.0.3 - 2026-09-13

- Update: overworld_wild_spawns 2.1.9 -> 2.2.0 (its manifest and tag now agree,
  gen1 support unchanged; FOLLOWERS_EX depends on this mod without a version
  constraint, so the dependency holds).
- Checked every other pin against its repo's releases: all are already the
  latest installable build. kanto_life 0.8.35 is published with no release
  assets, so 0.8.34 remains the newest installable. The FAFF0x mirrors are
  current with upstream's repo (45 zips, no newer commits). gen1online stays
  at 0.3.0: 0.4/0.5 "Gen1Online++" is Crystal-only, and this cart is Yellow.

## 1.0.2 - 2026-09-13

- Fix: the mirrored Gen1Online archive now declares the `compute` permission.
  The mod's netcode runs on `love.thread`, which the engine's sandbox refuses
  unless `compute` is in `manifest.json` - upstream never declared it, so the
  mod failed to load with "needs the compute permission". The mirror's zip is
  upstream's archive with exactly that one manifest line added; the pin sha
  changed accordingly. Cart content is otherwise unchanged.

## 1.0.1 - 2026-09-13

- Fix: gen1online is now pinned at **0.3.0** via
  [notquiteog/Gen1Online](https://github.com/notquiteog/Gen1Online), a
  byte-identical mirror of upstream's `v0.3.1` archive re-tagged to the
  version the mod's manifest actually declares. Upstream's mislabeled tag made
  the pinned 0.3.1 never match the installed 0.3.0, so a sealed cart refused
  to enforce (which disabled every mod, Battle Art Voxel included). Cart
  content is otherwise unchanged from 1.0.0.

## 1.0.0 - 2026-09-13

- First cut of the sealed Yellow Online cart: 58 pinned mods on a Yellow base,
  built around Gen1Online 0.3.1 (the last Gen-1-era build), the full FAFF0x
  QoL + quest suite, the voxel diorama, followers, skies, rides and the
  community's QoL and art mods. Locked to 1x speed.
