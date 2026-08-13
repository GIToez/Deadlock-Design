# Weapons

Each weapon gets its own Markdown document in this folder. Source material: **[`Deadlock Weapons
and Items.docx`](../Deadlock%20Weapons%20and%20Items.docx)**, uploaded by the project owner
(2026-08-13) and transcribed here in full — see [`STORY_NOTES.md`](../STORY_NOTES.md) → "Weapons
and Items document — audit and folder buildout" for the complete audit, including cross-references
found against already-scripted weapons and open questions about where the not-yet-placed weapons
belong.

A weapon document contains:

- **Description** — the doc's own flavor text, transcribed verbatim.
- **Stats** — the doc's own numeric stat block, transcribed verbatim (see "Stat Glossary" below).
- **Concept art**.
- **Story Placement** — where/how the weapon fits (or might fit) into the currently-scripted story,
  cross-referenced against `Locations/`, `Characters/`, and `Scripts/`. Flagged as a proposal where
  no scripted placement exists yet.

## Stat Glossary

Transcribed verbatim from the source document's header notes — applies to every weapon's Stats
block below:

| Field | Meaning |
|---|---|
| **Damage** | Bullet damage (or, for melee/explosives, hit/tick damage) |
| **Fire Rate** | Seconds per shot |
| **Bullet Speed** | Travel speed |
| **Handling** | Ready/aim time, in seconds. **Lower = faster, higher = slower** — matters for animation timing and responsiveness |
| **Mag Size** | Ammo capacity. **-1 indicates infinite** |
| **Scoped** | Whether the weapon uses the scope camera system |
| **Recoil** | Angular spread in degrees (not the same as shotgun pellet spread). 0° = perfect accuracy, laser-straight; 1–3° = very accurate; 4–8° = moderate spread; 9–15° = heavy spread; 16°+ = extreme spread |
| **Noise lvl** | Sound radius, in pixels |
| **Sight Range** | Camera expansion, in pixels, while aiming down sights. 0 = no change; higher = farther view distance |

## Current files

**Standard Firearms:**

- [`Sentinel_9_Service_Pistol.md`](Sentinel_9_Service_Pistol.md) — RPD-issue sidearm; the game's
  first firearm (Chapter 1).
- [`Ranger_870_Pump_Shotgun.md`](Ranger_870_Pump_Shotgun.md) — civilian pump shotgun; the game's
  second firearm (Chapter 2, Police Station armory).
- [`Vanguard_M15_AR_Platform.md`](Vanguard_M15_AR_Platform.md) — Vanguard-modified semi-auto rifle.
- [`Ironback_357_Heavy_Revolver.md`](Ironback_357_Heavy_Revolver.md) — six-shot heavy revolver.
- [`Steelstorm_M60_LMG.md`](Steelstorm_M60_LMG.md) — belt-fed light machine gun, salvaged from a
  Steelgate factory security cache — plausibly placed in the not-yet-written Refinery district.
- [`Longview_308_Sniper_Rifle.md`](Longview_308_Sniper_Rifle.md) — bolt-action long-range rifle.

**Melee:**

- [`Roadwrecker_Baseball_Bat.md`](Roadwrecker_Baseball_Bat.md) — Jim's first weapon, grabbed from
  wrecked lobby furniture in Chapter 1.
- [`Cleaverborn_Survival_Sword.md`](Cleaverborn_Survival_Sword.md) — a cut-down machete/sword.

**Vanguard Experimental Prototype Set:**

- [`Thunderlance_Railgun.md`](Thunderlance_Railgun.md) — anti-Titan electromagnetic railgun
  prototype.
- [`CRN9_Decimator_Beam.md`](CRN9_Decimator_Beam.md) — unstable prototype energy beam projector.

**Heavy Weapon:**

- [`Titanbreaker_RLR7_Rocket_Launcher.md`](Titanbreaker_RLR7_Rocket_Launcher.md) — single-shot
  anti-bio-weapon rocket launcher.

Only the Baseball Bat and the two shown firearms above (Sentinel-9, Ranger 870) currently have a
confirmed placement in scripted content; the rest are documented per the source material but not
yet placed in a specific chapter/district — see each file's "Story Placement" section and
[`STORY_NOTES.md`](../STORY_NOTES.md) for the full list of open questions.

## Convention: concept art for weapons

> Locked 2026-08-13, alongside the folder's creation — see [`../README.md`](../README.md) rule 16.
> Every weapon gets a concept render as part of finishing its writeup, same standing rule as rooms,
> creatures, and characters.
>
> **Style corrected same day, before any weapon renders were generated:** the project owner
> uploaded eight actual in-game item-icon sprites as a style reference (inline in chat only — see
> [`STORY_NOTES.md`](../STORY_NOTES.md) → "Weapons and Items document — audit and folder buildout"
> for the full description, since they couldn't be saved into this repo directly). These are small,
> clean, flat-shaded pixel-art **inventory icons** — closer to the existing
> [`Assets/Reference/vern_terminal_icon.gif`](../Assets/Reference/vern_terminal_icon.gif) than to
> the painterly digital-concept-art style used for rooms/creatures. **Weapons and items use the
> icon style below, not the creature-concept-art painterly style.**

- **Filename:** `Reference/weapon_<name>_concept.png`, lowercase with underscores, matching the
  weapon's own filename (e.g. `Sentinel_9_Service_Pistol.md` →
  `weapon_sentinel_9_service_pistol_concept.png`).
- **Style:** a small, clean, flat-shaded pixel-art inventory icon — a simple, mostly-monochrome
  silhouette for firearms/melee weapons (dark gunmetal/black, minimal shading, a slight 3/4 angled
  view as if laid out in an inventory grid slot), matching the uploaded reference icons' scale and
  simplicity. **Not** a detailed painterly illustration, not a full scene, no background props — an
  isolated item on a plain dark background, the same convention as `vern_terminal_icon.gif`.
- **Base the prompt strictly on the weapon's own Description and Stats** (visible action type,
  material, wear/condition implied by its flavor text) — don't invent new canon-affecting details
  (e.g. a specific manufacturer logo) in the image prompt alone.
- **Embed it directly in the weapon's own file** near the top, with a one-line caption, then add it
  to this README's file list above.
