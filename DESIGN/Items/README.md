# Items

Every consumable and key/puzzle item gets its own Markdown document, split into two subfolders:

- **[`Consumables/`](Consumables/README.md)** — health, ammo, and throwables. Generally
  stackable/countable, not tied to a single narrative instance.
- **[`Key_Items/`](Key_Items/README.md)** — keys, tools, and unique story-critical objects that
  gate a specific door/puzzle/reward. Each one is a distinct narrative object, even when its icon
  is shared with other key items (see "Reusable key/keycard icon templates" below).

> **Audited and restructured 2026-08-13** — see [`STORY_NOTES.md`](../STORY_NOTES.md) → "Items
> folder audit and Consumables/Key_Items split" for the full rationale, including which items were
> already established per-location before this pass and which were newly catalogued here for the
> first time.

## Reusable key/keycard icon templates

> Per the project owner: the physical-key and keycard sprites were **designed to be reused across
> multiple different key items**, not as unique art per named key. Don't treat a shared icon as
> evidence that two different keys are "the same item" — check each file's own Description/Story
> Placement, not just its icon.

- `spr_managerKey.png`, `spr_maintenanceKey.png`, and `spr_graveyardKey.png` (all in
  `Key_Items/`) are three interchangeable **generic physical-key icons** — despite their filenames,
  none of them is uniquely tied to one specific key (e.g. `spr_managerKey.png` isn't only used for
  the Manager's Key; it's also reused for the Armory Key). Which of the three gets used for which
  key item is an arbitrary/cosmetic assignment, not a canon fact.
- `spr_keycard.png` is the generic **keycard icon**, reusable for the Bollard Override Keycard now
  and for any future keycard item in a later district.
- Items with no real sprite yet (Gate Crank Handle, Bolt Cutters, Pocketknife, Authority Crest)
  have an AI-generated icon instead, per the convention below — these are placeholders, not
  reused-template art, since they're visually distinct one-of-a-kind objects.

## Convention: concept art for items

> Locked 2026-08-13 — see [`../README.md`](../README.md) rule 16 and
> [`Weapons/README.md`](../Weapons/README.md) → "Convention: concept art for weapons" for the full
> icon-style rationale (small, clean, flat-shaded pixel-art inventory icon, isolated on a plain
> dark background — not a painterly illustration). Items use the exact same style as weapons.

- **Filename:** `Assets/Reference/item_<name>_concept.png`, lowercase with underscores, for
  AI-generated icons. Real uploaded sprites stay directly alongside their `.md` file in
  `Consumables/` or `Key_Items/` as `spr_<name>.png`/`.gif` — don't move or rename those, and check
  each item's current status before generating a competing AI icon.
- **Base the prompt strictly on the item's own Description/Effects** — don't invent new
  canon-affecting details in the image prompt alone.
- **Embed it directly in the item's own file** near the top, then log it in the relevant
  subfolder's `README.md` file list.
