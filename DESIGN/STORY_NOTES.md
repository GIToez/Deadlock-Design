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
- **Sarah/Jim call dialogue rewritten, three passes (2026-08-13).** First pass fixed two issues
  flagged by the project owner: missing "I love you" in both calls, and a logic mismatch where
  Sarah says "text me when you stop" (Scene 1) but then *calls* Jim in Scene 3 rather than
  receiving a text. Second pass, prompted by the project owner pointing out that Scene 3 is the
  **only real-time impression the player ever gets of Sarah before she reappears in the
  [`Epilogue`](Locations/Epilogue.md)**, added a "little dot" location-tracking explanation as a
  dialogue reveal in Scene 1 — but the project owner flagged this third draft as feeling
  artificial/over-explained, on two specific points: (1) the pre-existing "GPS took you through a
  field in Ohio" joke works better **unexplained**, as a pure running-joke callback, not spelled
  out with a full tracking-app conversation; (2) Jim already knowing and being fine with Sarah
  tracking his location reads as more natural than a "gotcha" reveal where he's surprised/mildly
  scandalized — and the *reason* it exists should be practical safety (he travels for work; she'd
  know where to send help if something ever happened), not a "sneaky/cute" quirk. Third pass fixed
  both:
  - Scene 1's cornfield joke reverted to fully unexplained — no GPS/tracking mechanism mentioned
    there at all, just the callback line itself.
  - Scene 3 now establishes the tracking arrangement in one short piece of **narration**, once,
    stated as a mundane, already-settled fact of their relationship (practical/safety-motivated,
    not secretive) — no dialogue "reveal," no surprise from Jim. The dialogue itself was also
    trimmed to reduce joke-per-line density and read more like a real, slightly mundane phone
    call.
  - The ending was simplified too — cut an overly neat, on-the-nose foreshadowing line ("I'll be
    right here either way") that read as written for the audience rather than something a person
    would actually say; the full "I love you" now lands on its own, unadorned.
  - Updated `Characters/Sarah_Mercer.md` (Personality, Relationships, Dialogue Characteristics,
    Important Scenes) to match — tracking is now described as a known, practical safety habit, not
    a secret or a "reveal."
- **Police Station district written — Scenes 22–33 (2026-08-13).** The Southwest District
  (Authority Crest) is now fully scripted, closing three open questions [`AI.json`](AI.json) raised
  but never answered (what's inside the station, who the conditional survivor is, what the emblem
  looks like/where it is). All of the following is **new and treated as a proposal pending
  review**, not locked canon, even though it's been written into `CANON.md` and the location file
  for tracking purposes:
  - **The station is two buildings**, not one: a modern annex (the working department — lobby,
    bullpen, armory, dispatch) and, across a breezeway, the original 1887 station house (boarded,
    historical-only) — directly justifying the guardhouse note's specific "not the annex — the
    original structure" distinction, which had been sitting unresolved since Memorial Park was
    written.
  - **The Tier 2 conditional survivor is Sergeant Ruth Calloway**, the desk sergeant — a concrete
    name/character for a mechanic that was previously locked only as an abstract rule in
    `CANON.md`. Alive-if-first, she gives Jim the armory key and the Marshal Hale lead directly;
    her "already turned" version is described (body + note, same information) but **not yet
    scripted scene-by-scene** — flagged as follow-up work.
  - **The Authority Crest** is a bronze wedge-shaped medallion in a dusty display case in the old
    station house's main hall — a department "heirloom" nobody ever questioned — bearing a relief
    portrait, name, and title of **Marshal Josiah Hale, first peace officer of Ravenwood (1887)**,
    proposed here as the Authority Crest's founder. The other four founders' names are deliberately
    deferred (a damaged 1887 charter document lists five "Incorporators," only Hale's name
    legible) rather than invented wholesale, so later districts can pick names that feel
    consistent with his.
  - **New equipment:** a shotgun (the game's second firearm), gated behind Sergeant Calloway's
    trust rather than a cold pickup.
  - **New creature type:** the **Ashen Hound** (`Creatures/Ashen_Hound.md`) — two named mutated
    K-9 unit dogs (Diesel and Baxter) at the Municipal Garage, the game's first fast/pack-hunting
    enemy, introduced as this district's "major encounter" per [`AI.json`](AI.json)'s per-district
    design rule, and established as a reusable creature class (not a one-off) for later districts.
  - **Concept art generated (same day):** `Assets/Reference/ashen_hound_concept.png`, depicting
    Diesel at the Municipal Garage. The generated image suggested a good visual detail not
    previously written down — faint dark vein-like discoloration visible beneath the cracked
    hide, a literal nod to Black Vein itself — folded back into `Creatures/Ashen_Hound.md`'s
    Appearance section so the art and the prose stay in sync. Per the project owner's request,
    `Assets/README.md` now documents a standing convention for generating concept art for future
    enemies/bosses (filename pattern, style consistency, and the rule that any new visual detail
    an image suggests gets written back into the creature's own file rather than living only in
    the image).
  - The three secondary locations (Fire Station, Municipal Garage, City Courthouse) were written
    to match [`AI.json`](AI.json)'s own outline notes for them fairly closely — dispatch board,
    mechanic's office, courthouse survivor camp — with the courthouse's evidence room deliberately
    keyed to an item found back at the station (Evidence Room Key), as originally proposed in
    `AI.json`.
  - Updated `CANON.md` (Named Characters Confirmed, Survivor System, a new Ashen Hound entry under
    Creature Classification), `MASTER_STORY.md`, `Locations/Police_Station.md` (fully written, was
    a `_TBD_` placeholder), and created `Characters/Ruth_Calloway.md` and
    `Creatures/Ashen_Hound.md`.
- **Chapter 2 opening: Cindy's blood trail and robe (2026-08-13).** New content, approved directly
  by the project owner, continuing (not resolving) Cindy Sweets' unresolved Chapter 1 thread: a
  blood trail starts right at the courtyard gate as Jim steps onto the street (Scene 1), runs
  roughly parallel to his path, thins out, and — rather than leading directly to the park's south
  gate — goes wide of it and ends at her torn, empty, hotel-issue robe in the hedges along the
  fence line (end of Scene 3, right before the park). No body, no further trail. Explicitly
  designed as an escalation of dread, not a resolution — see the "Cindy Sweets' fate" entry above.
  Updated `Characters/Cindy_Sweets.md` and `Locations/Memorial_Park.md` to reflect it.
- **Founders Memorial plaque redesigned as a circular medallion (2026-08-13).** The project owner
  shared a rough reference image of the emblem/plaque and asked for an improved version. This
  changed the physical shape from what `CANON.md` previously said (a flat plaque that the five
  emblems combine to form a pentagon) to: a **circular medallion** with a small pentagon hub at
  the exact center (bearing a single weathered "V" — an unexplained, deniable early visual hint at
  the Vanguard connection, sitting in plain sight on an 1887 monument) and five trapezoidal wedge
  slots ringed around it like a compass rose. Generated a new concept-art reference image
  (`Assets/Reference/founders_memorial_plaque_concept.png`) showing this design with correct
  iconography (Cross/Faith/North, Serpent-Caduceus/Medical/Northeast, Torch/Knowledge/Southeast,
  Key/Authority/Southwest, Anvil/Industry/Northwest) and two wedges filled/glowing to demonstrate
  the assembled-vs-empty look. Updated `CANON.md` (added a Wedge Position column to the
  crest/district table), `Locations/Memorial_Park.md`, `MASTER_STORY.md` (three separate
  mentions), and `Scripts/Chapter_2_Ravenwood.md` Scenes 14–15 (renamed "slots" to "wedges,"
  fixed the plaque's physical description) to match. The directional-hint mechanic itself
  (corrected earlier the same day, see above) is unaffected — the wedge positions still map to the
  same five compass directions and districts.
- **Concept art refined, v2 (2026-08-13, same day).** Two fixes to the first pass, approved by the
  project owner: (1) the center hub rendered as a six-sided shape instead of a proper five-sided
  pentagon — regenerated correctly; (2) more importantly, **each emblem needs to read as a
  separate physical piece that fully fills its recess**, not just a small glowing icon on the same
  continuous stone surface as the empty slots. Regenerated
  `Assets/Reference/founders_memorial_plaque_concept.png` (replacing the original in place) with a
  visibly different, lighter-colored metal for the two filled wedges and a clear raised
  seam/lip where each inserted piece meets the surrounding frame, versus bare dark recessed cavities
  (with only a faint engraved silhouette) for the three empty ones. Tightened the wording in
  `CANON.md`, `Locations/Memorial_Park.md`, and `Scripts/Chapter_2_Ravenwood.md` Scene 14 to match:
  emblems are explicitly "a separate, physical wedge-shaped piece that inserts into and completely
  fills its matching recess... like a puzzle piece," not a marking that appears on existing stone.
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
- **Room concept art style-consistency pass (2026-08-13, same day).** Project owner feedback: "Make
  sure all room concepts follow the in game screenshots. Some don't." Audited every existing room
  concept against the real in-engine `Assets/Screenshots/` references and found the drift: several
  renders had leaned toward an isometric/painterly "3D diorama" look instead of the flat, directly-
  overhead, tile-based retro RPG style the actual screenshots use. Affected: `hotel_courtyard_concept.png`,
  `hotel_red_room_concept.png`, and all 16 Police Station room concepts. Fixed by rewriting the
  generation prompt to explicitly require "Strictly flat 2D top-down retro RPG tileset pixel art,
  viewed directly from above, NOT isometric and NOT a 3D diorama," validating it with two test
  renders, then re-generating and overwriting all 18 affected files in place. Incidentally fixed
  three of the previously flagged non-canonical details in the new renders (Records/Dispatch's
  invented "DET. HARRIS" nameplate, the Break Room locker's wrong name, and the Municipal Garage
  sign's wrong city name); the Old Station House medallion still isn't the exact canonical wedge
  shape but reads close enough for mood reference. Every other existing hotel/police-station room
  concept was re-checked against the screenshots and confirmed already consistent — no further
  regenerations needed. See [`Assets/README.md`](Assets/README.md) for the full file list.
- **Creature concept-art coverage completed (2026-08-13, same day).** Project owner: "Let's also do
  renders for creatures we don't have all. Make sure to do it for all future as well" — the second
  half of rule 16 in `README.md` (every new enemy/creature gets concept art) plus a backfill pass
  for the four creature files that predated that rule: the [Shambler](Creatures/Shambler.md),
  [The Caretaker](Creatures/The_Caretaker.md), [Della Marsh](Creatures/Della_Marsh.md), and
  [The Maw](Creatures/The_Maw.md). Generated one moody digital concept-art painting for each,
  consistent with the Ashen Hound's existing convention, and embedded each in its own file. Two
  minor approximations flagged in `The_Caretaker.md` rather than treated as canon: the render
  doesn't clearly distinguish hotel-maintenance overalls from generic dark workwear, and doesn't
  show a distinctly off-color glowing eye. Every creature in `Creatures/` now has concept art;
  going forward, rule 16 means this happens automatically as part of writing up any new creature,
  not as a separate catch-up pass.

## Implemented — Police Station Restructure (RE-style, approved and written 2026-08-13)

Per the new "District Main-Location Design Standard" locked in [`CANON.md`](CANON.md), the
originally-written Police Station (`Scripts/Chapter_2_Ravenwood.md`, then Scenes 22–33) was too
short and linear — it needed a Resident Evil RPD-style key-and-lock restructure before the
remaining four districts are written, so all five are built to the same standard. **This plan was
approved by the project owner and has been written into the script**, now Scenes 22–40 (see the
follow-up entry below for the "basic functioning rooms" addition that grew this further) — laid out
below (kept in its original planning form for traceability) the same way Memorial Park's layout
was decision-logged before it was scripted.

> **Revision note:** the first draft of this plan put the Ashen Hound encounter at the Municipal
> Garage and an "evidence room" at the Courthouse. The project owner flagged both as ungrounded —
> a K-9 unit's actual home is the station itself, not a general vehicle yard, and a courthouse
> doesn't run long-term evidence storage (that's the department's own Property & Evidence Room).
> Both are corrected below by moving weight into the main station building itself, which also
> better fits the design standard's intent (the main location should carry the district's densest
> content, not its secondary stops).

**What stays the same:** Sergeant Calloway as the survivor, the shotgun as the equipment reward,
the Authority Crest's location/appearance (old station house display case, Marshal Josiah Hale),
Diesel and Baxter as the Ashen Hound encounter, and all four buildings (Station, Fire Station,
Municipal Garage, Courthouse).

**What changes:**

1. **Bullpen (hub).** Visibly gates three locked things at once instead of unlocking in sequence:
   the **Armory** (keyed lock), the **Chief's Office** (keyed lock), and a padlocked **Property &
   Evidence Room** (a proper room now, not just a wall locker — sealed, requires bolt cutters).
   Calloway is barricaded in Records/Dispatch, same as now.
2. **Calloway** gives Jim the **Chief's Office key** (department protocol — the desk sergeant
   holds it) and explains that **Corporal Reyes** — who had the armory key on his belt — went to
   check on the **K-9 unit**, kenneled in its own room at the back of the station, when the dogs
   started acting up, and never came back. She also mentions the Property Room's been padlocked
   for months and "bolt cutters would do it."
3. **Chief's Office** (new room, unlocked with Calloway's key): confirms Reyes went to check the
   kennels; contains the **Old Station Skeleton Key** — kept here specifically because the Chief,
   not the desk sergeant, is the one responsible for the old building — plus a minor reward.
4. **K-9 Unit Room** (new area, off a back hallway of the annex itself — not the Garage, not
   locked, just somewhere Calloway's lead points Jim toward): Corporal Reyes' body, the **Armory
   Key** on his belt, and the Ashen Hound fight (Diesel and Baxter) right there in their own
   kennel room. This keeps the encounter in the main building, where a K-9 unit actually would be,
   and gives it a direct narrative reason to be on the critical path (Reyes is why Jim has to go
   there at all) rather than a stand-alone side-building detour.
5. **Armory** (Reyes' key): shotgun + shells, as already written.
6. **Fire Station** (secondary, now load-bearing): adds a pair of **bolt cutters** to its existing
   supplies/lore — needed back at the Bullpen.
7. **Property & Evidence Room** (bolt cutters): a real evidence-storage room at the station,
   containing the **Evidence Room Key** (same item as before, same flavor text — the key itself
   was evidence "release pending" to the municipal court) plus optional loot.
8. **Municipal Garage** (secondary, now optional rather than load-bearing): keeps its existing
   supplies, mechanic's office note, and shortcut gate; the K-9 transport van/Hound fight is
   removed from here. Proposed small addition: Reyes' own patrol cruiser, door open, radio still
   crackling — parked here rather than at the K-9 room, implying he walked back into the station
   on foot to check the kennels and never returned to the car. A light connective breadcrumb, not
   a requirement.
9. **Courthouse** (secondary, optional): the Evidence Room Key now opens a renamed **Clerk's
   Exhibit Storage** room — a small room holding an active trial exhibit rather than long-term
   evidence, a distinct and realistic reason for a courthouse to have a locked, key-gated room at
   all — with the same ammo/medkit-tier reward as before. The jury deliberation room survivor-camp
   beat is unchanged.
10. **Breezeway.** The antique deadbolt into the old station house — previously bypassed by an
    exterior "pried boards" workaround — now requires the **Skeleton Key** from the Chief's Office
    (step 3) as the one real solution, removing the workaround entirely.
11. **Old Station House** (Main Hall + Holding Cells) — unchanged: the Authority Crest and the
    damaged founders' document, reached only after the loop above.

Net effect: the **main station building** now contains Lobby, Bullpen, Records/Dispatch, Chief's
Office, K-9 Unit Room, Property & Evidence Room, Armory, Breezeway, Old Station Main Hall, and
Holding Cells — ten distinct areas carrying real exploration/combat weight, matching the "2–3
hours, hotel-comparable" bar. The three secondary locations are now lighter, more clearly optional
supply/lore stops (Fire Station load-bearing for bolt cutters; Garage and Courthouse worthwhile but
not gating), which is a more honest split than forcing all four buildings to be equally load-
bearing.

**Implementation notes:** `Scripts/Chapter_2_Ravenwood.md` (then Scenes 22–36) were rewritten in
full to match this plan exactly, with one new character added along the way — **Corporal Eli
Reyes** (`Characters/Eli_Reyes.md`), the K-9 unit's handler, needed to justify why the armory key
and the Ashen Hound fight are found together in the same room. `Locations/Police_Station.md` was
rewritten in full to match. `Characters/Ruth_Calloway.md` was updated (she now gives the Chief's
Office key and the Reyes/K-9 lead, not the armory key directly). `Creatures/Ashen_Hound.md` was
updated to reflect the new K-9 Unit Room location, and its concept art
(`Assets/Reference/ashen_hound_concept.png`) was regenerated to show the indoor kennel-room setting
instead of the original outdoor impound lot, per the concept-art convention's own rule that art
should stay in sync with the prose it depicts. `CANON.md` was updated (Reyes added to Named
Characters Confirmed; the design standard's retroactive note updated from "needs expansion" to
"done"). Scene numbers cited above reflect the state at the time this restructure was written; see
the next entry for the current final numbering (Scenes 22–40).

- **Police Station: added missing "basic functioning rooms" + full blueprint (2026-08-13).** The
  project owner pointed out the rebuilt station still felt small for a real department — missing
  booking/processing, holding cells, and similar ordinary rooms — and asked for the room-
  connectivity flowcharts (per [`Locations/Ravenwood_Hotel.md`](Locations/Ravenwood_Hotel.md)'s
  precedent) to be built for this district too. Added four new scenes between the Armory and the
  Fire Station, renumbering everything after (**now Scenes 22–40**, up from 22–36):
  - **Break Room** (Scene 30, optional) — a small, deliberately quiet scene: Corporal Reyes' locker
    holds an old K-9 graduation photo of him with Diesel and Baxter, adding one more human beat to
    his death after the fact, plus a Medkit and ammunition.
  - **Booking & Processing** (Scene 31, optional) — fingerprint station, mugshot backdrop,
    personal-effects lockers; yields an optional pocketknife.
  - **The Interview Room** (Scene 32, optional) — a recorder holds an old interview about
    unsettling pre-outbreak animal behavior near North Ridge, deliberately cross-referencing the
    newspaper clipping already established at Downtown's library
    ([`Scripts/Chapter_2_Ravenwood.md`](Scripts/Chapter_2_Ravenwood.md), Scene 20) — filed and
    forgotten rather than acted on, reinforcing the game's running "early warning signs went
    nowhere" motif without pushing the Vanguard connection further than already locked.
  - **Modern Holding Cells** (Scene 33, optional) — one empty cell with a torn, discarded uniform
    shirt (unresolved on purpose); one cell holding a shambler safely behind bars, reusing the
    lobby's "visible but harmless" convention rather than inventing a new one.
  - None of the four gate the Authority Crest or any existing key item — all purely additive
    depth/atmosphere, consistent with how Fire Station/Garage/Courthouse were already optional.
  - Added a full **Blueprint (Room Connectivity)** section to `Locations/Police_Station.md`, five
    Mermaid diagrams matching [`Ravenwood_Hotel.md`](Locations/Ravenwood_Hotel.md)'s exact
    legend/shape/color convention (District Entry → Lobby → Bullpen; the Annex Core; the Booking
    Wing; Breezeway → Old Station House; the three Secondary Locations).

- **AI-generated portraits for remaining named characters (2026-08-13).** Following the uploaded
  Chapter 1 portrait batch, the project owner asked for portraits for the still-missing named
  characters and for this to become standard practice for all future characters too. Generated
  five, matching the uploaded set's pixel-art style via reference-image-guided generation:
  **Richard Dalton, Officer Dale Pruitt, Sergeant Ruth Calloway, Corporal Eli Reyes, and
  Fennimore.** The first attempt at Richard Dalton came out wrong (the reference image pull was too
  strong and it regenerated something close to Earl instead of a distinct younger character) and
  was redone with a more detailed, specific prompt. Dale Pruitt's and Eli Reyes' generations
  incidentally produced a plausible Ravenwood PD badge/patch design (star-in-shield "RAVENWOOD
  POLICE" badge, mountain-range shoulder patch, K-9 Unit patch) — kept as loose visual reference,
  not formally locked as the department's official insignia. Documented the full generation
  convention in [`Characters/README.md`](Characters/README.md) (filename pattern, style/reference-
  image guidance, and an explicit rule that "never seen alive on-screen" characters like Fennimore
  and Reyes can still get a portrait as an internal design tool). Every currently-written named
  character now has a reference portrait.
- **Portrait pipeline corrected (2026-08-13, same day).** The project owner clarified that the
  five portraits above (Richard, Dale, Ruth, Eli, Fennimore) needed to be redone — the *originally
  uploaded* portraits were already correct and didn't need touching. The project owner then
  provided the exact prompt template and confirmed settings (PixelLab.ai's "Create Image (Pro)"
  tool, 256×256 output) used to make the original uploads. Replaced all five: generated a clean
  semi-realistic "source" photo per character with the given template, then ran each through
  PixelLab's `create_image_pro` MCP tool (the same tool, confirmed) with that photo as a labelled
  reference. Two practical issues worked through, now documented in
  [`Characters/README.md`](Characters/README.md) for future use: (1) the reference-image base64
  payload truncates unpredictably above roughly 2–3 KB via this transport, so the source photo
  needs to be shrunk to ~40–48px/16–24 colors before sending, which loses enough detail that 2 of
  the first 5 attempts came back as unrelated generic people rather than the intended character;
  (2) retrying with a more explicit text description (spelling out hair, skin tone, and clothing
  rather than relying on the reference alone) fixed both failed attempts. All five final portraits
  replace the earlier generic-image-generator versions in place and now genuinely match the
  uploaded set's house style rather than approximating it.

- **Zombie Conglomerate ("the Zombie King") introduced + Hotel reference screenshots organized
  (2026-08-13).** The project owner uploaded a large asset batch to `DESIGN/Assets/` — most of it
  in-engine room mockups for the Ravenwood Hotel (exterior/parking lot, Manager's Office, Room 104,
  Dining Hall/Kitchen), plus concept art and an animation test for a new creature, "the Zombie
  King" — "think of it as a rat king... it rolls around the town randomly, first displays after you
  collect your first emblem."
  - **Hotel screenshots** were renamed from generic upload filenames to descriptive ones, sorted
    into `Assets/Screenshots/`, and embedded directly in
    [`Locations/Ravenwood_Hotel.md`](Locations/Ravenwood_Hotel.md) at their matching rooms. These
    are genuine in-engine mockups (not concept sketches) and are now the most reliable art-style
    reference in the project. One new detail surfaced that wasn't in the original script — a
    circular fountain courtyard/walkway at the hotel's front entrance — flagged inline as additive
    rather than contradictory (a hotel plausibly has both a parking lot and a separate fountain
    drive), and a "E. Whitaker" desk nameplate in the Manager's Office, plausibly Earl's own desk
    but not confirmed in any script.
  - **The Zombie Conglomerate** ("ZK" in its own concept dossier — Vanguard's technical designation
    for "Zombie Conglomerate," which the write-up treats as a deliberate in-world coincidence with
    the player-facing nickname "the Zombie King," rather than a naming conflict) is a new,
    **unkillable, un-fightable roaming hazard** — a mass of dozens of fused infected bodies, closer
    to an environmental hazard than a combat encounter. Full writeup at
    [`Creatures/Zombie_Conglomerate.md`](Creatures/Zombie_Conglomerate.md).
  - **Flagged rather than silently imported:** the uploaded concept dossier includes a "Recorded
    Sightings" log spanning **Day 18 through Day 45**, which directly contradicts the locked
    one-night timeline (`CANON.md`: *"the entire game takes place over the course of one night"*).
    Proposed (not yet approved) resolution: treat that log as a **secret, Vanguard-internal**
    history — the creature existed and grew for weeks before Jim's arrival, but entirely within
    Vanguard's own containment, only becoming a public, citywide threat the same night as the main
    outbreak, when that containment fails along with everything else. This preserves nearly all of
    the dossier's flavor text (including its unsettling "we do not study it anymore, we survive it"
    Vanguard notes) while resolving the contradiction. The dossier's location names (e.g. "St.
    Michael Church") don't match the game's actual five districts and should be reconciled if this
    material is ever written into an actual found document in-game.
  - **Not yet integrated as an actual scripted encounter** — `Creatures/Zombie_Conglomerate.md`
    proposes a first-appearance size (Stage 3, "Consumption," blocking a street/pathway) and a
    design intent (never fightable, forces detours/avoidance during open-world city exploration),
    but this needs approval before being written into `Scripts/Chapter_2_Ravenwood.md`.
  - Updated `CANON.md` (new "Apex Mutation" classification), `Creatures/README.md`,
    `MASTER_STORY.md`, and `Assets/README.md` to reference it.
  - **Room concept art started (same day).** Per the project owner's request ("generate room
    concepts for each scene, how that room should look, at least the general idea"), documented a
    new "room concept art" convention in `Assets/README.md` using the uploaded Hotel screenshots as
    the definitive style anchor, and generated a first batch covering the Police Station's most
    narratively significant rooms: the Bullpen, the Chief's Office, the K-9 Unit Room, and the Old
    Station House main hall. Two generation issues came up and are worth remembering for future
    batches: (1) the Chief's Office concept unprompted invented a "CHIEF E. WHITAKER" desk
    nameplate, almost certainly echoing the "E. Whitaker" nameplate visible in the Hotel's Manager's
    Office reference screenshot used as a style guide — flagged as non-canonical rather than a
    hint; (2) the first attempt at the Old Station House main hall rendered the emblem as a
    triangle/pyramid and invented eight unrelated chief names, both contradicting the already-
    locked wedge-shaped Authority Crest and Marshal Josiah Hale specifically — this was
    regenerated with a much more constrained prompt (explicit shape description, explicit
    instruction to keep the photo wall illegible/generic) and came out correct. **This is the start
    of an ongoing pass, not a complete sweep** — the remaining Police Station rooms and all of
    Chapter 1/2's other locations still don't have concept art and should be generated
    incrementally going forward, prioritizing narratively significant rooms first per the new
    convention.
  - **Concept/portrait rendering made a permanent rule (2026-08-13, same day).** Per the project
    owner's explicit instruction, this is no longer a case-by-case request: *any* new scene/room,
    new enemy/creature, or new named character now gets a matching concept render or portrait as
    part of finishing it, in the established house style, so animators/artists always have
    something concrete to work from. Codified as rule 16 in [`README.md`](README.md) → "Visual
    Asset Pipeline," with pointers into the three convention sections (`Assets/README.md` ×2,
    `Characters/README.md`) that hold the actual style/technical details.
  - **Chapter 1 Hotel room concept sweep (2026-08-13, same day).** Generated the ten remaining
    Hotel rooms of real narrative weight that didn't already have a real in-engine screenshot:
    the Lobby, Room 106 (Cindy), the Hotel Courtyard, the Red Room (Della Marsh), the Laundry Room
    (Gerta's death), the Housekeeping Closet (Gate Crank Handle), the Main Bar, the Utility Room
    (screwdriver), the Courtyard Security Office, and the West Wing Maintenance Room (auxiliary
    fuse) — all style-anchored to the real uploaded screenshots per the room concept art
    convention. All embedded in `Locations/Ravenwood_Hotel.md` at their matching rooms. One
    flagged issue: the Housekeeping Closet render put a "305" door number on the closet door,
    which doesn't fit its canonical location (guest floor, between Rooms 114/116, not a numbered
    room on a third floor) — noted inline as non-canonical rather than silently accepted. Remaining
    Chapter 1 rooms without concept art are all minor pass-through/atmosphere spaces (Pantry,
    Walk-in Freezer, East Wing Maintenance Closet, Lounge/Recreation, Piano Area, Liquor Storage,
    Boiler Room, Staff Room/Storage, the public stairwells) — deliberately deprioritized per the
    convention's "narrative weight over minor pass-through spaces" guidance rather than skipped by
    oversight.
  - **Police Station room concept sweep completed (2026-08-13, same day).** Generated the twelve
    remaining Police Station rooms, completing full concept-art coverage for the district: the
    Lobby, Records/Dispatch, the Armory, the Property & Evidence Room, the three secondary
    locations (Fire Station, Municipal Garage, City Courthouse), the Break Room, Booking &
    Processing, the Interview Room, the Modern Holding Cells, and the Old Holding Cells — all
    style-anchored to the earlier Police Station renders (Bullpen / Chief's Office / K-9 Room /
    Old Main Hall). All embedded in `Locations/Police_Station.md`. Three flagged generation
    errors, none promoted to canon: Records/Dispatch invented an unrelated "DET. HARRIS"
    nameplate; the Break Room labeled Corporal Reyes' locker "K. HARRISON" instead of "E. REYES";
    the Municipal Garage's wall sign reads "CITY OF RAVENCROFT" instead of the locked city name
    Ravenwood. Every room in both the Ravenwood Hotel and the Police Station now has either a real
    in-engine screenshot or AI concept art, except the Hotel's deliberately-deprioritized minor
    pass-through spaces noted above.

## Still-Open Questions

- **Exact cause/mechanism of the Black Vein outbreak** — the *attribution* (Vanguard BioSystems /
  Project Ashen) is locked, but *how* containment failed and *why now* are not yet written.
  Reserved for Chapter 3.
- **Cindy Sweets' fate** after her Room 106 abduction — her abductor is now identified (**The
  Maw** — see below), but what actually happened to her (alive / dead / turned / something else)
  remains explicitly undecided per the project owner. Do not infer a resolution from the Gerta
  reveal — they are two separate open/closed questions. **Update (2026-08-13):** Chapter 2's
  opening street crossing adds a blood trail and her torn, empty robe near Memorial Park's south
  gate (see [`Scripts/Chapter_2_Ravenwood.md`](Scripts/Chapter_2_Ravenwood.md), Scene 3) —
  deliberately more dread, not a resolution. Still no body, still nothing confirming alive, dead,
  or turned.
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

- The four remaining districts (Hospital, Academy, Refinery, Monastery) are planned in
  outline/secondary-location form (above) but **not yet scripted scene-by-scene**. The Police
  Station (Southwest/Authority) is now fully scripted — see the Direction Log entry below and
  [`Scripts/Chapter_2_Ravenwood.md`](Scripts/Chapter_2_Ravenwood.md), Scenes 22–33.
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
