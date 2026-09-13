# Yellow Online

A version-pinned Gen1Recomp cart for **Pokemon Yellow**: multiplayer Kanto at
the core, wrapped in the modern QoL suite and the community's best world, quest
and art mods. **58 mods, sealed** - two people running this cart run the exact
same game.

## Install

Download the `yellow_online-<version>.g1rcart` asset from the
[latest release](https://github.com/notquiteog/yellow-online/releases/latest)
and import it from the launcher's **Custom Carts** panel (or drop it into your
save directory's `carts/` folder). The cart installs its pinned mods itself,
each fetched at the exact build in `cart.json` and verified against its
published `sha256sums.txt`.

This bundle ships no code. It is a pin list - every mod on it is published
separately and fetched at its exact build.

## The core

[Gen1Online](https://github.com/notquiteog/Gen1Online) is pinned at
**0.3.0**, the last Gen-1-era build - the newer 0.4/0.5 ("Gen1Online++") line
is Crystal-only. The pin points at a mirror: upstream tags this exact archive
`v0.3.1` while the mod's own manifest inside it says `0.3.0`, and a sealed
cart verifies pin against installed version, so the mislabel made v1.0.0 of
this cart refuse to enforce (which disabled every mod, Battle Art Voxel
included). The mirror re-publishes that archive under the version the mod declares,
with one packaging fix: upstream's manifest never declares the `compute`
permission its `love.thread` netcode needs (the sandbox errors without it),
so the mirror adds it. Multiplayer and the GTS use the mod's own server
exactly as upstream ships it.

## What's on it


### Core & multiplayer

| mod | build | what it does here |
| --- | --- | --- |
| [gen1online](https://github.com/gamecorner-033/Gen1Online) | 0.3.1 | the core: real-time overworld co-op, facing PVP link battles, vanilla link trades, chat and a 24/7 GTS |
| [PokePCFollowers_VoxelMerge](https://github.com/notquiteog/PokePCFollowers_VoxelMerge) | 0.5.1 | all 151 Gen 1 followers walking behind you, voxel-ready (Red/Blue/Yellow) |
| [overworld_wild_spawns](https://github.com/YoDrehDenSwagAuf/overworld-spawn-mod) | 2.1.9 | wild Pokemon visible roaming the grass, faced and battled in the field |
| [FOLLOWERS_EX](https://github.com/masterwebx/gen1recomp-followers-ex) | 1.0.19 | follower modes; on Yellow, Pikachu stays in slot 1 as the talkable companion |


### World, movement & sky

| mod | build | what it does here |
| --- | --- | --- |
| [BATTLE_ART_VOXEL_FORK](https://github.com/absol89/DramaticShapeVoxelMod) | 1.10.8 | the overworld drawn as a 3D diorama, with battles staged on its ground over the shoulder |
| [DRAMATIC_SKY_RIDE](https://github.com/burgerslayer7/dramatic-sky-ride) | 0.2.18 | controllable flight, ground rides and visible Surf mounts |
| [wild_skies](https://github.com/shanehudson-gen1recomp-mods/wild_skies) | 1.12.0 | flocks of local flying Pokemon crossing the sky and perching on rooftops |
| [kanto_life](https://github.com/jtfresh90/Kanto-Life-Mod) | 0.8.34 | daily-life dialogue and naming for Kanto's NPCs |
| [modern_kanto](https://github.com/MadeinTaly/gen1recomp-modern-kanto) | 0.3.0 | the physical/special split, decided by type |
| [npc_bubbles](https://github.com/ddagent/gen1recomp-npc-bubbles) | 2.3.12 | speech bubbles over NPCs saying what they would actually say |


### Quality of life (FAFF0x suite)

| mod | build | what it does here |
| --- | --- | --- |
| [quest_system](https://github.com/notquiteog/quest_system) | 1.0.5 | QUESTS menu: active and completed quest log with progress bars |
| [kanto_achievements](https://github.com/notquiteog/kanto_achievements) | 1.0.6 | 100 achievements with tabs, search and categories |
| [pokedex_plus](https://github.com/notquiteog/pokedex_plus) | 1.3.4 | Pokedex with base stats, habitat, evolutions and level-up moves |
| [area_dexnav](https://github.com/notquiteog/area_dexnav) | 1.0.0 | SELECT starts an encounter with an uncaught Pokemon from the local table |
| [modern_bag](https://github.com/notquiteog/modern_bag) | 1.6.0 | pocketed modern Bag: favorites, pins, unlimited capacity, search |
| [modern_battle_ui](https://github.com/notquiteog/modern_battle_ui) | 1.4.6 | redesigned battle HUD, FIGHT menu and in-battle party/bag screens |
| [catch_helper](https://github.com/notquiteog/catch_helper) | 1.4.0 | live catch chances and an owned-species ball marker |
| [move_inspector](https://github.com/notquiteog/move_inspector) | 1.0.0 | type/PP/power/accuracy/effectiveness shown in battle |
| [move_learn_stats](https://github.com/notquiteog/move_learn_stats) | 1.0.2 | forget-vs-learn comparison when replacing a move |
| [moves_manager](https://github.com/notquiteog/moves_manager) | 1.0.1 | per-Pokemon MOVES pages and move-memory replacement |
| [dv_ev_editor](https://github.com/notquiteog/dv_ev_editor) | 1.1.0 | edit DVs and stat EXP from the party menu |
| [advanced_box_system](https://github.com/notquiteog/advanced_box_system) | 1.1.0 | fast PC box navigation, direct swaps and quick swap |
| [exp_share_modes](https://github.com/notquiteog/exp_share_modes) | 1.0.0 | Off / Classic Even Split / Modern Progressive EXP distribution |
| [hm_anywhere](https://github.com/notquiteog/hm_anywhere) | 1.2.0 | use owned HMs straight from the Bag, badges still required |
| [item_shortcut](https://github.com/notquiteog/item_shortcut) | 1.4.0 | overworld item hotkeys with five assignable slots |
| [repel_reuse_prompt](https://github.com/notquiteog/repel_reuse_prompt) | 1.0.0 | prompt to re-apply a Repel when one expires |
| [reusable_machines](https://github.com/notquiteog/reusable_machines) | 1.0.1 | TMs are not consumed and HM moves can be forgotten |
| [trade_evolution_fix](https://github.com/notquiteog/trade_evolution_fix) | 1.0.0 | trade evolutions become level-40 evolutions |
| [nickname_changer](https://github.com/notquiteog/nickname_changer) | 1.0.0 | rename Pokemon from the party menu |


### Extras from the community

| mod | build | what it does here |
| --- | --- | --- |
| [ACCESS_PC_ANYWHERE](https://github.com/masterwebx/gen1recomp-access-pc-anywhere) | 1.0.1 | open the PC storage system from anywhere |
| [RUN_MODE](https://github.com/masterwebx/gen1recomp-run-mode) | 1.2.0 | hold a button to run |
| [trainer_rematch](https://github.com/ShaneMcGovernIE/trainer_rematch) | 0.5.4 | rematch trainers and gym leaders |
| [critical_capture](https://github.com/ShaneMcGovernIE/critical_capture) | 0.1.1 | Gen 5 critical captures, odds scaled to 151 species |
| [mew_under_the_truck](https://github.com/Maaggel/mew-under-the-truck) | 0.9.0 | the truck. the mew. behind the Rainbow Badge |
| [bookers_heaven](https://github.com/bryanthaboi/bookers_heaven) | 1.1.0 | welcome to booker's heaven |
| [new_game_plus](https://github.com/notquiteog/new_game_plus) | 1.0.0 | carry into a new run |


### Quests (FAFF0x)

| mod | build | what it does here |
| --- | --- | --- |
| [echoes_beyond_the_fog](https://github.com/notquiteog/echoes_beyond_the_fog) | 2.2.2 | Cape Signal Observatory and the Fogbound Caverns (after Bill, Soul Badge) |
| [crystal_onix](https://github.com/notquiteog/crystal_onix) | 1.0.8 | the Crystal Onix hunt |
| [eevee_three_stones](https://github.com/notquiteog/eevee_three_stones) | 1.0.2 | the Three-Stone Covenant: three trials and an Eevee reward |
| [mew_mirage](https://github.com/notquiteog/mew_mirage) | 1.0.1 | retrace Project Mew across Kanto to summon Mew (after Earth Badge) |
| [poachers_in_the_safari_zone](https://github.com/notquiteog/poachers_in_the_safari_zone) | 1.0.0 | run poachers out of the Safari Zone (after Soul Badge) |
| [rocket_gym_ambushes](https://github.com/notquiteog/rocket_gym_ambushes) | 1.0.1 | Team Rocket ambushes inside gyms |
| [team_rocket_returns](https://github.com/notquiteog/team_rocket_returns) | 1.0.1 | Team Rocket strikes back across Kanto |
| [the_abandoned_cabin](https://github.com/notquiteog/the_abandoned_cabin) | 1.0.0 | strange lights in an abandoned cabin on Route 11 (after Thunder Badge) |
| [the_black_flower](https://github.com/notquiteog/the_black_flower) | 1.0.0 | a black flower drains Celadon's garden (after Rainbow Badge) |
| [the_empty_throne](https://github.com/notquiteog/the_empty_throne) | 1.0.2 | a new Rocket commander beneath Viridian Gym (after Earth Badge) |
| [the_sixth_bell](https://github.com/notquiteog/the_sixth_bell) | 1.1.4 | the sixth bell tolls in Lavender (after six Badges) |
| [the_stolen_fossil](https://github.com/notquiteog/the_stolen_fossil) | 1.0.1 | a stolen fossil trail leads to Mt. Moon (after Boulder Badge) |
| [whispers_beneath_cerulean](https://github.com/notquiteog/whispers_beneath_cerulean) | 1.0.1 | contaminated canals under Cerulean (after Cascade Badge) |


### Art & polish

| mod | build | what it does here |
| --- | --- | --- |
| [new_sprites](https://github.com/notquiteog/new_sprites) | 1.1.0 | modern battle sprites |
| [new_icons](https://github.com/notquiteog/new_icons) | 1.1.1 | new small party icons |
| [new_item_icons](https://github.com/notquiteog/new_item_icons) | 1.0.0 | 88 new item and TM/HM type icons |
| [unique_menu_icons](https://github.com/menyas/unique-menu-icons) | 1.5.0 | a unique party icon for every Gen 1 species |
| [gen1_modern_ui](https://github.com/ArmstrongThomas/gen1-modern-ui) | 0.9.2 | responsive UI presentation (retired upstream; still loads and runs) |
| [widescreen_battle_intro](https://github.com/ShaneMcGovernIE/gen1recomp-widescreen-battle-intro) | 1.6.0 | widescreen battle intros |
| [player_sprite_flip](https://github.com/eduardocalafell/gen1recomp-player-sprite-flip) | 0.1.0 | the player sprite faces the foe in battle |
| [quality_of_life](https://github.com/unxpected-uxp/pokemon-gen1-recomp-mod-qol) | 1.3.0 | later-generation options, each default OFF under OPTION |
| [modern_ui_icon_fix](https://github.com/notquiteog/modern_ui_icon_fix) | 1.2.3 | fixes for modern-UI icon presentation; loads last for the outermost say on icons |

## Load order

`cart.json`'s `load_order` is the order above, top to bottom: core first, art
last, and the wraps around the engine's sprite and battle hooks land in a
fixed order. It matters - e.g. Battle Art Voxel Fork and the sprite replacers
both touch the `pokemon.sprite` hook, and the one that loads last has the
outermost say, and the icon fix is deliberately the outermost of all.

## The seal

`seal` is `sealed`: the list is fixed, every pin runs, nothing can be added or
switched off, and the cart is locked to 1x speed. That is what makes it a
competitive bundle for link play.

## Compatibility calls

From the candidate list, these were left off and why:

- **ShaneMcGovernIE/exp_share** - same feature as the pinned FAFF0x
  `exp_share_modes`; two EXP distributors would fight over the same math.
- **ShaneMcGovernIE/useful-bag** - same feature as the pinned FAFF0x
  `modern_bag`; two bag rewrites replace the same screens.
- **eduardocalafell/gen1recomp-better-battle-ui** (the repo behind the
  `gen1recomp-better-battle-` link) - overlaps the pinned `modern_battle_ui`
  and `catch_helper` on the same battle HUD real estate.
- **1-Camp0-1/Kanto-Dynamic-Weather** - hard-depends on the original
  `DRAMATIC_SHAPE` 1.7.x, which the pinned `BATTLE_ART_VOXEL_FORK` declares a
  conflict. One or the other; the voxel fork won.

From the FAFF0x collection, the fair-play call for an online/GTS cart left off
`all_tm_shop`, `free_master_ball`, `free_rare_candy`, `guaranteed_catch` and
`summon` (economy and catch integrity), plus `performance_monitor` (a debug
tool). Everything else is on.

## Mirrors

The FAFF0x mods ship as zips inside
[FAFF0x/gen1recomp](https://github.com/FAFF0x/gen1recomp) with no releases, and
[gamecorner-033/PokePCFollowers](https://github.com/gamecorner-033/PokePCFollowers)
published no release - cartkit pins need a release and a `sha256sums.txt`. They
are mirrored byte-for-byte under [notquiteog](https://github.com/notquiteog?tab=repositories)
(release assets are the original archives, unmodified). All credit for those
mods belongs to their authors.

No mod here distributes ROMs, extracted game data, or Pokemon-copyrighted art,
audio or text. Everything shown at runtime comes from your own cartridge dump,
imported by the engine on your machine.
