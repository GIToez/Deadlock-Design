# Scripts

Programmer/implementation-ready, **scene-by-scene** game scripts — the level of detail a
programmer would need to actually build a chapter: full dialogue, full action/description text,
and explicit interaction prompts, in play order.

This is a different level of detail than `Locations/`, `Characters/`, or `Creatures/`:

- **`Locations/*.md`** — structured design reference (purpose, rooms, items, puzzles, bosses as
  organized lists/summaries).
- **`Scripts/*.md`** — the actual scene-by-scene script that plays out in that location, written
  like a shooting script: scene number, slugline, prose description, dialogue.

Scenes are numbered sequentially within each chapter/district file (**Scene 1, Scene 2, ...**),
restarting at Scene 1 for each new file — not "Tabs," per an explicit instruction from the project
owner early on, since earlier source material used a confusing dual "Tab"/"Scene" numbering scheme.

> **Convention, locked 2026-08-13:** each Chapter 2 district gets its own standalone
> `Chapter_2_<District>.md` file, rather than one continuously growing chapter file. Per the
> project owner ("we should split each district into its own file to make it easier"),
> `Chapter_2_Ravenwood.md` originally continued straight into the Police Station as Scenes 22–45;
> that content has been split out into [`Chapter_2_Police_Station.md`](Chapter_2_Police_Station.md)
> (renumbered there as Scenes 1–24) — see [`STORY_NOTES.md`](../STORY_NOTES.md) for the full
> rationale and a renumbering map, in case any older note still cites a pre-split scene number.
> `Chapter_2_Ravenwood.md` itself now covers only the shared Downtown/Memorial Park content every
> district route passes through first.

## Current files

- [`Chapter_1_One_Night_Only.md`](Chapter_1_One_Night_Only.md) — the Ravenwood Hotel, in full (45 scenes). Locked.
- [`Chapter_2_Ravenwood.md`](Chapter_2_Ravenwood.md) — the street crossing, Memorial Park, and the
  Downtown introduction (21 scenes) — the shared entry point before Jim splits off into any of the
  five open-order districts.
- [`Chapter_2_Police_Station.md`](Chapter_2_Police_Station.md) — the Southwest District/Police
  Station in full (24 scenes), including its optional Vanguard sub-plot.
- [`Chapter_2_Hospital.md`](Chapter_2_Hospital.md) — the Northeast District/St. Dymphna Hospital in
  full (17 scenes).
- [`Chapter_2_Foundry.md`](Chapter_2_Foundry.md) — the Northwest District/Steelgate Refinery in
  full (17 scenes).

The two remaining districts (Academy, Monastery) each have a full location-design file in
[`Locations/`](../Locations/) but no `Scripts/` entry yet — planned as the same kind of standalone
per-district file, per the project owner's request to script each district in turn (see
[`STORY_NOTES.md`](../STORY_NOTES.md) for the Direction Log).

Chapter 3 ("What Was Hidden") and the Epilogue ("One More Night") are outlined in [`CANON.md`](../CANON.md) and
[`MASTER_STORY.md`](../MASTER_STORY.md) but have no script content yet.
