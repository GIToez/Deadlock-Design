# Assets

Reference images, concept art, and gameplay screenshots/GIFs for Deadlock Protocol. These are
visual reference material, not story content — cross-link to them from the relevant
`Locations/`, `Characters/`, `Creatures/`, or `Scripts/` file with standard markdown image syntax:

```markdown
![Ravenwood Hotel Lobby — full layout reference](../Assets/Screenshots/ravenwood_hotel_lobby.png)
```

## Suggested organization

- **`Screenshots/`** — actual in-engine/gameplay captures (stills or GIFs). These are the most
  reliable source of truth for art style, camera framing, and what the player actually sees —
  more trustworthy than prose descriptions when the two disagree. If a screenshot contradicts
  something written elsewhere, flag it rather than silently rewriting the screenshot's intent.
- **`Reference/`** — concept art, mood boards, or AI-generated placeholder visuals used for
  discussion rather than as ground truth.
- **Directly alongside a character/creature/location file** is also fine and used in practice —
  e.g. `Characters/spr_cindy_jumpscare.gif` sits right next to `Characters/Cindy_Sweets.md` and is
  embedded directly in it. Use whichever placement makes more sense for a given asset; there's no
  requirement to funnel everything into this folder specifically.

## How to add a file

Cursor cloud agents can't save images pasted directly into chat to disk — only files pushed as
real commits to the branch (the same way `AI.json` and the story `.docx` were added) become
accessible here. Push new images/GIFs into `DESIGN/Assets/Screenshots/` or `DESIGN/Assets/Reference/`
directly (e.g. via the GitHub web UI), using a short, descriptive filename
(`cindy_jumpscare.gif`, `ravenwood_hotel_lobby_overview.png`).

## Current files

- **`Reference/founders_memorial_plaque_concept.png`** — AI-generated concept art for the
  Founders Memorial's medallion-plaque (Memorial Park, Chapter 2): the central pentagon "V" hub
  and the five wedge slots, two shown filled/glowing and three empty, for visual reference only —
  not a literal in-game screenshot. Referenced from
  [`CANON.md`](../CANON.md) and [`Locations/Memorial_Park.md`](../Locations/Memorial_Park.md).
- **`Reference/ashen_hound_concept.png`** — AI-generated concept art for the
  [Ashen Hound](../Creatures/Ashen_Hound.md) ("Diesel," the Police Station's K-9 Unit Room
  encounter, Chapter 2). Regenerated 2026-08-13 to match the encounter's move from the Municipal
  Garage into the station itself. Referenced from `Creatures/Ashen_Hound.md`.
- **`Screenshots/ravenwood_hotel_*.png` / `.webp`** (11 files, uploaded by the project owner,
  2026-08-13) — in-engine room mockups for the Ravenwood Hotel: the exterior/parking lot, the
  Manager's Office (including the VERN terminal exactly as described in `CANON.md`), Room 104
  (bedroom + bathroom), and the Dining Hall/Kitchen. These are the most reliable art-style
  reference in the whole project so far — real room mockups, not concept sketches. Renamed from
  generic upload filenames (`image-2.webp`, `file_0000...png`, etc.) to descriptive ones; all
  embedded directly in [`Locations/Ravenwood_Hotel.md`](../Locations/Ravenwood_Hotel.md) at their
  matching rooms, with any new details not already in the script flagged inline rather than
  silently written in as fact.
- **`Reference/zombie_conglomerate_dossier.png`, `zombie_conglomerate_closeup.png`,
  `zombie_conglomerate_roll_animation.gif`** (uploaded by the project owner, 2026-08-13) — concept
  art and an animation test for **the Zombie Conglomerate** (the "Zombie King"), a new roaming
  creature — see [`Creatures/Zombie_Conglomerate.md`](../Creatures/Zombie_Conglomerate.md) for the
  full writeup, including a locked-canon conflict in the dossier's own timeline that's flagged
  there rather than silently imported.
