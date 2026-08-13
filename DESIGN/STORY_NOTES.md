# Deadlock Protocol — Story Notes

> Brainstorming and unresolved-ideas document. Nothing here is automatically canon.
> Nothing here should be promoted to [`CANON.md`](CANON.md) or [`MASTER_STORY.md`](MASTER_STORY.md) unless explicitly approved.

> **Sources referenced throughout this file:** a city layout **map image** (uploaded 2026-08-12,
> explicitly called a rough/not-final pass by the user);
> [`Deadlock Protocol - Story Design Rebuild.docx`](Deadlock%20Protocol%20-%20Story%20Design%20Rebuild.docx)
> (uploaded 2026-08-12, Prologue + full Hotel chapter); [`AI.json`](AI.json) (uploaded
> 2026-08-12, a much larger older AI planning conversation covering the Hotel chapter rewrite plus
> Memorial Park, the five districts, the crest/emblem system, and secondary locations). Where
> sources agree independently, that's noted as a positive cross-check. Where they disagree,
> [`AI.json`](AI.json) — being the latest, most deliberate pass — is treated as authoritative, and the
> conflict is recorded rather than silently resolved (see [`CANON.md`](CANON.md) → "Retcons").

## Resolved / Superseded Items (kept for traceability)

- ~~Are the location proper names (St. Dymphna Hospital, Worthy Academy, Steelgate Refinery, Our
  Lady of Solace Monastery, Ravenwood Police Station) placeholders?~~ **Resolved — confirmed.**
  All five names now appear consistently across three independent sources (the map image, the
  docx's incident report, and the full city description in [`AI.json`](AI.json)). Treated as locked; see
  [`CANON.md`](CANON.md).
- ~~Vanguard Facility placement — doesn't appear on the surface city map.~~ **Resolved.** Per
  [`AI.json`](AI.json), the Vanguard facility is **underground**, beneath Memorial Park's Founders Memorial
  statue, reached only after all five emblems are returned (Chapter 3 — "What Was Hidden"). That's
  exactly why it never appeared on a surface map. [`Locations/Vanguard_Facility.md`](Locations/Vanguard_Facility.md) has been
  updated to reflect this.
- ~~Is the East Wing screwdriver/maintenance-closet a duplication bug?~~ **Resolved — yes, and
  independently confirmed twice.** Both this project's own audit of the docx *and* the user's own
  later audit of the same material inside [`AI.json`](AI.json) reached the identical conclusion and the
  identical fix (one pickup, in the East Wing). See [`CANON.md`](CANON.md) → "Retcons."
- ~~Is the Red Room's backstage route into the Courtyard Security Office logically sound (a
  security office reachable only through a speakeasy lounge)?~~ **Resolved — no, and it's been
  fixed.** Per [`AI.json`](AI.json), the Red Room is now fully self-contained (no backstage, no connection to
  the Security Office), and the Security Office is reached via a separate West Wing service
  corridor instead. The "deadbolted door" detail from the docx is removed entirely.
  [`Locations/Ravenwood_Hotel.md`](Locations/Ravenwood_Hotel.md) reflects the fix.
- ~~Is the officer in the crashed cruiser the same one seen in the parking lot?~~ **Resolved —
  yes**, confirmed in [`AI.json`](AI.json). He's named **Officer Dale Pruitt**.
