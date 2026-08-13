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
  BATTERIES` instead, since he already has his own.
- **Chapter 1 combat/loot pass (2026-08-13), resolving the other two audit items.** Approved
  directly by the project owner:
  - **Shamblers now populate the hotel itself**, not just referenced by name (retconning the
    earlier "not fought until Chapter 2" design). Seven placed throughout the East/West Wing
    power-restoration loop — second-floor east hallway, Dining Hall, Utility Room (timed to the
    screwdriver pickup), Lounge/Recreation, Main Bar, Boiler Room, and the West Wing Service
    Corridor — deliberately not in every room, so the placement stays unpredictable. Kept clear of
    the emotionally heavier beats (Gerta, Cindy, both fuse pickups) and the Red Room. See
    [`Locations/Ravenwood_Hotel.md`](Locations/Ravenwood_Hotel.md) → "Creatures Encountered" and
    [`Creatures/Shambler.md`](Creatures/Shambler.md) for the full list.
  - **Healing items standardized as "Medkit"** across both chapters (replacing the ad hoc "bottled
    water" / "basic medical supplies" phrasing). Four placed in Chapter 1: second-floor east
    hallway suitcase, East Wing Pantry, West Wing Liquor Storage, West Wing Staff Room locker.
  - **Handgun Ammunition** is now also findable before the handgun itself (Utility Room supply
    drawer, West Wing Staff Room locker, Courtyard Security Office desk) — a deliberate
    genre-standard pattern (stockpile ready for when the gun arrives); it loads into the handgun
    automatically once Jim gets it from Officer Pruitt (Scene 41), so nothing is wasted or requires
    justifying bullets with no gun to put them in.
- **Pincer ambush + false-alarm scares added (2026-08-13).** Approved directly by the project
  owner:
  - **Two-Shambler pincer ambush** in the second-floor west hallway (Scene 35) — one bursts from a
    guest room Jim already mentally "cleared" on the way to check on Cindy (Scene 29); his
    instinctive retreat puts him directly in front of a second door, which opens the same way.
    First no-clean-retreat combat moment in the chapter (everything before it is one-on-one with
    room to back away). Brings the hotel's total Shambler count to nine.
  - **Three no-threat "false alarm" tension beats** added to otherwise-quiet optional rooms, so
    empty rooms don't telegraph themselves as safe purely by lacking buildup: a collapsing stack of
    boxes in the Walk-in Freezer (Scene 31), a metallic clang through the vents in the East Wing
    Maintenance Closet (Scene 34), and a photo falling off a shelf in the Piano Area (Scene 37).
    None of these have any payoff — they're pure atmosphere/pacing, not foreshadowing anything
    specific.
- **Courtyard endgame redesign — generator retired, pincer ambush relocated, Fennimore introduced
  (2026-08-13).** Superseding the pincer-ambush placement above. The project owner correctly
  flagged that "restore the generator" felt redundant as a puzzle immediately after a whole
  hotel-power-restoration sequence — the hotel's power is already fully back on by that point, so a
  second "fix the electricity" beat added nothing. Separately, the West Wing pincer ambush (Scene
  35) was stacking two big scares (Cindy's abduction + the ambush) into the same hallway crossing,
  and its "already walked this hallway once" setup didn't reliably hold up once Janeth's hallway
  encounter (Scene 19) was confirmed optional (Jim's room is West Wing; there was never a guaranteed
  reason for him to have crossed to the East Wing before flipping the breaker). Resolved together,
  through several rounds of brainstorming, approved by the project owner:
  - **The generator is gone entirely.** The north gate is a heavy steel-framed double gate,
    retrofitted at some point as the hotel's designated fire-code emergency exit — electrically
    motorized, with a manual crank override required for exactly this kind of power-failure
    scenario (a real, standard fire-code requirement, not an invented mechanic). The obstacle is
    physical/mechanical (a missing crank handle), not electrical — deliberately a different kind of
    puzzle than the two switch-flipping sequences already done.
  - **Fennimore**, the hotel's night-shift security guard (previously only glimpsed via his West
    Wing Staff Room locker), is found dead near the gate. His note reveals he discovered Roy Bullock
    transforming, chained the maintenance shed shut himself rather than confront him, and was
    trying to escape through the gate when he found the crank handle was exactly where he'd stored
    it per protocol — the East Wing Housekeeping Closet, between two new guest rooms, 114 and 116.
    Jim takes the key off his body. This also answers "why is the shed chained shut" with an actual
    story reason instead of an unexplained coincidence, and gives a piece of background lore a real
    payoff instead of leaving him a dangling name tag. See
    [`Characters/Fennimore.md`](Characters/Fennimore.md).
  - **The pincer ambush moved to the East Wing Housekeeping Closet (Scene 43)**, sprung from Rooms
    114 and 116 flanking the closet door. This is a *mandatory* revisit (not an invented reason) —
    the key didn't exist on Jim's first pass through this hallway (Scene 30, deliberately written
    to be forgettable, foreshadowing the two rooms and a locked closet without making anything feel
    ominous), so the ambush is fully earned on the second, motivated pass. The West Wing hallway
    keeps Cindy's scare as its own dedicated beat, no longer sharing the spotlight with a fight.
  - **Fennimore reanimates** on Jim's return to the courtyard with the crank handle — his body is
    simply gone, then he attacks from behind the fountain. An ordinary Shambler fight, no unique
    mechanics, closing his arc. Total hotel Shambler count is now ten.
  - **The Caretaker's reveal is now noise-triggered, not power-triggered.** Jim has to physically
    work the rusted crank by hand; the grinding noise draws Roy out of the shed **mid-effort**, gate
    still only partway open — he finishes opening it after the boss fight. Roy's own maintenance
    log (found post-fight, unchanged otherwise) had its one generator-related entry rewritten to
    reference routine maintenance on the gate's crank gearbox instead.
  - Files touched: `Scripts/Chapter_1_One_Night_Only.md` (Scene 30 foreshadowing; Scene 35 pincer
    removed; Scenes 42–46 rewritten, chapter total now 46 scenes, up from 45), new
    `Characters/Fennimore.md`, `Locations/Ravenwood_Hotel.md` (storyline, rooms, Diagrams 2 and 5,
    creatures, puzzles, key items, documents, scripted events, boss arena hazards),
    `Creatures/Shambler.md`, `Creatures/The_Caretaker.md`.
- **Full Chapter 1 audit (2026-08-13)** — read the entire chapter script front to back, cross-
  checked every note/document for full written text (not just "there's a note here"), verified
  every item pickup and enemy placement against `Locations/Ravenwood_Hotel.md`, and swept every
  file touched by the courtyard redesign above for stale leftovers. Found and fixed:
  - Scene 39 (West Wing Service Corridor) claimed its Shambler was "the last one in the hotel" —
    false since the courtyard redesign added the pincer ambush (Scene 43) and Fennimore (Scene 44)
    afterward. Corrected to note the courtyard is still ahead.
  - The Baseball Bat pickup (Scene 22) was missing its `ITEM ACQUIRED` tag — every other item
    pickup in the chapter has one; added for consistency.
  - `Locations/Ravenwood_Hotel.md` → "Exit / Progression to Next Area" still said "defeating the
    Caretaker restores the north courtyard gate," left over from the old generator design. Fixed
    to reflect that the gate is finished opening manually (crank) after the fight, not powered on.
  - `CANON.md` → "Named Characters Confirmed" was missing Fennimore; added alongside Della Marsh,
    Roy Bullock, and Pruitt.
  - This section (further up) still listed Gerta as "not yet created" and didn't mention Fennimore
    at all — both have files now; added an update note rather than rewriting the historical record.
  - Everything else checked out clean: all documents/notes/placards referenced in the script have
    full verbatim text; all `ITEM ACQUIRED`/`ITEM AVAILABLE` tags match the Key Items/Consumables
    counts in the Location doc exactly (4 Medkits, 3 optional Handgun Ammunition caches, plus the 7
    unique key items); all 10 Shambler placements (7 solo + pincer ×2 + Fennimore) match between
    the script, `Locations/Ravenwood_Hotel.md`, and `Creatures/Shambler.md`; all character/creature
    file scene-number cross-references are correct; all 5 blueprint diagrams re-rendered without
    errors; the chapter's scene list is a clean, gap-free sequence of 46.
- **Emblem direction mechanic corrected (2026-08-13).** The compass-pointer fix logged above (same
  day, earlier entry) was itself wrong — approved correction from the project owner: the
  directional hint is **not** a property of the individual carried emblem. It's the **empty wedge
  slot on the statue itself** — each slot's position on the pentagon (top, upper-right, lower-right,
  lower-left, upper-left) points in the general compass direction of the district its emblem
  belongs to, readable directly off the statue from the very first visit, before collecting
  anything. Fixed in `CANON.md`. This also surfaced a real, separate bug while fixing it:
  `Scripts/Chapter_2_Ravenwood.md` Scene 15's slot-position labels (ORDER at "top," KNOWLEDGE at
  "upper right," etc.) didn't actually correspond to the compass directions in `CANON.md`'s
  crest/district table at all — they were arbitrary. Corrected to a consistent mapping (regular
  pentagon, one vertex due north): FAITH (Monastery, North) at top, MEDICINE (Hospital, Northeast)
  upper-right, KNOWLEDGE (Academy, Southeast) lower-right, ORDER (Police, Southwest) lower-left,
  INDUSTRY (Refinery, Northwest) upper-left. Also updated `Locations/Memorial_Park.md`'s Puzzles
  section to document the mechanic.
- **`Locations/Epilogue.md` created (2026-08-13).** No dedicated file existed for the Epilogue
  before this — only the short summary already in `MASTER_STORY.md`. Consolidated everything known
  (including richer closing-image prose from `AI.json` — "Sarah's silhouette moving through the
  rain toward the city" — that never made it past the outline) into a proper Location-template
  file, with an explicit "Unresolved Ideas" list (time elapsed, whether the player controls Sarah
  at all, whether any creatures appear, what she believes about Jim's fate) so nothing gets
  silently assumed later. `MASTER_STORY.md` now links to it in both places it mentions the
  Epilogue.
- **Chapter 2 NPC documentation check (2026-08-13).** Confirmed the Chapter 2 content written so
  far (`Scripts/Chapter_2_Ravenwood.md`) has **zero on-screen, interactive named NPCs** — Pearl and
  "the Hargrove family" (Pearl's Diner) and the unnamed park groundskeeper (Memorial Park
  guardhouse note) are all name-drops via documents only, never met in person, which is fully
  consistent with the "no random background NPCs get files" rule (same pattern as "H. Garnett" on
  Della Marsh's booking slip in Chapter 1). Nothing is missing here — there's simply nobody to
  document yet. The one specific named-in-concept character still pending is the conditional
  Police Station survivor officer (see `CANON.md` → "Survivor System") — still an unnamed
  placeholder, which is expected since the Police Station itself hasn't been written yet.
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

**Still not created (at the time of this note):** Gerta (hotel maid) — appears once, very briefly,
with no plot function; recommend holding off unless she recurs later. Anything for Memorial Park
or the five districts — none of those chapters have named characters yet.

> **Update:** both since created, once each had a real story beat approved. **Gerta.md** was added
> once her death (killed by The Maw in the Laundry Room) was approved — see the Direction Log
> above. **Fennimore.md** was added later still, once his body/note/reanimation in the courtyard
> was approved (2026-08-13, same section). `Characters/README.md` has the current, complete list.

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
