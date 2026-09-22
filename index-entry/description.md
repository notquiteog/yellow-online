# Yellow Online

Multiplayer Kanto, sealed. Yellow Online pins **58 mods** into one cart for
**Pokemon Yellow**: RBY MMO at the core: shared overworld presence with on-the-spot trades
and PVP battles, parties, co-op 2v2, chat and friends - hosted from inside
the game, no dedicated server needed; the party follower and visible wild spawns in the grass;
the overworld drawn as a 3D diorama with battles staged on it; controllable
flight, rides and flocks crossing the sky; the FAFF0x modern suite (pocketed
bag, modern battle HUD, Pokedex Plus, quest log, achievements, HM anywhere,
EXP share modes); thirteen new quests from the FAFF0x collection; and the art
polish on top. The cart is locked to 1x and fully sealed, so link play is
fair: everyone runs the same builds of the same mods.

The core is RBY MMO 1.4.1 (host from the START menu; a dedicated hub is
optional).

## 1.2.0 — HD-2D worlds and interior dioramas

Pins Battle Art 1.21.0 from our fork, including upstream through 1.11.0.
Adds native-art scenery, reviewed building exteriors, shared render distance
and contextual boundary fill, plus framed interiors and warm lighting.
Requires Gen1Recomp 0.2.73+. Kanto Gear remains absent.
Replaces the upstream Battle Art 1.10.8 pin with our 1.21.0 fork. Yellow base, sealed policy and cartridge artwork are retained.

This is an incremental visual release, not complete Gamma Emerald parity.
Multiplayer doubles and FireRed companion ports remain unfinished.

Release preflight: Wild Skies 1.12.3 fixes generated sky cards under native
monochrome palettes. The overworld Poké Ball HUD stays hidden.
Removed the obsolete Followers EX/PokéPC pair after its sprite lookup failed
on 0.2.73. Wilds of Kanto 2.2.0 includes follower sprites, selection and
control modes independently; legacy follower settings can migrate there.

Final release validation (Gen1Recomp 0.2.73 Linux): all 56 exact pinned
versions loaded through the sealed-cart boot path; Oak's Lab rendered in
static, first-person and rotating third-person views, followed by Pallet Town
field return. Online release/hash validation passed. A forced Pidgey flyer
also rendered without the former virtual-card file failure. These checks
are not a full quest playthrough or Internet multiplayer test.