- ~~Earl's pre-outbreak "hesitation" — intentional foreshadowing or a mistake?~~ **Resolved.** Per
  [`AI.json`](AI.json) (and the user's own read of it — "that was ChatGPT's crappy way of trying to create
  something that shouldn't be there"), it's cut. Earl is now written as a plainly ordinary man
  with zero foreknowledge.
- ~~The muffled scream Jim hears before falling asleep in Room 104.~~ **Resolved — removed from
  canon** per [`AI.json`](AI.json). The horror should arrive with no warning.
- ~~The Red Room singer and the Caretaker were unnamed.~~ **Resolved.** Per [`AI.json`](AI.json): the singer
  is **Della Marsh** ("Della M." on stage); the Caretaker's real identity is **Roy Bullock**
  (longtime hotel maintenance man). Neither had any direct Vanguard connection — the hotel was
  simply caught in the outbreak's radius.
- ~~Was the mutagen called "Black Vein" or "Dark Vein"?~~ **Resolved — Black Vein**, per explicit
  user confirmation in [`AI.json`](AI.json).
- ~~Jim's occupation was never established.~~ **Resolved** — see [`CANON.md`](CANON.md).
- ~~Gerta's fate was left undecided.~~ **Resolved, approved directly by the project owner
  (2026-08-12):** she's killed by a previously-unnamed, now-named creature, **The Maw** — the same
  presence that drags Cindy Sweets into Room 106 later in Chapter 1. Her body is discovered in the
  hotel **Laundry Room**, now placed in the East Wing's ground-floor service area (see the hotel
  layout resolution below — this room moved from its original West Wing/behind-the-bar placement).
  See [`Creatures/The_Maw.md`](Creatures/The_Maw.md), [`Characters/Gerta.md`](Characters/Gerta.md), and
  [`Scripts/Chapter_1_One_Night_Only.md`](Scripts/Chapter_1_One_Night_Only.md) (Scene 33).

## Direction Log

- **Content rating confirmed as mature (M) — 2026-08-12.** Explicit violence/gore, strong
  profanity, and nudity are all permitted; writing should not self-censor by default going
  forward. Locked as rule 13 in [`README.md`](README.md). A situational (not blanket) tone
  punch-up pass was subsequently done on `Scripts/Chapter_1_One_Night_Only.md`.
- **Presentation/camera clarified via reference screenshots — 2026-08-12.** Deadlock Protocol is
  2.5D top-down (a fact that existed in `AI.json` from its very first message but was never
  actually written into a design doc until now — genuine documentation gap, now fixed). The
  in-game camera stays close to the player and shows roughly a room's-width of space, not a wide
  cinematic view — confirmed against two reference screenshots (a full Ravenwood Hotel lobby
  layout, and an actual gameplay-viewport screenshot showing a Shambler attacking Jim near the
  reception desk). Locked as rule 14 in [`README.md`](README.md) and under "Presentation &
  Perspective" in [`CANON.md`](CANON.md). The existing Chapter 1/2 scripts have **not** been
  audited yet for language that reads too cinematic/wide-shot for this camera — flagged as
  optional follow-up work, not yet done.
- **Ravenwood Hotel real floor plan reference + full power-restoration route rebuild —
  2026-08-12.** The project owner shared an AI-generated architectural floor plan (ground floor +
  guest floor) for the hotel. It was explicitly flagged as imperfect/AI-rendered (missing some
  rooms, not gospel) but gave the project a real two-floor layout to reconcile against the earlier,
  purely relational room-connectivity diagrams. Through several rounds of back-and-forth, the
  following was locked as the hotel's real architecture and the exact East/West Wing
  power-restoration route:
  - **Two floors only** — a ground floor and a guest floor above it. No second,
    player-inaccessible service floor, and no crossover corridor between wings (the earlier
    "second-floor service crossover" and "West Wing Maintenance Office reached via service
    stairwell" design is fully retired — see [`CANON.md`](CANON.md) → "Retcons").
  - The guest floor is freely walkable the entire chapter; the **Public Stairwells** at the end of
    each guest hallway (down to the ground floor) are what's power-gated per wing.
  - **The Laundry Room moved from the West Wing (behind the Main Bar) to the East Wing**, next to
    the Utility Room/Kitchen/Dining Hall — this is where Gerta's death scene now lives.
  - **The Red Room is explicitly tied to the Main Bar** (an entrance directly off it), not a
    generic hallway branch.
  - The rear **Courtyard is a single space**, reachable from the West Wing, the East Wing, and a
    passage under the Lobby's Grand Staircase — though only the West Wing route (via the Courtyard
    Security Office) is actually used/opened in Chapter 1.
  - The East Wing retrieval loop (Dining Hall → Kitchen → Pantry/Freezer → Utility Room →
    Laundry/Linen Room → East Wing Maintenance Closet) ends in a barricaded door that Jim clears
    by hand, opening a **permanent shortcut straight back to the Lobby** — no tool needed for that
    door; the screwdriver's only job is opening the fuse housing at the breaker panel.
  - The auxiliary fuse itself is in a small, simply-shut **West Wing Maintenance Room** on the
    guest floor (near the West Public Stairwell) — not power-gated, just closed. Reaching it is
    what re-anchors **Cindy's Room 106 jumpscare**, which now triggers while crossing the guest
    floor's west hallway to get there (previously it was anchored to a return trip through a
    since-removed second-floor route).
  - `Locations/Ravenwood_Hotel.md` (storyline, room list, all 5 blueprint diagrams, puzzles, key
    items), `Scripts/Chapter_1_One_Night_Only.md` (Scenes 28–40 fully rewritten), `MASTER_STORY.md`,
    and the affected character/creature files (`Characters/Gerta.md`, `Characters/Cindy_Sweets.md`,
    `Characters/README.md`, `Creatures/The_Maw.md`, `Creatures/Della_Marsh.md`) were all updated to
    match. Scene numbering from Scene 41 onward (Officer Pruitt, Courtyard, Generator, Caretaker)
    is unchanged.
  - **Follow-up (same day):** Cindy's Room 106 jumpscare was moved to trigger **before** Gerta's
    death rather than after — Jim now swings by Cindy's room right after flipping the East Wing
    breaker (Scene 29), before heading to the East Wing stairwell, rather than during the later
    trip to get the auxiliary fuse. Gerta's death (in the East Wing Laundry Room) is now Scene 33.
    This only reordered/renumbered Scenes 29–35; Scene 36 onward is unaffected. Also caught and
    fixed in the process: Scenes 39–40 (West Wing Service Corridor, Courtyard Security Office) had
    been accidentally dropped during the initial rewrite and were restored.