- **`Reference/vern_terminal_icon.gif`** (uploaded by the project owner, 2026-08-13) — a small
  pixel-art icon of the VERN terminal itself, consistent with its wall-mounted appearance in the
  Manager's Office screenshot above.
- **`Reference/police_station_bullpen_concept.png`, `police_station_chiefs_office_concept.png`,
  `police_station_k9_room_concept.png`, `police_station_old_main_hall_concept.png`** (AI-generated,
  2026-08-13) — the first batch of room concept art under the new convention below, covering the
  Police Station's most narratively significant rooms. Embedded in
  [`Locations/Police_Station.md`](../Locations/Police_Station.md). The Chief's Office concept
  invented an unprompted "CHIEF E. WHITAKER" nameplate (flagged, not canon); the first attempt at
  the Old Station House main hall rendered the wrong emblem shape and invented chief names and was
  regenerated.
- **`Reference/hotel_lobby_concept.png`, `hotel_room106_concept.png`, `hotel_courtyard_concept.png`,
  `hotel_red_room_concept.png`, `hotel_laundry_room_concept.png`,
  `hotel_housekeeping_closet_concept.png`, `hotel_main_bar_concept.png`,
  `hotel_utility_room_concept.png`, `hotel_security_office_concept.png`,
  `hotel_west_maintenance_room_concept.png`** (AI-generated, 2026-08-13) — the remaining
  Ravenwood Hotel rooms of real narrative weight that didn't already have a real in-engine
  screenshot: the Lobby, Room 106 (Cindy), the Hotel Courtyard, the Red Room (Della Marsh), the
  Laundry Room (Gerta's death), the Housekeeping Closet (Gate Crank Handle), the Main Bar, the
  Utility Room (screwdriver), the Courtyard Security Office, and the West Wing Maintenance Room
  (auxiliary fuse). All embedded in
  [`Locations/Ravenwood_Hotel.md`](../Locations/Ravenwood_Hotel.md) at their matching rooms. The
  Housekeeping Closet render invented a "305" door number that contradicts its canonical location
  (2F, between Rooms 114/116) — flagged there, not canon.
- **`Reference/police_station_lobby_concept.png`, `police_station_dispatch_concept.png`,
  `police_station_armory_concept.png`, `police_station_evidence_room_concept.png`,
  `police_station_fire_station_concept.png`, `police_station_municipal_garage_concept.png`,
  `police_station_courthouse_concept.png`, `police_station_break_room_concept.png`,
  `police_station_booking_concept.png`, `police_station_interview_room_concept.png`,
  `police_station_modern_cells_concept.png`, `police_station_old_cells_concept.png`**
  (AI-generated, 2026-08-13) — the remaining Police Station rooms, completing full room-concept
  coverage for the district: the Lobby, Records/Dispatch, the Armory, the Property & Evidence
  Room, the three secondary locations (Fire Station, Municipal Garage, City Courthouse), the
  Break Room, Booking & Processing, the Interview Room, the Modern Holding Cells, and the Old
  Holding Cells. All embedded in
  [`Locations/Police_Station.md`](../Locations/Police_Station.md) at their matching rooms. Three
  flagged generation errors: Records/Dispatch invented an unrelated "DET. HARRIS" nameplate, the
  Break Room labeled Corporal Reyes' locker "K. HARRISON" instead of "E. REYES," and the Municipal
  Garage's wall sign reads "CITY OF RAVENCROFT" instead of the locked city name Ravenwood — all
  non-canonical.
- **Room concept art style correction, take one — reverted (2026-08-13, same day).** First reading
  of project-owner feedback ("Make sure all room concepts follow the in game screenshots. Some
  don't.") wrongly concluded the real in-engine screenshots were a *flat, directly-overhead* style,
  and re-rendered `hotel_courtyard_concept.png`, `hotel_red_room_concept.png`, and all 16 Police
  Station room concepts as flat top-down. Corrected feedback ("2.5d room not flat, look at the
  uploaded screenshots. The older renders looked better than these new ones") confirmed the
  screenshots are actually **2.5D / isometric-leaning** (an elevated three-quarter angle that shows
  the fronts of furniture and walls, not a straight overhead view) — the *original* renders had this
  right, and the "fix" was itself the regression. Reverted all 18 files back to their pre-"fix"
  versions.
- **Room concept art style correction, take two (2026-08-13, same day).** Follow-up feedback ("Only
  like 2 maps didn't render right off the old") narrowed the actual problem to just two of the
  reverted files — `police_station_armory_concept.png` and `police_station_interview_room_concept.png`
  — which, on inspection, had rendered in a flat vector-cartoon style (thick black outlines, no
  pixel-art grain) unlike every other room concept's painterly 2.5D pixel-art look. Regenerated only
  those two, anchored to a known-good existing room concept plus a real Hotel screenshot, keeping the
  other 16 reverted files as-is. Net result: the three previously-fixed non-canonical details
  (Records/Dispatch's "DET. HARRIS," the Break Room locker name, and the Municipal Garage's
  "RAVENCROFT" sign) are back in their original flagged state, since those renders reverted along
  with everything else — see the original flagged notes in
  [`Locations/Police_Station.md`](../Locations/Police_Station.md).
- **`Reference/police_station_armory_concept.png`, `police_station_interview_room_concept.png`
  ("v4") (2026-08-13, take three).** The take-two regenerations still hadn't fixed the flat
  vector-cartoon look; regenerated a second time, anchored directly to a real Hotel screenshot and a
  known-good Police Station room concept — see
  [`STORY_NOTES.md`](../STORY_NOTES.md) "Room concept art style correction, take three."
- **Room concept art style correction, take four — attempted and reverted (2026-08-13).** Regenerated
  `police_station_modern_cells_concept.png`, `police_station_courthouse_concept.png`, and (never
  deployed) `hotel_red_room_concept_v2.png` to a strict flat-back-wall framing, matching the real
  screenshots' camera angle more literally. Rejected by the project owner ("Those r flat the old are
  better"); all three reverted/discarded. See
  [`STORY_NOTES.md`](../STORY_NOTES.md) "Room concept art style correction, take four" for the
  confirmed lesson: concept art's camera framing (including tilted/isometric corner views) doesn't
  need to exactly match the flatter in-engine screenshot framing, just the same painterly 2.5D
  pixel-art style. `hotel_lobby_concept.png` was also removed from this folder around the same time
  (2026-08-13) at the project owner's direction — the Lobby already has a real gameplay screenshot in
  the actual game (not yet pushed to this repo) and shouldn't be represented by an AI approximation;
  see [`Locations/Ravenwood_Hotel.md`](../Locations/Ravenwood_Hotel.md) for the TBD note.
- **`Reference/shambler_concept.png`, `the_caretaker_concept.png`, `della_marsh_concept.png`,
  `the_maw_concept.png`** (AI-generated, 2026-08-13) — creature concept art for the four remaining
  creature writeups that didn't have one yet, completing visual coverage for every creature in
  `Creatures/`. Moody digital concept-art painting style, per the convention below. Embedded in their
  matching `Creatures/` files. Two approximations flagged there rather than treated as canon: the
  Caretaker's render doesn't clearly show hotel-maintenance overalls or a distinctly off-color glowing
  eye.

Several other assets have been uploaded, placed directly alongside their character files instead:

- `Characters/spr_cindy_jumpscare.gif` — embedded in
  [`Characters/Cindy_Sweets.md`](../Characters/Cindy_Sweets.md).
- **Character reference portraits** — every named character now has one; see
  [`Characters/README.md`](../Characters/README.md) → "Convention: reference portraits for named
  characters" for the full file list, the confirmed two-step PixelLab generation pipeline, and
  status. Sarah, Cindy (two states), Earl, Gerta, Janeth, Maria, and Jim were uploaded directly by
  the project owner (two filenames corrected after upload — a stray space, and a generic name
  confirmed to be Jim); Richard Dalton, Officer Dale Pruitt, Sergeant Ruth Calloway, Corporal Eli
  Reyes, and Fennimore were generated (2026-08-13) to match, via PixelLab's `create_image_pro`
  tool once that was confirmed as the correct pipeline (an earlier attempt using a generic image
  generator was replaced).

## Convention: room concept art

> **This is now a permanent rule, not a one-off pass** (locked 2026-08-13 — see
> [`README.md`](../README.md) rule 16): every new scene/room gets a matching concept render as
> part of finishing it, going forward, not as a separate follow-up task.

The project owner's uploaded Hotel screenshots (`Screenshots/ravenwood_hotel_*`) are genuine
in-engine mockups and now the definitive visual-style reference for the whole project — a warm,
detailed, isometric-leaning 2.5D top-down pixel art style with a high density of readable props.
Generating a matching room concept for scenes/locations that don't have a real mockup yet is now
standard practice, to give the team a general sense of "how that room should look" ahead of actual
in-engine work. Guidelines:

- **Filename:** `Reference/<location>_<room>_concept.png`, lowercase with underscores (e.g.
  `police_station_bullpen_concept.png`).
- **Always pass at least one existing Hotel screenshot as a style reference** when generating —
  these are AI-generated approximations, not real game assets, so staying visually anchored to the
  one style reference we know is accurate matters more than for mood-board concept art (like the
  creature concept art convention below, which allows more painterly latitude).
- **Base the prompt strictly on what's already written** in the room's own scene text (props,
  layout, key items visible) — don't invent new canon-affecting layout details in the image prompt
  alone. If the generated image suggests something worth keeping (an item placement, a detail),
  fold it back into the script/location file rather than leaving it only in the image.
- **Label these clearly as concept approximations, not locked layouts** — they're meant to
  communicate a general feeling and prop density, not dictate exact in-engine placement.
- **Embed directly in the relevant `Locations/` file** near the room's description, and log it in
  the "Current files" list above.
- Prioritize rooms with real narrative weight (hubs, signature encounters, key-item rooms) over
  minor pass-through spaces — this is meant to be an ongoing, iterative pass across all locations,
  not a one-time exhaustive sweep.

## Convention: concept art for new enemies and bosses

> **This is now a permanent rule, not a one-off pass** (locked 2026-08-13 — see
> [`README.md`](../README.md) rule 16): every new enemy/creature gets concept art as part of
> finishing its design, going forward, not as a separate follow-up task.

Once a new enemy or boss creature's design is written up in `Creatures/`, generate one piece of
concept art for it as standard practice going forward (not just for one-off cases like the
Founders Memorial). Guidelines:

- **Filename:** `Reference/<creature_name>_concept.png`, lowercase with underscores, matching the
  creature's `Creatures/<Name>.md` filename (e.g. `Ashen_Hound.md` → `ashen_hound_concept.png`).
- **Base the prompt strictly on what's already locked** in the creature's own file (Appearance,
  Behavior) plus [`CANON.md`](../CANON.md)'s general infected traits (pale/clouded eyes, "wrong"
  stiff movement or, for fast types, low predatory posture) — don't invent new canon-affecting
  details in the image prompt alone. If the generated image suggests a good new visual detail not
  yet written down (e.g. the Ashen Hound's visible dark vein-like discoloration, a nod to "Black
  Vein" itself), fold it back into the creature's own Markdown file afterward so the prose and the
  art stay in sync — the image should never be the only place a design detail lives.
- **Style:** moody digital concept-art painting, desaturated/muted palette, dramatic low-key
  lighting — consistent with both existing reference images. These are mood/reference art, not
  literal in-game screenshots (2.5D top-down), and should say so explicitly wherever embedded.
- **Embed it directly in the creature's own file** (top or near the Appearance section) with a
  one-line caption explaining what it shows and that it's reference art, then add it to the
  "Current files" list above.
- This same convention applies to bosses (e.g. a future Founders Memorial-style piece for a major
  district boss) and to major unique creatures generally, not just recurring enemy classes.
