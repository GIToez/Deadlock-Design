# Deadlock Protocol — Story Notes

> Brainstorming and unresolved-ideas document. Nothing here is automatically canon.
> Nothing here should be promoted to `CANON.md` or `MASTER_STORY.md` unless explicitly approved.

> **Sources referenced throughout this file:** a city layout **map image** (uploaded 2026-08-12,
> explicitly called a rough/not-final pass by the user); `Deadlock Protocol - Story Design
> Rebuild.docx` (uploaded 2026-08-12, Prologue + full Hotel chapter); `AI.json` (uploaded
> 2026-08-12, a much larger older AI planning conversation covering the Hotel chapter rewrite plus
> Memorial Park, the five districts, the crest/emblem system, and secondary locations). Where
> sources agree independently, that's noted as a positive cross-check. Where they disagree,
> `AI.json` — being the latest, most deliberate pass — is treated as authoritative, and the
> conflict is recorded rather than silently resolved (see `CANON.md` → "Retcons").

## Resolved / Superseded Items (kept for traceability)

- ~~Are the location proper names (St. Dymphna Hospital, Worthy Academy, Steelgate Refinery, Our
  Lady of Solace Monastery, Ravenwood Police Station) placeholders?~~ **Resolved — confirmed.**
  All five names now appear consistently across three independent sources (the map image, the
  docx's incident report, and the full city description in `AI.json`). Treated as locked; see
  `CANON.md`.
- ~~Vanguard Facility placement — doesn't appear on the surface city map.~~ **Resolved.** Per
  `AI.json`, the Vanguard facility is **underground**, beneath Memorial Park's Founders Memorial
  statue, reached only after all five emblems are returned (Chapter 3 — "What Was Hidden"). That's
  exactly why it never appeared on a surface map. `Locations/Vanguard_Facility.md` has been
  updated to reflect this.
- ~~Is the East Wing screwdriver/maintenance-closet a duplication bug?~~ **Resolved — yes, and
  independently confirmed twice.** Both this project's own audit of the docx *and* the user's own
  later audit of the same material inside `AI.json` reached the identical conclusion and the
  identical fix (one pickup, in the East Wing). See `CANON.md` → "Retcons."
- ~~Is the Red Room's backstage route into the Courtyard Security Office logically sound (a
  security office reachable only through a speakeasy lounge)?~~ **Resolved — no, and it's been
  fixed.** Per `AI.json`, the Red Room is now fully self-contained (no backstage, no connection to
  the Security Office), and the Security Office is reached via a separate West Wing service
  corridor instead. The "deadbolted door" detail from the docx is removed entirely.
  `Locations/Ravenwood_Hotel.md` reflects the fix.
- ~~Is the officer in the crashed cruiser the same one seen in the parking lot?~~ **Resolved —
  yes**, confirmed in `AI.json`. He's named **Officer Dale Pruitt**.