- **Chapter 1 audit + starting flashlight fix (2026-08-13).** A full pass over Chapter 1 caught one
  real continuity gap: Jim explored genuinely dark, powerless spaces (the East Wing stairwell in
  particular) with no personal light source, while Chapter 2 originally introduced a "found"
  police flashlight framed as his first one. Resolved, approved directly by the project owner:
  **Jim starts the entire game with his own belt-clipped flashlight** — standard field-engineer
  everyday-carry, not a pickup. Locked in [`CANON.md`](CANON.md) → "Player Starting Equipment" and
  [`Characters/Jim_Mercer.md`](Characters/Jim_Mercer.md). Chapter 2's police-flashlight beat (Scene
  2) was changed from an `ITEM ACQUIRED: FLASHLIGHT` pickup to `ITEM ACQUIRED: FLASHLIGHT
  BATTERIES` instead, since he already has his own. Two other items surfaced by the same audit are
  still open, not yet decided: (1) Chapter 1's combat roster is very sparse for its length — only
  Earl, Officer Pruitt, and the optional Della Marsh fight before the Caretaker boss, with no
  generic Shambler encounters (those start in Chapter 2) — flagging in case that's worth changing
  rather than confirmed intentional; (2) no standardized healing/consumable item name exists yet
  across chapters (Chapter 1 says "bottled water," Chapter 2 says "basic medical supplies") — likely
  a systems-doc concern rather than a story one.
- The two reference screenshots (lobby layout + gameplay viewport combat shot) were shared inline
  in chat only — not saved to the repo, since inline chat images aren't accessible as real files.
  If they should become permanent reference material, they need to be pushed as actual files
  (same workflow as `AI.json` and the story `.docx`).
- **Update (2026-08-12):** the project owner did push a real file — `spr_cindy_jumpscare.gif` —
  directly into `Characters/` (embedded in `Characters/Cindy_Sweets.md`). Confirmed via full
  frame-by-frame extraction (51 frames) that it matches `Scripts/Chapter_1_One_Night_Only.md`
  Scene 29 as written; no script changes were needed. Also confirmed: the lobby combat screenshot
  showed **The Maw**, not a generic Shambler, but it was explicitly a tech/engine demo, not a
  planned encounter — The Maw is not fought in Chapter 1, matching what's already documented.
