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
>
> **Convention, locked 2026-08-14:** every scene with a matching room-concept image in its
> `Locations/` file embeds that same image directly, right after the scene header — see
> [`Assets/README.md`](../Assets/README.md) → "Concept art now also embedded directly in
> `Scripts/` files." Applied to all five Chapter 2 district scripts. The image caption line
> ("AI-generated room concept, for visual reference — see `Locations/...`") was dropped during each
> district's puzzle-mechanic rewrite, per the same declutter direction that trimmed the stacked
> "Revision note" blockquotes in the `Locations/` files themselves — the image speaks for itself;
> a one-line pointer back to the `Locations/` file isn't needed on every single scene.

## Current files

- [`Chapter_1_One_Night_Only.md`](Chapter_1_One_Night_Only.md) — the Ravenwood Hotel, in full (45 scenes). Locked.
- [`Chapter_2_Ravenwood.md`](Chapter_2_Ravenwood.md) — the street crossing, Memorial Park, and the
  Downtown introduction (23 scenes, including the Ravenwood Pharmacy and Riverside Apartments) —
  the shared entry point before Jim splits off into any of the five open-order districts.
- [`Chapter_2_Police_Station.md`](Chapter_2_Police_Station.md) — the Southwest District/Police
  Station in full (24 scenes), including its optional Vanguard sub-plot. **Rewritten 2026-08-14**
  to the Lockdown Puzzle mechanic (see [`CANON.md`](../CANON.md) → "Five Puzzle Philosophies").
- [`Chapter_2_Hospital.md`](Chapter_2_Hospital.md) — the Northeast District/St. Dymphna Hospital in
  full (19 scenes). **Rewritten 2026-08-14** to the Quarantine Puzzle mechanic.
- [`Chapter_2_Foundry.md`](Chapter_2_Foundry.md) — the Northwest District/Steelgate Refinery in
  full (19 scenes). **Rewritten 2026-08-14** to the Casting Puzzle mechanic — also fixes an
  internal contradiction where the Industry Crest was previously described in two places at once
  (the seized mold and the Founder's Boardroom's display case, now empty).
- [`Chapter_2_Academy.md`](Chapter_2_Academy.md) — the Southeast District/Worthy Academy in full
  (18 scenes). **Rewritten 2026-08-14** to the Archive Puzzle mechanic, including
  [The Matron](../Creatures/The_Matron.md) as the district's new boss.
- [`Chapter_2_Monastery.md`](Chapter_2_Monastery.md) — the North District/Our Lady of Solace
  Monastery in full (17 scenes). **Written from scratch 2026-08-14** directly against the Bell
  Tower Puzzle mechanic, including [The Penitent](../Creatures/The_Penitent.md) as the district's
  boss; the Sealed Passage / Old Caves is self-contained and reachable in the same visit as the
  Faith Crest, with no dependency on any other district. This is the fifth and final district
  script — **all five Chapter 2 main locations now have a full scene-by-scene script matching their
  locked puzzle mechanic.**

The dialogue/pacing pass (Jim's over-narration trim, deliberate messiness in crossovers, the
per-district storytelling-material table) and the `Items/Key_Items/` audit are both complete as of
2026-08-14 — see [`STORY_NOTES.md`](../STORY_NOTES.md) for the full history. Remaining polish is
now at the level of individual lines, tracked in [`STORY_NOTES.md`](../STORY_NOTES.md) as it comes
up, not as a standing to-do here.

Chapter 3 ("What Was Hidden") and the Epilogue ("One More Night") are outlined in [`CANON.md`](../CANON.md) and
[`MASTER_STORY.md`](../MASTER_STORY.md) but have no script content yet.
