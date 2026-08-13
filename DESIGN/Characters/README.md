# Characters

Each significant recurring character gets its own Markdown document in this folder.

Do not create one file for every random background NPC.

A character document may contain:

- Role
- Background
- Appearance
- Personality
- Relationships
- Story arc
- Important scenes
- Dialogue characteristics
- Established facts
- Unresolved ideas

## Current files (Chapter 1 — Ravenwood Hotel)

- [`Jim_Mercer.md`](Jim_Mercer.md) — protagonist
- [`Sarah_Mercer.md`](Sarah_Mercer.md)
- [`Earl_Whitaker.md`](Earl_Whitaker.md)
- [`Cindy_Sweets.md`](Cindy_Sweets.md)
- [`Maria_Dalton.md`](Maria_Dalton.md)
- [`Richard_Dalton.md`](Richard_Dalton.md)
- [`Janeth_Caldwell.md`](Janeth_Caldwell.md)
- [`Dale_Pruitt.md`](Dale_Pruitt.md)
- [`Gerta.md`](Gerta.md) — added once her death scene (killed by The Maw) was approved; see
  [`Creatures/The_Maw.md`](../Creatures/The_Maw.md) and [`Scripts/Chapter_1_One_Night_Only.md`](../Scripts/Chapter_1_One_Night_Only.md), Scene 33.
- [`Fennimore.md`](Fennimore.md) — hotel security guard, never seen alive; established through his
  locker, his body/note in the courtyard, and his reanimated Shambler fight — see
  [`Scripts/Chapter_1_One_Night_Only.md`](../Scripts/Chapter_1_One_Night_Only.md), Scenes 37, 42, and 44.

## Current files (Chapter 2 — Ravenwood / Southwest District)

- [`Ruth_Calloway.md`](Ruth_Calloway.md) — Ravenwood PD desk sergeant; the Police Station's Tier 2
  conditional survivor — see [`Scripts/Chapter_2_Ravenwood.md`](../Scripts/Chapter_2_Ravenwood.md),
  Scene 26.
- [`Eli_Reyes.md`](Eli_Reyes.md) — Ravenwood PD's K-9 unit handler, never seen alive; found dead in
  the station's K-9 Unit Room, killed by his own K-9 partners — see
  [`Scripts/Chapter_2_Ravenwood.md`](../Scripts/Chapter_2_Ravenwood.md), Scenes 26–28.

Characters for the remaining four districts (Hospital, Academy, Refinery, Monastery) will be added
once those are written — see [`STORY_NOTES.md`](../STORY_NOTES.md).

## Convention: reference portraits for named characters

The project owner began uploading pixel-art reference portraits (2026-08-13) for the Chapter 1
cast, in the visual style the actual game will use. Generating a matching portrait for every named
character — existing and future — is now standard practice, not a one-off. Guidelines:

- **Filename:** `spr_<firstname>_portrait.png`, lowercase, matching the uploaded convention (e.g.
  `spr_maria_portrait.png`). For characters known only by surname (e.g. Fennimore), use the
  surname instead. Add a distinguishing suffix for variant states (`spr_cindy_robe_portrait.png`)
  the same way the uploaded set already does.
- **Style:** pixel art, bust/chest-up, roughly 3/4 turned pose, soft cel-shaded pixel shading, a
  plain light/neutral background — matching the already-uploaded portraits exactly. When
  generating a new one, pass an existing portrait as a reference image so the art style, canvas
  proportions, and shading approach stay consistent across the whole cast rather than drifting
  character to character.
- **Base the prompt strictly on what's already written** in the character's own Appearance section
  (and Personality, for expression/bearing) — don't invent new canon-affecting physical details in
  the image prompt alone. If nothing is written yet (as with several minor characters), keep new
  details generic/unremarkable rather than specific, and note in the file that the appearance was
  loosely interpreted for the portrait rather than independently established.
- **Characters who are "never seen alive on-screen"** (e.g. Fennimore, Corporal Eli Reyes) can
  still get a reference portrait — it's a design/continuity tool for the team, not an in-game
  asset, and doesn't contradict the choice to keep them off-screen while alive in the actual script.
- **Embed it directly in the character's own file**, same placement/caption convention already in
  use (see any existing character file), and log it in this README's file list above.
- This mirrors the concept-art convention already documented in
  [`Assets/README.md`](../Assets/README.md) for enemies/bosses — same spirit, applied to named
  characters instead.

**Portrait status (2026-08-13):** every currently-written named character has a reference
portrait — Sarah, Jim, Earl, Cindy (two states), Maria, Janeth, and Gerta were uploaded directly by
the project owner; Richard Dalton, Officer Dale Pruitt, Sergeant Ruth Calloway, Corporal Eli Reyes,
and Fennimore were AI-generated to match, following the convention above. Any newly-written
character from this point forward should get one as part of finishing their character file, not as
a separate follow-up pass.