- **Chapter 1 camera-consistency pass done (2026-08-12):** fixed Scene 1 (no player driving
  control on Highway 13 — it's a fixed shot; control begins at the hotel exterior, Scene 2) and
  softened one sightline claim in Scene 3. Added a documented convention (in the script's header
  note) for how full-room descriptions (Lobby, Courtyard) and multi-NPC simultaneous reaction
  beats relate to the actual constrained camera, rather than rewriting every atmospheric line.

## Still-Open Questions

- **Exact cause/mechanism of the Black Vein outbreak** — the *attribution* (Vanguard BioSystems /
  Project Ashen) is locked, but *how* containment failed and *why now* are not yet written.
  Reserved for Chapter 3.
- **Cindy Sweets' fate** after her Room 106 abduction — her abductor is now identified (**The
  Maw** — see below), but what actually happened to her (alive / dead / turned / something else)
  remains explicitly undecided per the project owner. Do not infer a resolution from the Gerta
  reveal — they are two separate open/closed questions.
- **Maria & Richard Dalton's fate** — per [`AI.json`](AI.json), confirmed to be resolved later at **St.
  Dymphna Hospital** once that chapter is written, but the specific outcome is not yet decided.
- **"Something near the tree line" / "something near the cruiser"** (the two lightning-flash
  glimpses during the Highway 13 drive and from the Room 104 window) — per [`AI.json`](AI.json), deliberately
  left as an unexplained, intentional mystery for now, not yet tied to anything specific.
- **Full nature/scope of "Deadlock Protocol" as an authority/directive** — locked as a containment
  order triggered by the outbreak and broadcast over police radio, but who specifically authorizes
  it beyond local Ravenwood government (city hall's own emergency response collapses fast — see
  the Downtown audio log in [`Scripts/Chapter_2_Ravenwood.md`](Scripts/Chapter_2_Ravenwood.md)) isn't established.
- **The Founders Memorial's two dates don't quite reconcile:** the park's own archway reads "EST.
  1891," but the statue's plaque is dated "1887." Is the statue older than the park's formal
  founding (i.e., moved/rebuilt around when the park was established), or is one of these dates a
  typo that should be unified? Not yet resolved — flagging rather than picking one.
- **Exploration order guardrails** — fully open by design, but no specific difficulty/danger
  tuning has been written per district yet (only that the Monastery, being farthest and most
  isolated, is expected to be hardest).

## Concepts Being Considered

- A two-tier survivor system is locked as a *rule* (see [`CANON.md`](CANON.md)), but beyond the one confirmed
  example (Police Station officer, alive-if-first / turned-if-later), no other specific
  conditional survivors have been written yet. [`AI.json`](AI.json) floated illustrative, **not locked**,
  examples: a civilian barricaded near the Hospital, a Vanguard employee hiding at the Academy, someone
  trapped in a vehicle near the Foundry — all explicitly "not locked yet, just illustrating the
  system."

## Ravenwood City Layout — Cross-Validated

