# Changelog

## 1.0.1 - 2026-09-13

- Fix: gen1online is now pinned at **0.3.0** via
  [notquiteog/Gen1Online](https://github.com/notquiteog/Gen1Online), a
  byte-identical mirror of upstream's `v0.3.1` archive re-tagged to the
  version the mod's manifest actually declares. Upstream's mislabeled tag made
  the pinned 0.3.1 never match the installed 0.3.0, so a sealed cart refused
  to enforce and disabled the whole mod set. Cart content is otherwise
  unchanged from 1.0.0.

## 1.0.0 - 2026-09-13

- First cut of the sealed Yellow Online cart: 58 pinned mods on a Yellow base,
  built around Gen1Online 0.3.1 (the last Gen-1-era build), the full FAFF0x
  QoL + quest suite, the voxel diorama, followers, skies, rides and the
  community's QoL and art mods. Locked to 1x speed.
