# Items

Each consumable/utility item gets its own Markdown document in this folder. Source material for
the current files: **[`Deadlock Weapons and Items.docx`](../Deadlock%20Weapons%20and%20Items.docx)**,
uploaded by the project owner (2026-08-13) — see [`STORY_NOTES.md`](../STORY_NOTES.md) → "Weapons
and Items document — audit and folder buildout" for the full audit.

An item document contains:

- **Description** — the doc's own flavor text, transcribed verbatim.
- **Effects** — the doc's own numeric effect block, transcribed verbatim (see "Effect Glossary"
  below).
- **Concept art**.
- **Story Placement** — where/how the item fits (or might fit) into the currently-scripted story.
  Flagged as a proposal where no scripted placement exists yet.

> **Scope note:** this folder is for the general-purpose consumable/utility items catalog (the
> source document only covers throwables so far: Molotov Cocktail, Pipe Bomb). It does **not**
> replace or migrate the location-specific key items already documented per-location (the Medkit,
> screwdriver, bolt cutters, Gate Crank Handle, Handgun Ammunition, etc. — see each `Locations/`
> file's own "Key Items" section) — those stay where they are unless a future decision consolidates
> them here too.

## Effect Glossary

Transcribed verbatim from the source document, matching the fields actually used for throwables:

| Field | Meaning |
|---|---|
| **Damage** | Direct or damage-over-time hit amount (see each item's own notation) |
| **Throw Range** | Maximum throw distance, in pixels |
| **Radius** | Effect/blast radius, in pixels |
| **Use Time** | Time to prime/throw, in seconds |
| **Noise lvl** | Sound radius, in pixels |
| **Special** | Any unique behavior beyond raw damage/radius |

## Current files

**Consumables Set (Throwables):**

- [`Molotov_Cocktail.md`](Molotov_Cocktail.md) — homemade incendiary throwable; area-denial fire.
- [`Pipe_Bomb.md`](Pipe_Bomb.md) — improvised shrapnel explosive; high burst damage.

Neither throwable currently has a confirmed placement in scripted content — see each file's "Story
Placement" section and [`STORY_NOTES.md`](../STORY_NOTES.md) for open questions.

## Convention: concept art for items

> Locked 2026-08-13, alongside the folder's creation — see [`../README.md`](../README.md) rule 16.
> Every item gets a concept render as part of finishing its writeup, same standing rule as rooms,
> creatures, characters, and weapons.
>
> **Style corrected same day, before any item renders were generated** — see
> [`Weapons/README.md`](../Weapons/README.md) → "Convention: concept art for weapons" for the full
> rationale (uploaded in-game icon references, described in
> [`STORY_NOTES.md`](../STORY_NOTES.md)). Items use the same small icon style as weapons, not a
> painterly illustration.

- **Filename:** `Reference/item_<name>_concept.png`, lowercase with underscores, matching the
  item's own filename (e.g. `Molotov_Cocktail.md` → `item_molotov_cocktail_concept.png`).
- **Style:** a small, clean, flat-shaded pixel-art inventory icon, isolated against a plain dark
  background — consumables can use more color than weapons (the uploaded references show a
  reddish-orange round consumable icon and a tan/khaki pouch icon among the mostly-monochrome
  weapon icons) but should stay just as simple/flat — same convention as
  [`Weapons/README.md`](../Weapons/README.md) → "Convention: concept art for weapons."
- **Base the prompt strictly on the item's own Description and Effects** — don't invent new
  canon-affecting details in the image prompt alone.
- **Embed it directly in the item's own file** near the top, with a one-line caption, then add it
  to this README's file list above.
