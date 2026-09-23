## 1.5.0-test.2

**TEST PRERELEASE — published before gameplay testing at the user’s request.** Includes Gen 1 online doubles, HGSS overworld art (Gen 3 default; opt-in for Gen 1/2), and Battle Art right-stick/door/healing fixes.

Battle Art itself now handles front/back sprite selection across all three generations. Existing animated atlases take priority; supplied BW art is a static full-body fallback. No separate BW mod is included. Gen 1 retains ROM art by default; Crystal retains its Gen 2 animated companion and full-body backs; FireRed selects Gen 5 battle art. Change the shared Battle Art options to opt in/out.

Unsupported generation-specific settings remain visible but read-only (ADAPTER PENDING). Gen 1 doubles, new projection adapters and advanced mechanics are experimental and await gameplay verification. Gen1Recomp 0.3.1 target; no ROMs or saves.

## 1.5.0-test.1 — 2026-09-22

**TEST PRERELEASE — published before gameplay testing at the user’s request.** Build/compile validation only at publication. Includes Gen 1 online doubles, supplied HGSS overworld art (Gen 3 default; opt-in for Gen 1/2), expanded Battle Art settings visibility, and Gen 3 right-stick/door/healing presentation changes. Options lacking a generation adapter are explicitly marked unavailable.

Known risks: new Gen 1 doubles and door/healing projections have not yet been gameplay-tested; advanced moves and disconnect combinations may need fixes. Complete visual parity and all generation-specific settings adapters remain unfinished. Gen1Recomp 0.3.1 is the target engine. No ROM or player save is included. Stable releases remain available.

## 1.4.0 — 2026-09-22

Updates Online 0.7.0, Wilds 2.3.1, Double Battles 0.11.0 and Dramatic Ride 0.3.0; retains Battle Art 1.22.0. Adds optional synchronized mount visuals and fixes the room menu interrupting battle setup.

Includes the five core mods and Running Shoes, with synchronized mount visuals. No extra sprite mod is included.

Verified on Gen1Recomp 0.3.1 in isolated profiles. Known limits: Gen 1 online doubles remain unavailable; Crystal doubles and advanced move combinations remain experimental; the full mixed-mod/disconnect matrix and exhaustive scenery coverage are unfinished. Gen 3 free flight remains within the current map.

Import the attached .g1rcart after importing your own base game. No ROM or save is included. Existing published carts are unchanged; this is a new version.

## 1.3.0 — 2026-09-22

Bundles Battle Art, Online+, Wilds, Double Battles and Dramatic Ride plus Running Shoes. Requires Gen1Recomp 0.3.1 or newer. Includes original-art scenery, Oak lab and settings fixes, host-owned visible encounters and updated native multiplayer integration.

Gen 1/2 online doubles and the full multiplayer disconnect/mixed-mod matrix remain unfinished.

Install the attached .g1rcart. Your own legally obtained and imported base game is required; no ROM is included.

## 1.2.0 — 2.5D worlds and interior dioramas

Pins Battle Art 1.21.0 from our fork, including upstream through 1.11.0.
Adds native-art scenery, reviewed building exteriors, shared render distance
and contextual boundary fill, plus framed interiors and warm lighting.
Requires Gen1Recomp 0.2.73+. Kanto Gear remains absent.
Replaces the upstream Battle Art 1.10.8 pin with our 1.21.0 fork. Yellow base, sealed policy and cartridge artwork are retained.

This is an incremental visual release, not complete Gamma Emerald parity.
Multiplayer doubles and FireRed companion ports remain unfinished.

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

Release preflight: Wild Skies 1.12.3 fixes generated sky cards under native
monochrome palettes. The overworld Poké Ball HUD stays hidden.
Removed the obsolete Followers EX/PokéPC pair after its sprite lookup failed
on 0.2.73. Wilds of Kanto 2.2.0 includes follower sprites, selection and
control modes independently; legacy follower settings can migrate there.