- ~~Earl's pre-outbreak "hesitation" — intentional foreshadowing or a mistake?~~ **Resolved.** Per
  `AI.json` (and the user's own read of it — "that was ChatGPT's crappy way of trying to create
  something that shouldn't be there"), it's cut. Earl is now written as a plainly ordinary man
  with zero foreknowledge.
- ~~The muffled scream Jim hears before falling asleep in Room 104.~~ **Resolved — removed from
  canon** per `AI.json`. The horror should arrive with no warning.
- ~~The Red Room singer and the Caretaker were unnamed.~~ **Resolved.** Per `AI.json`: the singer
  is **Della Marsh** ("Della M." on stage); the Caretaker's real identity is **Roy Bullock**
  (longtime hotel maintenance man). Neither had any direct Vanguard connection — the hotel was
  simply caught in the outbreak's radius.
- ~~Was the mutagen called "Black Vein" or "Dark Vein"?~~ **Resolved — Black Vein**, per explicit
  user confirmation in `AI.json`.
- ~~Jim's occupation was never established.~~ **Resolved** — see `CANON.md`.

## Still-Open Questions

- **Exact cause/mechanism of the Black Vein outbreak** — the *attribution* (Vanguard BioSystems /
  Project Ashen) is locked, but *how* containment failed and *why now* are not yet written.
  Reserved for Chapter 3.
- **Cindy Sweets' fate** after her Room 106 abduction — per `AI.json`, explicitly left
  undecided ("we haven't gotten that far in the story yet"), not just unwritten.
- **Maria & Richard Dalton's fate** — per `AI.json`, confirmed to be resolved later at **St.
  Dymphna Hospital** once that chapter is written, but the specific outcome is not yet decided.
- **Gerta's fate** — left undecided; she may not need resolution at all if she doesn't recur.
- **"Something near the tree line" / "something near the cruiser"** (the two lightning-flash
  glimpses during the Highway 13 drive and from the Room 104 window) — per `AI.json`, deliberately
  left as an unexplained, intentional mystery for now, not yet tied to anything specific.
- **Full nature/scope of "Deadlock Protocol" as an authority/directive** — locked as a containment
  order triggered by the outbreak and broadcast over police radio, but who specifically authorizes
  it beyond local Ravenwood government (city hall's own emergency response collapses fast — see
  the Downtown audio log in `Scripts/Chapter_2_Ravenwood.md`) isn't established.
- **The Founders Memorial's two dates don't quite reconcile:** the park's own archway reads "EST.
  1891," but the statue's plaque is dated "1887." Is the statue older than the park's formal
  founding (i.e., moved/rebuilt around when the park was established), or is one of these dates a
  typo that should be unified? Not yet resolved — flagging rather than picking one.
- **Exploration order guardrails** — fully open by design, but no specific difficulty/danger
  tuning has been written per district yet (only that the Monastery, being farthest and most
  isolated, is expected to be hardest).

## Concepts Being Considered

- A two-tier survivor system is locked as a *rule* (see `CANON.md`), but beyond the one confirmed
  example (Police Station officer, alive-if-first / turned-if-later), no other specific
  conditional survivors have been written yet. `AI.json` floated illustrative, **not locked**,
  examples: a civilian barricaded near the Hospital, a Vanguard employee hiding at the Academy, someone
  trapped in a vehicle near the Foundry — all explicitly "not locked yet, just illustrating the
  system."

## Ravenwood City Layout — Cross-Validated

> Two independent sources — a map **image** (uploaded first, explicitly called rough/not-final)
> and a **text description** given later in the `AI.json` conversation (also explicitly "not set
> in stone" for secondary buildings/street names) — describe the same city and agree strongly on
> the big picture. Both are logged below. Where they add complementary detail (e.g. the text
> description adds Highway 13/the bridge/downtown grid; the image adds specific street names),
> both are kept. Still **not formally locked into `CANON.md`** beyond the five-district/crest
> structure itself (already locked, since it's confirmed by three independent sources including
> the fully-scripted Chapter 2 material) — exact building placement is still explicitly subject to
> change per the user.

### Districts and Crests (locked structure — see `CANON.md`)

| Direction | Crest | Primary Location | Other buildings in district (image map) | Matches `Locations/` file |
|---|---|---|---|---|
| North | Faith Crest | Our Lady of Solace Monastery | Hillside Cemetery; Bell Tower; Overlook Trail | `Monastery.md` |
| Northwest | Industry Crest | Steelgate Refinery | Machine Shops; Warehouse District; Loading Docks; Rail Yard (tracks lead into the mountain — Black Vein's entry point) | `Foundry_Refinery.md` |
| Northeast | Medical Crest | St. Dymphna Hospital | Doctor Offices; Parking Structure; Ambulance Bay; Medical Clinic; Quarantine Checkpoint (blocks the road out of town) | `Hospital.md` |
| Southwest | Authority Crest | Ravenwood Police Station | Police Parking; Fire Station; Municipal Garage; Public Works; City Courthouse | `Police_Station.md` |
| Southeast | Knowledge Crest | Worthy Academy | Academy Library; Student Housing; Athletic Field; Playgrounds | `Academy.md` |

### Central / Downtown Ravenwood

- **Memorial Park** — central hub of the city, directly across the street from the Ravenwood
  Hotel (per both sources). Matches `Memorial_Park.md`.
- **Ravenwood Hotel** — sits just north of Ravenwood Bridge / just south of Memorial Park —
  effectively the first major building reached from Highway 13. Matches `Ravenwood_Hotel.md`.
- Downtown itself (regular street grid) contains: City Hall, the Public Library, the Post Office,
  a bookstore, cafés, small shops, offices, older apartments. Three of these are now fully
  scripted secondary locations — **Pearl's Diner, the Ravenwood Public Library, and City Hall** —
  see `Scripts/Chapter_2_Ravenwood.md`.

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

Fully planned in `AI.json` but **not yet scripted** except Downtown's three (see above). Kept here
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

## Character / Creature File Candidates (proposed — NOT yet created)

Updated with names confirmed since the original proposal. Nothing has been created yet — still
awaiting explicit go-ahead:

**Characters/ (proposed):**
- Jim Mercer (protagonist)
- Sarah Mercer (Jim's partner — arc now runs through the Epilogue)
- Earl Whitaker (hotel night clerk → first infected)
- Cindy Sweets (guest, Room 106)
- Maria Dalton (guest, Room 118)
- Richard Dalton (guest, Room 118)
- Janeth Caldwell (guest, Room 112 — dies in Chapter 1)
- Officer Dale Pruitt (parking-lot officer → infected police officer)
- *Borderline:* Gerta (hotel maid) — appears only once, very briefly, with no plot function yet.
  Recommend holding off unless she recurs later.

**Creatures/ (proposed):**
- The Caretaker / Roy Bullock (hotel courtyard boss)
- Della Marsh / "the Red Room Singer" (hotel Red Room mini-boss)
- Shambler (standard infected type — now directly depicted on-screen during the Chapter 2 street
  crossing, not just referenced in passing)

## Things That Still Need Development

- The five districts (Police Station, Hospital, Academy, Refinery, Monastery) are planned in
  outline/secondary-location form (above) but **not yet scripted scene-by-scene**.
- Chapter 3 ("What Was Hidden" — the underground Vanguard facility, Project Ashen, Black Vein's
  full reveal, Jim's final message to Sarah, the ambiguous ending) is locked only at the outline
  level in `CANON.md` — no scenes written.
- The Epilogue ("One More Night" — Sarah's arrival, sequel hook) is likewise outline-only.
- Fate/resolution of Cindy Sweets, the Daltons, and Gerta (see "Still-Open Questions" above).
- The precise mechanism/cause of the Black Vein outbreak.

## Audit — `Deadlock Protocol - Story Design Rebuild.docx` (uploaded 2026-08-12)

> Read in full and transcribed into `CANON.md`, `MASTER_STORY.md`, and
> `Locations/Ravenwood_Hotel.md`. The original `.docx` remains in `DESIGN/` as an archival source
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

## Audit — `AI.json` (uploaded 2026-08-12)

> A ~200-message, ~500,000-character AI planning conversation (NovelCrafter Q&A assistant), read
> in full. It covers: a full rewrite/audit of the Prologue + Hotel chapter (now folded into
> "Chapter 1 — One Night Only"), Jim & Sarah's character voices and full dialogue rewrites, the
> chapter structure (Ch.1/Ch.2/Ch.3/Epilogue), Memorial Park and the Founders Memorial/five-crest
> mechanic in full, the citywide map, and secondary locations for all five districts plus Downtown
> (three of which — Pearl's Diner, the Library, City Hall — are fully scripted). All of this has
> been transcribed into `CANON.md`, `MASTER_STORY.md`, the relevant `Locations/` files, and
> `Scripts/`.
>
> **Not transcribed:** a long stretch of the conversation (roughly the back third) is not story
> content at all — it's the user and the AI going back and forth about whether the AI could
> directly write into the user's NovelCrafter document (it could not; NovelCrafter's Q&A chat is
> read-only against the project, separate from the document's own inline AI writing tool). That
> back-and-forth is a tooling/platform issue, not lore, and has been deliberately left out of the
> design docs.
