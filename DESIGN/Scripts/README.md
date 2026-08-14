# Scripts

Programmer/implementation-ready, **scene-by-scene** game scripts — the level of detail a
programmer would need to actually build a chapter: full dialogue, full action/description text,
and explicit interaction prompts, in play order.

This is a different level of detail than `Locations/`, `Characters/`, or `Creatures/`:

- **`Locations/*.md`** — structured design reference (purpose, rooms, items, puzzles, bosses as
  organized lists/summaries).
- **`Scripts/*.md`** — the actual scene-by-scene script that plays out in that location, written
  like a shooting script: scene number, slugline, prose description, dialogue.

Scenes are numbered sequentially within each chapter (**Scene 1, Scene 2, ...**), restarting at
Scene 1 for each new chapter file — not "Tabs," per an explicit instruction from the project owner
early on, since earlier source material used a confusing dual "Tab"/"Scene" numbering scheme.

## Current files

- [`Chapter_1_One_Night_Only.md`](Chapter_1_One_Night_Only.md) — the Ravenwood Hotel, in full (45 scenes). Locked.
- [`Chapter_2_Ravenwood.md`](Chapter_2_Ravenwood.md) — the street crossing, Memorial Park, the Downtown
  introduction, and the Southwest District/Police Station in full (45 scenes, including its optional
  Vanguard sub-plot).
- [`Chapter_2_Hospital.md`](Chapter_2_Hospital.md) — the Northeast District/St. Dymphna Hospital in
  full (17 scenes), kept as its own file rather than appended to `Chapter_2_Ravenwood.md`, per that
  file's already-large size — restarts its own Scene 1 count.

The three remaining districts (Academy, Foundry, Monastery) each have a full location-design file
in [`Locations/`](../Locations/) but no `Scripts/` entry yet — planned as the same kind of
standalone per-district file as `Chapter_2_Hospital.md`, per the project owner's request to script
each district in turn (see [`STORY_NOTES.md`](../STORY_NOTES.md) for the Direction Log).

Chapter 3 ("What Was Hidden") and the Epilogue ("One More Night") are outlined in [`CANON.md`](../CANON.md) and
[`MASTER_STORY.md`](../MASTER_STORY.md) but have no script content yet.
