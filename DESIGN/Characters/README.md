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
character — existing and future — is now standard practice, not a one-off.

**The correct pipeline (confirmed 2026-08-13) is a two-step process, using the project owner's own
tool and prompt, not a generic image generator:**

1. **Generate a clean "source" reference photo first**, using this exact prompt template (the
   project owner's own, used for the original uploads) with a semi-realistic style:
   > *"Waist-up character portrait, cropped from top of head to mid-torso, consistent framing.
   > Character centered in frame, slight 3/4 angle facing toward the right side of the screen. Eyes
   > looking toward the right edge of the image. Camera distance fixed, medium shot (not
   > close-up, not full body). Use the reference image for exact skin tone, hair color, clothing,
   > and overall color palette. Match colors exactly, do not desaturate or darken. Realistic human
   > proportions and facial structure, not stylized, not cartoon. Natural lighting with soft
   > shadows, no heavy contrast or color grading. Black background. Semi-realistic grounded style
   > with accurate colors and realistic detail."*

   Adapt only the character-specific details (age, hair, clothing) within that same structure.
2. **Run that photo through PixelLab's `create_image_pro` tool** (the MCP equivalent of PixelLab.ai's
   "Create Image (Pro)" web tool, confirmed by the project owner as what produced the original
   uploaded portraits) — same prompt template as step 1, `width`/`height` **256** (confirmed exact
   output size of the uploaded set), `no_background: true`, and the step-1 photo passed via
   `reference_images` with `usage: "exact character identity, skin tone, hair color, and clothing
   colors"`. This is what actually produces the matching pixel-art result — a generic image
   generator (not PixelLab) reliably fails to match the house style even with the same prompt.
   - **Reference image size/transmission is finicky:** the `reference_images` base64 payload
     truncates unpredictably above roughly 2–3 KB in practice. Resize the step-1 photo down to
     roughly 40–48px square with a reduced color palette (16–24 colors) before encoding — small
     enough to transmit reliably. This loses fine detail, so **compensate by making the text
     description explicit** about hair color/style, skin tone, and clothing (don't rely on the
     reference image alone to carry identity). If a result comes back clearly unrelated to the
     reference (a stock/generic person), don't treat that as final — retry once with a more
     explicit description; it resolved every case tried so far.
   - Prefer `reference_images` (JSON array with one labelled entry) over `style_image_base64`.
3. **Save the `create_image_pro` result** (256×256 PNG, matching the uploaded set's exact
   dimensions) as the character's `spr_<name>_portrait.png` and embed it as normal.

Other guidelines:

- **Filename:** `spr_<firstname>_portrait.png`, lowercase, matching the uploaded convention (e.g.
  `spr_maria_portrait.png`). For characters known only by surname (e.g. Fennimore), use the
  surname instead. Add a distinguishing suffix for variant states (`spr_cindy_robe_portrait.png`)
  the same way the uploaded set already does.
- **Base the prompt strictly on what's already written** in the character's own Appearance section
  (and Personality, for expression/bearing) — don't invent new canon-affecting physical details in
  the image prompt alone. If nothing is written yet (as with several minor characters), keep new
  details generic/unremarkable rather than specific, and note in the file that the appearance was
  interpreted for the portrait rather than independently established.
- **Characters who are "never seen alive on-screen"** (e.g. Fennimore, Corporal Eli Reyes) can
  still get a reference portrait — it's a design/continuity tool for the team, not an in-game
  asset, and doesn't contradict the choice to keep them off-screen while alive in the actual script.
- **Embed it directly in the character's own file**, same placement/caption convention already in
  use (see any existing character file), and log it in this README's file list above.
- This mirrors the concept-art convention already documented in
  [`Assets/README.md`](../Assets/README.md) for enemies/bosses, but for named characters the
  PixelLab pipeline above is what actually matches the house style — the concept-art convention's
  generic-image-generator approach is not a substitute for it.

**Portrait status (2026-08-13):** every currently-written named character has a reference
portrait, and all of them now go through the confirmed PixelLab pipeline above — Sarah, Jim, Earl,
Cindy (two states), Maria, Janeth, and Gerta were uploaded directly by the project owner (made with
the same pipeline on their end); Richard Dalton, Officer Dale Pruitt, Sergeant Ruth Calloway,
Corporal Eli Reyes, and Fennimore were generated to match (an earlier attempt at these five, using
a generic image generator instead of PixelLab, was replaced once the correct pipeline was
confirmed). Any newly-written character from this point forward should get one as part of
finishing their character file, using this same two-step process, not as a separate follow-up pass.