> Two independent sources — a map **image** (uploaded first, explicitly called rough/not-final)
> and a **text description** given later in the [`AI.json`](AI.json) conversation (also explicitly "not set
> in stone" for secondary buildings/street names) — describe the same city and agree strongly on
> the big picture. Both are logged below. Where they add complementary detail (e.g. the text
> description adds Highway 13/the bridge/downtown grid; the image adds specific street names),
> both are kept. Still **not formally locked into [`CANON.md`](CANON.md)** beyond the five-district/crest
> structure itself (already locked, since it's confirmed by three independent sources including
> the fully-scripted Chapter 2 material) — exact building placement is still explicitly subject to
> change per the user.

### Districts and Crests (locked structure — see [`CANON.md`](CANON.md))

| Direction | Crest | Primary Location | Other buildings in district (image map) | Matches `Locations/` file |
|---|---|---|---|---|
| North | Faith Crest | Our Lady of Solace Monastery | Hillside Cemetery; Bell Tower; Overlook Trail | [`Monastery.md`](Locations/Monastery.md) |
| Northwest | Industry Crest | Steelgate Refinery | Machine Shops; Warehouse District; Loading Docks; Rail Yard (tracks lead into the mountain — Black Vein's entry point) | [`Foundry_Refinery.md`](Locations/Foundry_Refinery.md) |
| Northeast | Medical Crest | St. Dymphna Hospital | Doctor Offices; Parking Structure; Ambulance Bay; Medical Clinic; Quarantine Checkpoint (blocks the road out of town) | [`Hospital.md`](Locations/Hospital.md) |
| Southwest | Authority Crest | Ravenwood Police Station | Police Parking; Fire Station; Municipal Garage; Public Works; City Courthouse | [`Police_Station.md`](Locations/Police_Station.md) |
| Southeast | Knowledge Crest | Worthy Academy | Academy Library; Student Housing; Athletic Field; Playgrounds | [`Academy.md`](Locations/Academy.md) |

### Central / Downtown Ravenwood

- **Memorial Park** — central hub of the city, directly across the street from the Ravenwood
  Hotel (per both sources). Matches [`Memorial_Park.md`](Locations/Memorial_Park.md).
- **Ravenwood Hotel** — sits just north of Ravenwood Bridge / just south of Memorial Park —
  effectively the first major building reached from Highway 13. Matches [`Ravenwood_Hotel.md`](Locations/Ravenwood_Hotel.md).
- Downtown itself (regular street grid) contains: City Hall, the Public Library, the Post Office,
  a bookstore, cafés, small shops, offices, older apartments. Three of these are now fully
  scripted secondary locations — **Pearl's Diner, the Ravenwood Public Library, and City Hall** —
  see [`Scripts/Chapter_2_Ravenwood.md`](Scripts/Chapter_2_Ravenwood.md).

### Edges of the Map / Terrain

- **Highway 13** runs east–west along the southern edge of the city; a single road crosses
  **Ravenwood Bridge** over the river and is the only way into town from the south. Nothing
  significant exists south of the river. (The image map additionally shows a sign reading "To
  Oakridge, 35 miles" past the bridge — not contradicted by the text description, just not
  repeated in it.)
- A **river** runs through Ravenwood (enters near the northwest, bends around the city, exits
  south), with smaller drainage channels/tributaries, plus rail cuts, retaining walls, fences,
  collapsed roads, police barricades, flooded channels, and locked gates acting as natural
  progression barriers throughout.
- The **Northwest district's rail yard** has tracks that lead into the mountain — confirmed as the
  physical point Black Vein entered Ravenwood. Visible from the rail yard, not enterable during
  Chapter 2 (reserved for later).

### Secondary Locations (per district — 2–3 each, "enough to not feel boring," per the user)

Fully planned in [`AI.json`](AI.json) but **not yet scripted** except Downtown's three (see above). Kept here
as a working list for whenever the five districts get written:

- **Southwest / Authority (Police Station):** Ravenwood Fire Station; Municipal Garage / Impound
  Lot; City Courthouse.
- **Southeast / Knowledge (Academy):** a residential block (Elm Street or similar); a
  neighborhood pharmacy; the Academy athletic field/bleachers.
- **Northeast / Medical (Hospital):** all reworked to be physically part of the hospital complex
  rather than standalone buildings (the user pointed out a town this size wouldn't have a separate
  urgent care *and* a hospital) — the **Hospital Parking Structure**, **Ravenwood EMS /
  Ambulance Bay** (across the street from the hospital), and a small, separate **Ravenwood Animal
  Clinic** (whose vet notebook is meant to foreshadow that animal behavior changed *before* the
  human outbreak — important Chapter 3 foreshadowing).
- **Northwest / Industry (Refinery):** the Ravenwood Rail Yard (sealed freight car, tunnel into
  the mountain); a Worker Housing Block; the Steelgate Loading Docks.
- **North / Faith (Monastery):** a Hillside Residential Street (an unsent letter warning the
  monastery about Black Vein; a calm, living dog on a porch as a deliberate emotional beat); the
  Hillside Cemetery (disturbed graves, one very recent unmarked grave); the Overlook Trail (a
  quiet vista of the whole burning city — meant to reframe the scale of the disaster for the
  player).

## Character / Creature Files — Created

The Chapter 1 cast now has files in `Characters/` and `Creatures/` (created after the story
analysis + [`AI.json`](AI.json) review, per the original "analyze first, then create" instruction):

**Characters/:** Jim Mercer, Sarah Mercer, Earl Whitaker, Cindy Sweets, Maria Dalton, Richard
Dalton, Janeth Caldwell, Officer Dale Pruitt.

**Creatures/:** The Caretaker (Roy Bullock), Della Marsh (the Red Room Singer), and **Shambler**
(the standard/base infected type — this was a real documentation gap: referenced by name in the
Caretaker's design notes since the original docx audit, but never given its own write-up until
now).

**Still not created:** Gerta (hotel maid) — appears once, very briefly, with no plot function;
recommend holding off unless she recurs later. Anything for Memorial Park or the five districts —
none of those chapters have named characters yet.

## Things That Still Need Development

- The five districts (Police Station, Hospital, Academy, Refinery, Monastery) are planned in
  outline/secondary-location form (above) but **not yet scripted scene-by-scene**.
- Chapter 3 ("What Was Hidden" — the underground Vanguard facility, Project Ashen, Black Vein's
  full reveal, Jim's final message to Sarah, the ambiguous ending) is locked only at the outline
  level in [`CANON.md`](CANON.md) — no scenes written.
- The Epilogue ("One More Night" — Sarah's arrival, sequel hook) is likewise outline-only.
- Fate/resolution of Cindy Sweets and the Daltons (see "Still-Open Questions" above). Gerta's fate
  is now resolved (see "Resolved / Superseded Items" above).
- The precise mechanism/cause of the Black Vein outbreak.

## Audit — [`Deadlock Protocol - Story Design Rebuild.docx`](Deadlock%20Protocol%20-%20Story%20Design%20Rebuild.docx) (uploaded 2026-08-12)

> Read in full and transcribed into [`CANON.md`](CANON.md), [`MASTER_STORY.md`](MASTER_STORY.md), and
> [`Locations/Ravenwood_Hotel.md`](Locations/Ravenwood_Hotel.md). The original `.docx` remains in `DESIGN/` as an archival source
> reference.

**Structural inconsistency:** the document's own opening Table of Contents (TAB 01 — Core Story
Overview ... TAB 15 — Implementation Notes) does not match the actual tab numbering used in the
document body (body TAB 01 = Prologue, ... body TAB 12 = Hotel Courtyard). The body instead tells
the hotel chapter as one continuous scene-by-scene script. This is effectively superseded by the
`DESIGN/` folder structure and, further, by the cleaner "Scenes not Tabs" numbering adopted in
`Scripts/` per your explicit instruction.

**Leftover draft duplication:** the docx contains a shorter, rougher, near-identical draft of the
opening Highway 13 scene immediately before the polished, locked version. Not transcribed as a
distinct beat — flagging in case it's worth deleting from the source `.docx` itself (which has
been left otherwise untouched).

## Audit — [`AI.json`](AI.json) (uploaded 2026-08-12)

> A ~200-message, ~500,000-character AI planning conversation (NovelCrafter Q&A assistant), read
> in full. It covers: a full rewrite/audit of the Prologue + Hotel chapter (now folded into
> "Chapter 1 — One Night Only"), Jim & Sarah's character voices and full dialogue rewrites, the
> chapter structure (Ch.1/Ch.2/Ch.3/Epilogue), Memorial Park and the Founders Memorial/five-crest
> mechanic in full, the citywide map, and secondary locations for all five districts plus Downtown
> (three of which — Pearl's Diner, the Library, City Hall — are fully scripted). All of this has
> been transcribed into [`CANON.md`](CANON.md), [`MASTER_STORY.md`](MASTER_STORY.md), the relevant `Locations/` files, and
> `Scripts/`.
>
> **Not transcribed:** a long stretch of the conversation (roughly the back third) is not story
> content at all — it's the user and the AI going back and forth about whether the AI could
> directly write into the user's NovelCrafter document (it could not; NovelCrafter's Q&A chat is
> read-only against the project, separate from the document's own inline AI writing tool). That
> back-and-forth is a tooling/platform issue, not lore, and has been deliberately left out of the
> design docs.
