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
- **Room concept art style correction, take one — wrong diagnosis, reverted (2026-08-13, same
  day).** Project owner feedback: "Make sure all room concepts follow the in game screenshots. Some
  don't." Misread the real in-engine `Assets/Screenshots/` references as a *flat, directly-overhead*
  retro-RPG style and "corrected" `hotel_courtyard_concept.png`, `hotel_red_room_concept.png`, and
  all 16 Police Station room concepts to match that (wrong) reading, overwriting all 18 files.
  Immediate follow-up feedback: "2.5d room not flat, look at the uploaded screenshots. The older
  renders looked better than these new ones." Re-examined the screenshots (e.g.
  `ravenwood_hotel_room104_bedroom_a.webp`, `ravenwood_hotel_exterior_fountain_entrance.webp`) and
  confirmed they're actually **2.5D / isometric-leaning** — an elevated three-quarter angle showing
  the fronts of furniture, walls, and building facades, not a strict top-down view of rooftops/floor
  only. The *original* pre-"fix" renders had this right all along; the "fix" was the actual
  regression. Reverted all 18 files to their pre-"fix" versions (`git checkout` from the commits
  before the flat re-render) and reverted the matching captions in `Locations/Ravenwood_Hotel.md` and
  `Locations/Police_Station.md` back to their original text. This also brought back the three
  non-canonical details those "fixed" renders had incidentally corrected (Records/Dispatch's
  invented "DET. HARRIS" nameplate, the Break Room locker's wrong name, and the Municipal Garage
  sign's wrong city name) — restored their original flagged-error captions rather than silently
  losing that context.
- **Room concept art style correction, take two (2026-08-13, same day).** Further feedback: "Only
  like 2 maps didn't render right off the old." Reviewed all 18 reverted files side-by-side and found
  the actual outliers: `police_station_armory_concept.png` and
  `police_station_interview_room_concept.png` had rendered in a flat vector-cartoon look (thick black
  outlines, no pixel-art grain, flatter shading) that doesn't match the painterly 2.5D pixel-art
  style every other room concept (and the real screenshots) uses. Regenerated only those two, using
  an existing correctly-styled render (`police_station_booking_concept.png`) plus a real Hotel
  screenshot as style anchors, and updated their captions in `Locations/Police_Station.md`. The other
  16 reverted files were left as-is — already correct. Lesson for future room concept generation:
  the house style is 2.5D/isometric-leaning with visible object fronts, not flat top-down — see the
  (already-correct) description in [`Assets/README.md`](Assets/README.md) → "Convention: room
  concept art."
- **Room concept art style correction, take three (2026-08-13, later the same day).** The take-two
  regenerations of `police_station_armory_concept.png` and `police_station_interview_room_concept.png`
  ("v3") still hadn't actually fixed the flat vector-cartoon problem — closer inspection found they
  still had thick black outlines and flat cel-shading instead of the painterly pixel-art grain every
  other room concept uses. Regenerated both a second time ("v4"), this time anchored directly to a
  real Hotel screenshot (`ravenwood_hotel_dining_hall.png`) plus a known-good Police Station room
  concept, with an explicit prompt instruction rejecting the flat vector-cartoon look. Copied the v4
  renders over the existing files and updated their captions in
  [`Locations/Police_Station.md`](Locations/Police_Station.md) to record the full two-attempt history.
- **Room concept art style correction, take four — attempted and rejected (2026-08-13, later
  still).** Independently, side-by-side comparison of every remaining room concept against the real
  in-engine screenshots (`ravenwood_hotel_kitchen_full.png`, `ravenwood_hotel_dining_hall.png`) turned
  up what looked like a genuine camera-angle inconsistency: `police_station_modern_cells_concept.png`,
  `police_station_courthouse_concept.png`, and `hotel_red_room_concept.png` all use a tilted/rotated,
  corner-of-the-room isometric framing, while the real screenshots show a strictly flat single back
  wall with a straight horizontal top edge. Regenerated all three to that strict flat-back-wall
  framing (new v2s of all three). Immediate project-owner feedback: "Those r flat the old are
  better." Reverted `police_station_modern_cells_concept.png` and
  `police_station_courthouse_concept.png` to their pre-attempt versions via `git restore`, and
  discarded the `hotel_red_room_concept_v2.png` file before it was ever deployed into
  [`Ravenwood_Hotel.md`](Locations/Ravenwood_Hotel.md) (the original `hotel_red_room_concept.png` was
  never actually changed). **Lesson — now confirmed a second time, independently of take one's
  identical finding:** the project's real house style for concept art is 2.5D/isometric-leaning,
  including a tilted corner-of-the-room framing for some rooms, even though the actual in-engine
  gameplay screenshots use a flatter single-wall framing. Concept art is not required to exactly copy
  the gameplay camera's framing — it should stay in the general painterly 2.5D pixel-art *style*
  (grain, palette, prop density, three-quarter object fronts), not be forced into a flat top-down
  layout. Do not attempt another "flatten the camera" pass on any room concept without new, explicit
  direction from the project owner.
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

- **Maw sprite reference uploaded — discrepancy flagged, not resolved (2026-08-13).** The project
  owner uploaded (inline in chat only, not as a real file) an image described as "the Maw sprite": a
  small, in-game-scale pixel-art sprite sheet of a generic-looking crouched grey humanoid, repeated
  seven times. It does not show the Maw's locked defining mutation (the torso splitting into a
  vertical, tooth-lined mouth) at all — it reads much closer to the [Shambler](Creatures/Shambler.md)'s
  design than the Maw's. Documented and flagged in [`Creatures/The_Maw.md`](Creatures/The_Maw.md) →
  "Open Design Gaps" rather than silently used to rewrite the Maw's Appearance section or silently
  ignored. **Needs an explicit decision from the project owner**: is this genuinely meant to be the
  Maw's in-game sprite (requiring a real revision to the locked Appearance section), or was it
  intended for a different creature? Left open pending that answer.
- **Unnamed Hospital boss proposed (2026-08-13).** The project owner uploaded (inline in chat only,
  same file-access limitation as above) a five-pose concept sheet and a photo of an unrelated
  third-party 3D-printed sculpture ("Biocreator" by Bogdan Stepanenko, shared for silhouette/pose
  reference only) depicting a new, explicitly **unnamed** boss creature intended for the not-yet-
  written Hospital chapter: a hulking, aged-faced mutant, one arm overgrown into an enormous clawed
  hand it perches/lunges on, carrying an oversized syringe in its other hand. Created
  [`Creatures/Unnamed_Hospital_Boss.md`](Creatures/Unnamed_Hospital_Boss.md) describing both uploaded
  images in full (since they couldn't be saved directly) and generated a fresh in-house-style concept
  render (`Assets/Reference/hospital_unnamed_boss_concept.png`) reconstructing the design rather than
  copying either reference image directly. Added a forward-reference note plus a Boss Encounters
  entry to [`Locations/Hospital.md`](Locations/Hospital.md), which otherwise remains fully `_TBD_`.
  Explicitly a proposal pending review, not locked canon — still needs a name, an origin story, a
  full combat kit, and the rest of the Hospital chapter written around it before it's more than a
  design placeholder.
- **Red Room / Main Bar / Security Office / Courtyard render fixes (2026-08-13).** Project owner
  feedback: these four specific renders had "the wrong perspective," "a door where there shouldn't
  be," or otherwise "did not render correctly" — distinct from the take-four framing question above
  (the *style* was fine, specific content/composition wasn't). Regenerated all four:
  `hotel_red_room_concept.png` (v3, flat-back-wall framing, and a backstage sign typo — "The Red
  Roam" — flagged, not fixed, since it's cosmetic AI text-rendering noise rather than a canon
  detail), `hotel_main_bar_concept.png` (v2, removed an unscripted door behind the bar), and
  `hotel_security_office_concept.png` (v2, replaced a too-tight desk/monitor crop with a full-room
  view). `hotel_courtyard_concept.png` (v2) was independently already regenerated the same day for
  an unrelated rooftop-angle issue (see the take-four entry above) — no further change needed here.
  Updated captions in [`Locations/Ravenwood_Hotel.md`](Locations/Ravenwood_Hotel.md) to record each
  fix.
- **Full room/hallway gap-fill sweep — Hotel and Police Station (2026-08-13).** Project owner:
  after confirming "all the current concepts in the police station look damn near perfect," asked
  for an exhaustive pass across both locations, "even if it's just a hallway that connects to
  another room," to make sure nothing was missing. This **supersedes the "deliberately
  deprioritized minor pass-through spaces" note above** — those spaces are no longer deprioritized;
  they're now covered. Cross-checked every node in both locations' Mermaid blueprint diagrams
  against `Assets/Reference/` and found real gaps beyond the ones already called out:
  - **Hotel (18 new renders across four batches):** Staff Hallway, Grand Staircase, East/West
    Hallway (the guest-floor corridors themselves, not just the rooms off them), Room 112, Room
    118, Rooms 114 & 116 (shown from the hallway, since their narrative purpose is staging the
    pincer ambush, not their interiors), East/West Public Stairwell, West Wing Service Corridor,
    Pantry, Walk-in Freezer, East Wing Maintenance Closet, Lounge/Recreation, Piano Area (blank on
    the first generation attempt — a plain retry with the same prompt succeeded), Liquor Storage,
    Boiler Room, Staff Room/Storage, and — the one genuine narrative-weight gap in the whole
    sweep — the **Maintenance Shed's interior**, the Caretaker boss fight's starting location,
    which had never gotten its own render despite the Caretaker himself and the courtyard exterior
    both already having one. All embedded in
    [`Locations/Ravenwood_Hotel.md`](Locations/Ravenwood_Hotel.md). Flagged inaccuracy: Room 118's
    concept embroiders a pillow "H&R," matching neither Dalton's initials.
  - **Police Station (3 new renders):** the Back Hallway (Bullpen → Break Room/K-9 Unit Room), the
    Booking Corridor (Bullpen → Booking/Interview Room/Modern Holding Cells), and the Breezeway
    (the annex → old station house transition itself, not just the rooms on either end) — all named
    as pill/connector nodes in the blueprint diagrams but never actually rendered. The Booking
    Corridor's first attempt drifted into the same flat vector-cartoon look flagged earlier for the
    Armory/Interview Room; regenerated once more, anchored to the Booking & Processing and Bullpen
    renders, before deploying. All embedded in
    [`Locations/Police_Station.md`](Locations/Police_Station.md).
  - Every room *and* named connector/hallway in both locations' blueprint diagrams now has either a
    real in-engine screenshot or AI concept art, with no remaining gaps.
- **Weapons and Items document — audit and folder buildout (2026-08-13).** Project owner uploaded
  [`Deadlock Weapons and Items.docx`](Deadlock%20Weapons%20and%20Items.docx) directly to the repo
  (pushed straight to `main`, per the new "main only" workflow rule) and asked for the same
  folder/file/concept-art treatment already used for `Characters/`, `Creatures/`, and `Locations/`.
  Read in full (13 entries: 11 weapons, 2 throwables) and built out new
  [`Weapons/`](Weapons/README.md) and [`Items/`](Items/README.md) folders, one file per
  weapon/item, transcribing each Description/Stats block verbatim. Cross-referenced every entry
  against already-scripted content rather than treating the new doc as a blank slate:
  - **Strong, flagged (not silently applied) matches:** the "Sentinel-9" Service Pistol's
    description (RPD-issue sidearm) matches Jim's already-established first firearm — "a handgun"
    taken from Officer Dale Pruitt, Chapter 1; the "Ranger 870" Pump Shotgun's description (rugged
    12-gauge, manual pump) matches the Police Station Armory's already-established shotgun reward,
    Chapter 2. Both are treated as **very likely** the same items, but neither existing script/
    location file actually names a model, so the connection is documented as a pending-approval
    proposal in each weapon's own "Story Placement" section rather than silently renaming "the
    handgun"/"the shotgun" everywhere they're mentioned.
  - **Confirmed exact match:** the "Roadwrecker" Aluminum Baseball Bat matches Jim's already-
    established first weapon (grabbed from wrecked lobby furniture, Chapter 1) closely enough
    (baseball bat, no other candidate) to link directly without the same hedging.
  - **Plausible future placement, not locked:** the "Steelstorm M60" LMG's description ("salvaged
    from a Steelgate factory security cache") lines up with the Northwest/Refinery district's
    planned secondary location, the **Steelgate Loading Docks** (see `MASTER_STORY.md` → "Secondary
    Locations") — noted as a good fit for whoever writes that district, not a decision made here.
  - **No placement yet, by design:** the Vanguard M-15 AR Platform, Ironback .357 Revolver,
    Longview .308 Sniper Rifle, Cleaverborn Survival Sword, Thunderlance Railgun, CRN-09 Decimator
    Beam, Titanbreaker RLR-7 Rocket Launcher, Molotov Cocktail, and Pipe Bomb have no scripted
    pickup location anywhere yet — expected, since only two chapters (Hotel, Police Station) are
    written. Documented as available inventory for future chapters rather than force-placed.
  - **Minor doc-structure note:** the source docx's "🧪 Vanguard Experimental Prototype Set"
    heading appears in the raw text *after* the Thunderlance Railgun's own entry, even though the
    Railgun's flavor text ("A Vanguard anti-bio-weapon prototype...") clearly belongs to that set
    alongside the CRN-09 Decimator Beam. Treated as a loose paragraph-ordering artifact in the
    original document, not a content contradiction — grouped both under "Vanguard Experimental
    Prototype Set" in [`Weapons/README.md`](Weapons/README.md)'s file list.
- **In-game item icon references uploaded — style correction before any renders were made
  (2026-08-13).** Immediately after the folder buildout above, and before generating any weapon/
  item concept art, the project owner uploaded eight actual in-game item-icon sprites (inline in
  chat only, same file-access limitation as previous inline uploads — not saved directly into this
  repo) specifically to correct the reference style. Described here since they couldn't be saved as
  files: three black, simple, mostly-monochrome firearm silhouette icons (a compact SMG/rifle held
  at a slight angle, a handgun, and a longer shotgun/carbine); two dark maroon/red elongated
  melee-weapon-shaped icons (differing slightly in silhouette from each other); one small
  red-orange round icon; one tan/khaki soft pouch-or-bag icon; and one gray metal box with a
  handle (toolbox/case silhouette). All are small, flat-shaded, simple pixel-art **inventory
  icons** — much closer to the existing `Assets/Reference/vern_terminal_icon.gif` than to the
  painterly digital-concept-art style used for room and creature renders. **Corrected the
  `Weapons/README.md` and `Items/README.md` concept-art conventions to this icon style before any
  weapon/item renders were generated**, avoiding the same mistake made earlier with room concepts
  (see the "Room concept art style correction" entries above) — this time the style reference
  arrived before generation started, not after.
- **Real weapon/item sprites uploaded — 15 files (2026-08-13).** The project owner pushed 15 actual
  in-game sprites directly into `Weapons/` and `Items/` (not inline-chat images this time — real
  committed files, so no description-only workaround was needed): `spr_handgun.png`,
  `spr_shotgun.png`, `spr_AR15.png`, `spr_baseballBat.gif` (weapons — matching four of the eleven
  catalogued weapons) and `spr_medkit.png`, `spr_smallMedKit.png`, `spr_handgunAmmo.png`,
  `spr_shotgunAmmo.png`, `spr_riffle ammo.png`, `spr_screwDriver.png`, `spr_managerKey.png`,
  `spr_MaitenanceKey.png`, `spr_graveyardKey.png`, `spr_keycard.png`, `spr_fuseItem.gif` (items —
  mostly location-specific key items already documented per-location, e.g. the Manager's Key and
  screwdriver from `Locations/Ravenwood_Hotel.md`, plus two new items not yet documented anywhere:
  a graveyard key and a keycard). Embedded the four weapon sprites directly into their matching
  `Weapons/` files (confirmed real assets, replacing the "no concept art yet" gap). The item
  sprites are not yet individually catalogued as `Items/` files or cross-linked to their existing
  `Locations/` mentions — flagged as a follow-up, not done in the same pass as the naming
  discussion below.
- **Weapon naming convention — settled after three iterations (2026-08-13).** The project owner
  asked whether to drop the source document's invented brand nicknames (e.g. "Sentinel-9,"
  "Ranger 870") in favor of plain model numbers. This went through several rounds before landing:
  1. **First pass:** assumed the uploaded sprite filenames (`spr_handgun.png`, `spr_shotgun.png`,
     `spr_AR15.png`, `spr_baseballBat.gif`) reflected the actual in-fiction naming convention (fully
     generic: "Handgun," "Shotgun," "AR-15," "Baseball Bat") and renamed all 11 weapon files to
     match, demoting the original nicknames to an "AKA" note. **Wrong premise** — the project owner
     clarified the sprite filenames are just generic asset-pipeline names, not meaningful in-fiction
     names.
  2. **Second pass:** the project owner then said plain-generic names alone felt too bare and asked
     for "at least a model number." Renamed again to "model number + generic type" (e.g. "M9
     Handgun," "870 Shotgun"), inventing plausible numbers for weapons that had none in the source
     document (e.g. an invented "XL-3" for the baseball bat, "SK-5" for the survival sword).
  3. **Third pass — corrected further:** the project owner supplied real calibers (9mm pistol,
     12-gauge shotgun, 5.56mm AR) and clarified two things: caliber shouldn't be *in* the displayed
     name (it's lore/stat detail, not a title element), and weapon names should either match the
     source document exactly or use an actual real-world firearm model — not an invented
     placeholder number. Renamed a third time to real-world manufacturer+model names (Beretta M9,
     Remington 870, Colt Python, Remington 700), dropping the source document's nicknames entirely
     for the six standard firearms.
  4. **Final, settled decision:** the project owner referenced Resident Evil's "Samurai Edge" — an
     in-universe custom name for what's functionally a modified Beretta 92FS — as the model to
     follow. **This is the deciding precedent:** the real-world gun is the *basis* for a weapon's
     feel/flavor, not its displayed name. Reverted a final time to the **source document's own
     in-universe names as the primary name for every weapon** (all 11 filenames and headers back to
     their original form), with a **"Real-World Basis" note** added to each of the six standard
     firearms (Beretta M9 for the Sentinel-9, Remington 870 for the Ranger 870, AR-15 platform for
     the Vanguard M-15, Colt Python-style for the Ironback .357, M60 for the Steelstorm M60,
     Remington 700-style for the Longview .308) purely as flavor/grounding detail, and a **Caliber**
     row added to each one's Stats table (9mm, 12-gauge, 5.56mm, .357 Magnum, .308 Winchester) so
     the caliber is recorded as data, not baked into the title. The five weapons with no real-world
     analog (Roadwrecker Baseball Bat, Cleaverborn Survival Sword, Thunderlance Railgun, CRN-09
     Decimator Beam, Titanbreaker RLR-7 Rocket Launcher) simply keep their document names outright,
     with a short note confirming why no real-world substitution applies to them.
  - **Lesson for future naming decisions:** don't over-rotate on a single new data point (like an
    asset filename) without confirming it's actually meaningful — ask or wait for confirmation
    before a full rename pass, since three of the four rename passes here turned out to be
    unnecessary churn once the full picture (calibers, the Samurai Edge precedent) was in.
- **Three weapon placements confirmed; one material contradiction caught and fixed (2026-08-13).**
  The project owner confirmed explicitly: the Sentinel-9 Service Pistol *is* Jim's handgun from
  Officer Pruitt (Chapter 1); the Ranger 870 Pump Shotgun *is* the Police Station Armory's shotgun
  (Chapter 2); and the Roadwrecker Baseball Bat *is* Jim's bat from the wrecked lobby furniture
  (Chapter 1) — upgrading all three "Story Placement" sections from hedged proposals to confirmed
  facts, and adding named cross-links from `Locations/Ravenwood_Hotel.md`,
  `Locations/Police_Station.md`, and `Characters/Dale_Pruitt.md` back to their `Weapons/` files.
  In the process, caught a real contradiction: the source weapons document calls the bat an
  "Aluminum Baseball Bat," but the already-locked
  [`Scripts/Chapter_1_One_Night_Only.md`](Scripts/Chapter_1_One_Night_Only.md) (Scene 22)
  specifically describes "the smooth worn wood of a baseball bat." Per the project owner, the
  locked script wins — corrected `Roadwrecker_Baseball_Bat.md` to describe a wooden bat (dropping
  "Aluminum" from the title/Description; stats unchanged). The locked script prose itself was left
  untouched (still says "a baseball bat" / "the handgun" / "the shotgun" generically) per the
  project's "preserve existing material unless a rewrite is requested" rule — only the
  higher-level `Locations/`/`Characters/`/`Weapons/` docs got the specific names.
- **Concept art generated for the remaining 7 weapons (2026-08-13).** Generated inventory-icon
  concepts for the Ironback .357 Revolver, Steelstorm M60, Longview .308 Sniper Rifle, Cleaverborn
  Survival Sword, Thunderlance Railgun, CRN-09 Decimator Beam, and Titanbreaker RLR-7 Rocket
  Launcher, style-anchored to the four real uploaded sprites. The Cleaverborn Survival Sword's
  first two generation attempts both failed (HTTP 400, likely a content-safety trip on "machete"
  phrasing combined with the baseball-bat sprite as a reference image); succeeded on a third
  attempt after rephrasing to "camping machete-style tool" and dropping the reference image.
  **Every weapon in [`Weapons/`](Weapons/README.md) now has concept art** — four real sprites, and
  seven AI-generated icons.
- **Items folder audit and Consumables/Key_Items split (2026-08-13).** Project owner asked for the
  same folder/file/concept-art treatment for `Items/`, and clarified an important design fact
  first: the physical-key and keycard sprites were **designed to be reused across multiple
  different key items**, not as unique art per named key — so a shared icon between two items
  doesn't mean they're the same item. Restructured `Items/` into two subfolders,
  [`Consumables/`](Items/Consumables/README.md) and [`Key_Items/`](Items/Key_Items/README.md), and
  audited every item already established across `Locations/Ravenwood_Hotel.md`,
  `Locations/Police_Station.md`, and `Locations/Memorial_Park.md` (not just the ones with a real
  uploaded sprite), giving each its own file:
  - **Consumables (7):** Medkit, Small Medkit (a visually distinct second healing-item sprite with
    no established mechanical difference from Medkit yet — flagged as an open design gap, not
    resolved), Handgun Ammunition, Shotgun Shells, Rifle Ammo (for the not-yet-placed Vanguard
    M-15 — matches that weapon's own "not yet placed" status), and the two existing throwables
    (Molotov Cocktail, Pipe Bomb), moved into the new subfolder.
  - **Key Items (13):** every key/tool/unique object already named in the Hotel's, Police
    Station's, and Memorial Park's "Key Items" sections — Manager's Key, Housekeeping Closet Key,
    Gate Crank Handle, Screwdriver, Auxiliary Fuse (Hotel); Chief's Office Key, Old Station
    Skeleton Key, Armory Key, Evidence Room Key, Bolt Cutters, Pocketknife, Authority Crest
    (Police Station); Bollard Override Keycard (Memorial Park). Four of these (Gate Crank Handle,
    Bolt Cutters, Pocketknife, Authority Crest) had no real sprite, so got a new AI-generated icon
    each, matching the weapon-icon style; the rest reuse the real uploaded key/keycard sprites per
    the reuse note above — `spr_managerKey.png`, `spr_maintenanceKey.png` (typo-corrected from
    `spr_MaitenanceKey.png`), and `spr_graveyardKey.png` are distributed arbitrarily across the
    plain "key" items (Manager's Key, Armory Key get one; Chief's Office Key, Evidence Room Key,
    Old Station Skeleton Key get another) with an explicit note in each file that this is a
    cosmetic assignment, not a canon fact.
  - **Confirmed exact match:** `spr_keycard.png`'s flavor (orange/white laminated card) and the
    already-scripted "Ravenwood Emergency Management keycard" / "BOLLARD OVERRIDE KEYCARD" item
    (Memorial Park guardhouse, `Scripts/Chapter_2_Ravenwood.md` Scene 8) are unambiguously the same
    item — no hedging needed, unlike the weapon placements.
  - Added cross-links back from `Locations/Ravenwood_Hotel.md`, `Locations/Police_Station.md`, and
    `Locations/Memorial_Park.md`'s existing "Key Items" prose to each new `Items/` file, the same
    pattern used for the confirmed weapon placements above.
  - **Not included in this pass:** the various in-fiction *documents* already tracked in each
    location's own "Documents" section (guest ledger, incident reports, maintenance logs, etc.) —
    those are lore text, not inventory items, and stay where they are rather than getting `Items/`
    files.
- **Vanguard's Grip on Ravenwood PD — a deeper reframe of the Police Station (2026-08-13).** The
  project owner supplied substantial older design material reframing the district: the officers
  aren't secretly Vanguard villains — they're real Ravenwood cops who believe they're protecting
  their town while Vanguard spent years quietly turning the department into an unofficial
  containment arm around them, most of them never fully realizing how far they'd already crossed
  the line. Explicitly asked to use judgment on how much this should expand the location, "trying
  to give it more depth" — treated as approval to actually integrate it, not just log it as a
  brainstorm. A follow-up clarified the key structural detail before any rooms were built: Vanguard
  has an office *inside* the station (the Liaison Program), but actual containment happens
  off-site, at the hidden underground facility already established in
  [`Locations/Vanguard_Facility.md`](Locations/Vanguard_Facility.md) (Chapter 3's Project Ashen
  reveal) — the station's basement holding area is a transfer point, not the destination.
  - **Added to [`CANON.md`](CANON.md)** as a new "Vanguard's Grip on Ravenwood PD" section (world
    lore bigger than just this one district): the Ravenwood–Vanguard Public Safety Agreement
    (funding that created dependency without technical ownership), the Vanguard Public Safety
    Liaison Program, V-CASE classification (the cover story given to officers, and the actual
    isolate/restrain/surrender-to-Vanguard/seal-footage procedure), the confidential watchlist and
    its traffic-stop radio code convention, Vanguard's hidden interrogation-room experiments, and
    the "town as a field study" thread — offered as a strong *contributing* factor toward the
    already-flagged-open "how containment failed / why now" question, explicitly not a full
    answer, since that's reserved for Chapter 3.
  - **New character: [`Characters/Aaron_Cole.md`](Characters/Aaron_Cole.md)** — a detective who
    connected a string of local disappearances to Vanguard's V-CASE program, got discredited via a
    fabricated internal-affairs case once Vanguard noticed, and disappeared *before* the outbreak
    (a deliberately older wound than Fennimore's or Corporal Reyes' outbreak-night deaths — signals
    the corruption predates Black Vein escaping containment). Never seen alive or dead; reconstructed
    entirely through his abandoned office and hidden investigation, per the game's established
    "environmental discovery, not exposition" convention. Got a reference portrait via the standard
    two-step PixelLab pipeline (generic/unremarkable appearance, since nothing about his looks was
    otherwise established).
  - **Four new optional rooms in [`Locations/Police_Station.md`](Locations/Police_Station.md)**,
    added as a parallel discovery track that does **not** gate the Authority Crest or any part of
    the mandatory critical path: Detective Cole's Office (unlocked; hidden investigation +
    Vanguard Access Card), the Vanguard Liaison Office (corporate furniture starkly out of place;
    the V-CASE protocol binder and confidential watchlist), the Cold Cells (Vanguard's renovated
    basement holding area), and the Vanguard Observation Booth (the hidden other side of the
    Interview Room's one-way glass). All four gated behind a single new key item, the
    [Vanguard Access Card](Items/Key_Items/Vanguard_Access_Card.md) — a deliberate "one key opens
    a whole hidden layer" design, distinct from the main critical path's one-key-per-door
    convention, meant to land as a gut-punch once the player realizes how much of the station
    Vanguard could already move through freely. Blueprint updated: new nodes in the Annex Core and
    Booking Wing diagrams, plus a new Diagram 5 for the Basement/Cold Cells (the old Diagram 5,
    Secondary Locations, renumbered to Diagram 6) — all four new rooms use a new purple "Vanguard"
    node color, visually distinct on purpose.
  - Generated four new room concepts and one new item icon; the Vanguard Liaison Office's render
    got its own wall "V" emblem, which the location file explicitly notes is a deliberate echo of
    the Founders Memorial's own weathered "V" rather than a coincidence introduced by the
    generator.
  - Added a small cross-reference to
    [`Characters/Ruth_Calloway.md`](Characters/Ruth_Calloway.md) flagging a possible (not yet
    scripted) restrained dialogue hook about Cole/the Cold Cells, kept deliberately minor per the
    "environmental discovery" convention.
  - **Not done in this pass:** full scene-by-scene scripting into
    `Scripts/Chapter_2_Ravenwood.md` — everything above is at the location-design/prose level,
    matching the status of several other not-yet-fully-scripted beats already in that file (e.g.
    Calloway's alternate death scene). See `Locations/Police_Station.md` → "Unresolved Ideas" for
    the complete list of what's still open.
- **Outbreak Night — What Actually Happened: a full timeline for the department's collapse
  (2026-08-13).** The project owner supplied a detailed 15-beat outbreak-night timeline for the
  station, explicitly asking that it read as "a slow institutional collapse, not 'monsters attack
  the station and everyone dies'" — cops spending the first half of the night trying to do their
  jobs while Vanguard fed them bad orders, suppressed information, and prevented them from
  responding correctly, reconstructable almost entirely from radios, bodies, barricades, paperwork,
  and the environment itself by the time Jim arrives. Integrated as a new "Outbreak Night — What
  Actually Happened" section in [`Locations/Police_Station.md`](Locations/Police_Station.md),
  directly preceding "Arrival / Setup," summarizing all 15 beats (the V-CASE procedure's origin,
  the Cold Cells filling up, "Emergency Public Safety Directive 7," officers realizing Vanguard
  knows more than it's saying, the first rupture, the Chief's "essential containment asset" call,
  officers disobeying Vanguard, the Highway 13 confrontation, the station becoming a shelter, the
  Cold Cells' disaster, the Sally Port breach, internal breakdown, the Chief's final broadcast, and
  the final stand) as the master reference behind several new/updated in-room details:
  - **New room: the Sally Port** — the station's own attached vehicle bay (distinct from the
    separate Municipal Garage secondary location), added as the actual outbreak-night breach point:
    a half-lowered, jammed emergency shutter, a parked cruiser with its door left open, a dropped
    shotgun. Added to the Annex Core blueprint diagram as a Bullpen branch; got its own AI-generated
    concept art (`police_station_sally_port_concept.png`), style-anchored to the Municipal Garage
    and Bullpen renders.
  - **New document, Bullpen:** the "SURVIVORS / MISSING / DECEASED" whiteboard, and a printed copy
    of "Emergency Public Safety Directive 7" (the Vanguard order to seal the town rather than
    evacuate it) pinned beside it.
  - **New document, Records/Dispatch:** the Chief's final broadcast — a recording of him publicly
    overriding Vanguard's containment order over the emergency network, ending on gunfire and
    static. His own ultimate fate stays deliberately unresolved either way, unchanged from before
    this addition.
  - **Cold Cells enrichment:** one cell door found bent outward from the inside; a second holds a
    handwritten note taped beside it — an officer's own words to someone he'd known his whole life,
    ending "Please don't let me turn into one of those things." This **resolves** the previously
    open question of whether the Cold Cells should hold a combat encounter: they don't — the room
    is meant to land as tragedy, not a fight.
  - **Vanguard Liaison Office enrichment:** the confidential watchlist now cross-references a name
    on the Bullpen's whiteboard, making explicit that Vanguard had flagged specific Ravenwood
    residents *months* before the outbreak, not discovered them that night.
  - **Exterior enrichment:** the wrecked patrol lot's damage now includes mixed RPD/Vanguard
    markings, the physical trace of the Highway 13 confrontation (kept as environmental evidence
    only, not a new playable location or scene — Highway 13 itself remains a fixed, non-interactive
    shot per Chapter 1's convention). A new arrival beat: a faint, intermittent police radio
    transmission ("...any officer... please respond...") audible before Jim ever opens a door,
    plus an explicit note that the station should read as very recent (flashing emergency lights,
    an idling cruiser, ringing phones), not decades-abandoned.
  - **Speculative connective thread, flagged not locked:** the timeline's step 7 (officers
    disobeying Vanguard, redirecting toward civilians, "one cruiser is dispatched toward the
    Ravenwood Hotel") is offered as a plausible explanation for Officer Dale Pruitt's cruiser
    crashing through the hotel's front doors in Chapter 1. Logged as an unresolved idea in both
    `Locations/Police_Station.md` and [`Characters/Dale_Pruitt.md`](Characters/Dale_Pruitt.md) —
    explicitly **not** a rewrite of the locked Chapter 1 script; Scene 41 (Pruitt's infected reveal)
    is unchanged.
  - **Not done in this pass:** full scene-by-scene scripting of these specific beats into
    `Scripts/Chapter_2_Ravenwood.md`; deciding the Chief's actual name (needed only if his final
    broadcast is ever voice-acted with a self-identification line); whether the Sally Port needs
    its own creature encounter (leaning no, consistent with the Cold Cells resolution, but not
    locked). See `Locations/Police_Station.md` → "Unresolved Ideas" for the complete list.

## Direction Log (continued) — Hospital chapter kickoff (2026-08-13)

- **The Broodling — new creature, then corrected against the real uploaded sprite.** The project
  owner described [Maria Dalton](Characters/Maria_Dalton.md)'s hospital fate: her unborn child is
  mutated by Black Vein into a creature (called "the Broodling") that emerges during childbirth,
  killing her; asked for concept art to follow and for "two new files" in the creatures folder.
  Created [`Creatures/Broodling.md`](Creatures/Broodling.md) from the text description alone
  first (guessed at a wrongly-shaped-infant appearance), generated an AI concept render to match.
  The project owner then uploaded the real in-game sprite directly (`spr_broodling.gif`,
  `spr_broodling_alt.gif`, two palette variants of the same 8-direction rotation set) — a small,
  emaciated, hunched *parasite*-type creature, closer to a crawling gremlin than an infant, with a
  wide tooth-filled mouth and reddened head/jaw markings. This **superseded** the text-only guess;
  the AI-generated placeholder render was deleted, and Appearance/Behavior were rewritten to match
  the real sprite. **The "two new files" request is still only partially resolved:** only one
  creature was ever described/uploaded (the Broodling); per the Della Marsh/Earl Whitaker/Officer
  Pruitt precedent (a named character who was alive on-screen before dying stays in `Characters/`,
  not a new `Creatures/` file), Maria's own death/birth scene was documented as an update to her
  existing [`Characters/Maria_Dalton.md`](Characters/Maria_Dalton.md) file instead of a second
  creature file. Flagged as an open interpretation in `Broodling.md` → "Open Design Gaps" rather
  than inventing a second creature to force the count to two.
- **The Hospital Boss — real reference art finally uploaded, correcting the AI reconstruction.**
  [`Creatures/Unnamed_Hospital_Boss.md`](Creatures/Unnamed_Hospital_Boss.md) was originally written
  from a *text description* of reference art the project owner had uploaded inline in chat (which
  never reached the repo as a real file, per the known file-access limitation), plus an AI-generated
  reconstruction render. The project owner has now uploaded the actual five-pose reference sheet
  directly (`Creatures/ref_hospital_boss_sheet.png`) and clarified two mechanical details the text
  description alone hadn't made clear: **the giant clawed hand is the creature's actual means of
  locomotion** (it rides the hand; the hand does the walking), not a perch it occasionally leans
  on, and it doubles as an attack; the other arm's weapon is **"a medical sort of tranquilizer
  gun,"** not a plain handheld syringe. Appearance/Behavior/Concept rewritten to match; the old
  AI-generated placeholder render (`Assets/Reference/hospital_unnamed_boss_concept.png`) deleted as
  superseded and, in places, inaccurate. Also proposed (not locked) a specific origin for this
  creature — the abdominal-trauma surgical patient described in
  [`Locations/Hospital.md`](Locations/Hospital.md) → "Outbreak Night" beat 15, whose organs kept
  malformed-regenerating no matter what the surgical team tried — and a staff nickname, **"The
  Surgeon,"** distinct from a confirmed real identity.
- **St. Dymphna Hospital — the Northeast district's main location, written in full (2026-08-13).**
  The project owner supplied a very detailed 20-beat outbreak-night account for the hospital,
  explicitly mirroring the Police Station's own timeline in tone and structure — institutions
  trying to do their jobs while Vanguard's contradictory orders and active obstruction made it
  impossible — distinguished thematically as *"Police Station: we followed orders until we
  realized they were killing the town. Hospital: we tried to save everyone until we realized
  Vanguard never wanted everyone saved."* Combined with the Maria/Richard Dalton fate (see above)
  and an explicit request that the two locations' records overlap directly (shared radio calls,
  shared officers, the same Highway 13 shutdown), [`Locations/Hospital.md`](Locations/Hospital.md)
  was rewritten from its original `_TBD_` placeholder into a full main-location file matching the
  Police Station's density, per [`CANON.md`](CANON.md) → "District Main-Location Design
  Standard":
  - **"Outbreak Night — What Actually Happened"** — a 20-beat timeline (first unexplained cases,
    Vanguard's hospital-specific V-CASE protocol, Vanguard quietly removing patients, the ER
    overflowing, the lab's independent "necrosis provokes regeneration" discovery, the Radiology
    transformation, staff hiding patients from Vanguard, the maternity-ward problem, the ~20-minute
    police/hospital cooperation window, Vanguard's remote biohazard lockdown, the Ambulance Bay
    firefight, the Surgical Wing horror that produces the boss creature, the zone-by-zone building
    collapse, the morgue's "one of these people isn't dead" reveal, the paired final transmission
    with the Police Station, the failed evacuation, and Vanguard's final act of cutting power to
    everywhere except its own areas) — mirroring
    [`Locations/Police_Station.md`](Locations/Police_Station.md)'s own timeline directly.
  - **Full room/blueprint build:** Ambulance Bay → Emergency Department (hub, gating the
    Laboratory, Administration, Surgical Wing, and the Psychiatric Ward) → Radiology → Laboratory
    → Administration → the Morgue (optional) → Surgical Wing (boss fight) → ICU → St. Dymphna
    Chapel (Medical Crest) → Maternity Ward → NICU → Psychiatric Ward (optional), plus three
    secondary locations (Medical Arts Building, Hospital Parking Structure, Vanguard Quarantine
    Checkpoint) pulled from the already-cross-validated city map. Six mermaid blueprint diagrams,
    same convention as the Hotel and Police Station.
  - **Richard Dalton's fate resolved as a new "Tier 2b" survivor mechanic** (see
    [`CANON.md`](CANON.md) → "Survivor System"): gated on *emblem count* (0–1 = alive, 2+ = dead)
    rather than strict visit order, the first variant on the existing Tier 2 rule. Maria Dalton's
    death is not conditional — only whether Richard survives to grieve it is.
  - **New creature, the Broodling**, and a corrected, art-verified rewrite of the previously
    text-only **Unnamed Hospital Boss** (now nicknamed "The Surgeon," with a proposed origin tying
    it directly to this timeline's Surgical Wing beat) — both logged in detail earlier in this
    same Direction Log entry, above.
  - **Direct crossover documents added to [`Locations/Police_Station.md`](Locations/Police_Station.md):**
    the "Unit Twelve, respond Ravenwood Memorial, violent patient, radiology" dispatch call, and a
    recorded RPD/Memorial radio exchange immediately preceding the Chief's final broadcast — both
    appear on both locations' "Documents" lists, satisfying the project owner's explicit request
    for the two locations' records to overlap.
  - **New founder named: Dr. Nathaniel Voss**, St. Dymphna Hospital's founding physician, keeper of
    the Medical Crest — added to [`CANON.md`](CANON.md) → "Named Characters Confirmed" alongside
    Marshal Josiah Hale, following the same period-appropriate-naming convention.
  - **15 new AI-generated room concepts** — full visual coverage for the entire new location in one
    pass, logged in [`Assets/README.md`](Assets/README.md). Several renders invented wrong
    hospital/founder names (echoing the same "generation invents a name" pattern seen throughout
    the Police Station's own concept art); flagged in each render's caption rather than adopted.
  - **Not done in this pass:** individual `Items/Key_Items/` writeups for this district's seven new
    key items (Fire Axe, Laboratory Key, Administration Key, Surgical Wing Access Card, Pry Bar,
    Chapel Key, Medical Crest) — flagged as the next natural pass once this location's overall
    shape is confirmed, matching how the Police Station's own `Items/` audit followed its location
    write-up rather than happening simultaneously. Also not done: scene-by-scene scripting into a
    `Scripts/` file (this location is at the same location-design/prose level the Police Station
    was at before its own scripting pass).

- **Steelgate Refinery — the Northwest district's main location, written in full (2026-08-13).**
  The project owner supplied a 22-beat outbreak-night account for the Foundry, explicitly framed
  as the *earliest* piece of the same shared night — *"the police station sees the consequences,
  the hospital receives the injured, but the Foundry is physically connected to the cave system
  containing Black Vein, making it the closest civilian-industrial site to the source"* — and
  distinguished thematically from both other locations: *"Police Station: Vanguard turned the
  people protecting Ravenwood into an extension of their containment system. Hospital: Vanguard
  turned Ravenwood's injured into research assets. Foundry: Vanguard turned Ravenwood's workers
  into long-term exposure subjects and built an entire industrial operation over the source."*
  [`Locations/Foundry_Refinery.md`](Locations/Foundry_Refinery.md) was rewritten from its original
  `_TBD_` placeholder into a full main-location file matching the Police Station and Hospital's
  density, per [`CANON.md`](CANON.md) → "District Main-Location Design Standard":
  - **"Outbreak Night — What Actually Happened"** — a 22-beat timeline (the Foundry's decades-long
    compromise and secret "EXPOSURE COHORT" occupational-surveillance program, the storm-night
    underground alarm and impact, the first injured workers surfacing, Vanguard's "DO NOT EVACUATE"
    order, the ambulance-transfer discrepancy, the nurse being told not to treat the injured, the
    restricted lower levels going silent, workers attempting to flee and being met with Vanguard
    rifles, Plant Manager Daniel Fitch's confrontation with the Vanguard liaison, the first full
    mutation, Vanguard arriving to secure research rather than rescue anyone, police growing
    suspicious, workers discovering the underground Vanguard facility and their own 12-year
    exposure files, Fitch's evacuation order, the lower containment seal failing, the Foundry's
    fragmentary warning to police, the citywide highway lockdown beginning as a direct consequence,
    some workers escaping into town, the plant's three-way internal fracture, Vanguard abandoning
    the site under the internal designation **"SITE LOSS ACCEPTABLE,"** and the final broadcast —
    *"They didn't find this thing tonight. They've been digging at it for years."*) — explicitly
    cross-referenced beat-by-beat against both [`Locations/Police_Station.md`](Locations/Police_Station.md)
    and [`Locations/Hospital.md`](Locations/Hospital.md)'s own timelines via a new "How the Three
    Outbreak Stories Connect" comparison table, per the project owner's explicit request that all
    three institutions feel like one continuous catastrophe.
  - **Full room/blueprint build:** Loading Yard → Casting Hall (hub, gating the Plant Manager's
    Office, the Vanguard Site Office, and the Restricted Elevator) → Foundry Clinic → Break Room →
    Manager's Office → Vanguard Site Office (needs a key from the secondary Loading Docks) →
    Restricted Elevator → Exposure Records Room → Research Bay → Security Checkpoint (needs a
    Cutting Torch from the secondary Machine Shops; this district's signature pack encounter) →
    Old Mine Workings (optional) → Founder's Boardroom (Industry Crest) → the Black Vein Cavern (a
    mandatory, non-combat climax reached only *after* the crest, not gating it), plus three
    secondary locations (Machine Shops, Loading Docks, Rail Yard) pulled from the already-
    cross-validated city map's own "tracks lead into the mountain — Black Vein's entry point"
    detail. Five mermaid blueprint diagrams, same convention as the Hotel, Police Station, and
    Hospital.
  - **New creature, proposed: the Exposure Cohort** — chronically, long-term exposed Foundry
    workers whose mutation is more "settled/adapted" than a standard Shambler's one-night
    transformation, filling the same structural role as the Ashen Hound pair and "The Surgeon" as
    this district's signature encounter. Unlike the Broodling and Hospital Boss, this one has **no
    real uploaded reference art** — a first-pass, unreviewed proposal built directly from the
    source material's own "EXPOSURE COHORTS" detail, flagged as more speculative than those two.
  - **New founder named: Elias Thorne**, Steelgate Refinery's founder, keeper of the Industry
    Crest — added to [`CANON.md`](CANON.md) → "Named Characters Confirmed" alongside Marshal
    Josiah Hale and Dr. Nathaniel Voss. **New named character: Plant Manager Daniel Fitch** — the
    Foundry's own Chief-equivalent, whose fate is deliberately left unresolved, same convention.
  - **New `CANON.md` addition: Black Vein is a natural cave-system formation**, not manufactured,
    with the 1887 Memorial Park facility as its original access point and a **second, later
    (1968) access point at the Foundry** — the two are explicitly *not* physically connected
    (Vanguard deliberately compartmentalized them), so nothing here provides a shortcut into
    Chapter 3's still-`_TBD_` facility. This resolves what could otherwise have been read as
    redundant with Chapter 3's own planned Black Vein reveal — the Foundry shows Jim the raw
    phenomenon itself as a mid-game gut-punch; Chapter 3 is reserved for the full facility and its
    complete history.
  - **Direct crossover documents added to both
    [`Locations/Police_Station.md`](Locations/Police_Station.md) and
    [`Locations/Hospital.md`](Locations/Hospital.md):** the Foundry/RPD dispatch exchange about
    additional ambulances, the fragmentary "Vanguard knew... the mine is the source" transmission
    (Police Station), and the Ambulance Three casualty-count mismatch plus an early unexplained
    industrial-trauma triage cluster (Hospital) — satisfying the project owner's explicit request
    that all three locations' records overlap directly.
  - **16 new AI-generated room concepts** — full visual coverage for the entire new location in one
    pass (13 main-plant/underground rooms plus 3 secondary locations), logged in
    [`Assets/README.md`](Assets/README.md), plus one new creature concept. Several renders repeated
    the same "Ravencroft" naming-generation error seen at the Police Station, the Manager's Office
    invented a wrong plant name/founding date, and the Founder's Boardroom invented five wrong
    portrait names instead of Elias Thorne — all flagged in each render's caption rather than
    adopted, plus one render (the Break Room) that visually carried over police-specific set
    dressing from its own style-reference image.
  - **Not done in this pass:** individual `Items/Key_Items/` writeups for this district's seven new
    key items (Manager's Office Key, Restricted Elevator Access Card, Vanguard Site Key, Research
    Bay Key, Cutting Torch, Boardroom Key, Industry Crest) — flagged as the next natural pass,
    matching the Police Station and Hospital's own pattern. Also not done: scene-by-scene
    scripting into a `Scripts/` file, a unique named boss creature beyond the Exposure Cohort pack
    encounter, and any explicit tie-in between specific already-encountered creatures and named
    Foundry employees (a compelling idea floated directly by the source material, deliberately not
    locked without further review).

- **Worthy Academy — the Southeast district's main location, written in full (2026-08-13).** The
  project owner supplied a 29-beat outbreak-night account for the Academy, explicitly framed as
  fundamentally different in kind from the Foundry, Hospital, and Police Station: *"If the Foundry
  is where Ravenwood's disaster begins, the Academy should be where the town tries to save its
  children and families... It isn't primarily about Vanguard research. It is about what happens
  when hundreds of terrified civilians gather in one place while nobody actually understands what
  they're hiding from."* Per that framing, this location deliberately tells its story through
  **people** rather than machinery, medical charts, or dispatch logs — handwritten rosters, teacher
  notes, children's drawings, family photographs — and introduces **no new creature type**, reusing
  standard Shamblers for both its signature encounters.
  [`Locations/Academy.md`](Locations/Academy.md) was rewritten from its original `_TBD_` placeholder
  into a full main-location file matching the other three districts' density, per
  [`CANON.md`](CANON.md) → "District Main-Location Design Standard":
  - **"Outbreak Night — What Actually Happened"** — a 29-beat timeline (the Academy's pre-existing
    role as Ravenwood's storm shelter, the first ordinary-disaster evacuees arriving, Vanguard's
    symptom-based isolation instructions reaching untrained school staff, the first Foundry
    families arriving, Vanguard demanding the full shelter roster to locate exposure cohorts, the
    Harris family's removal, the shelter filling into the hundreds, the first person turning inside
    the cafeteria, the police locking the doors, the GREEN/YELLOW/RED zone system and its
    breakdown, the hospital's "do not treat" warning reaching untrained staff, half the security
    detail being pulled to Highway 13, the PA system's escalating announcements, Vanguard demanding
    all RED-zone civilians and being physically refused, the standoff outside the Academy, the
    chief's broadcast reaching the shelter, a planned bus evacuation whose escort never arrives, the
    Yellow Zone's containment failure and a father forcing open a quarantine door, panic in the
    gymnasium, Vanguard's abandonment, the Academy's fracture into six survivor pockets, the Last
    School Bus's unanswered radio log, the children-left-behind whiteboards and teacher's notebook,
    Principal Ashford's final unanswered broadcast, and the last defensive stand's badge and note —
    *"If they make it out, that's enough."*) — explicitly cross-referenced against
    [`Locations/Police_Station.md`](Locations/Police_Station.md),
    [`Locations/Hospital.md`](Locations/Hospital.md), and
    [`Locations/Foundry_Refinery.md`](Locations/Foundry_Refinery.md)'s own timelines via a new "How
    the Academy Connects to the Other Locations" table, per the project owner's explicit framing
    that the Academy gives the civilian perspective on events already established elsewhere.
  - **Full room/blueprint build:** Front Entrance → Gymnasium (hub, gating the Administration
    Office, Auditorium, Library, and Maintenance Basement) → Cafeteria (signature single encounter)
    → Administration Office → Isolation Wing, plus a second branch (needs an Auditorium Key from
    the secondary Student Housing location) → Auditorium → Library, plus a third, deepest branch
    (needs Generator Fuel from the secondary Athletic Field location) → Maintenance Basement → East
    Academic Wing / Science Rooms (needs a Fire Axe; this district's signature pack encounter) → PA
    / Principal's Office → Founder's Hall (Knowledge Crest) → the Maintenance Escape Corridor (a
    mandatory, non-combat climax reached only *after* the crest, not gating it), plus a non-gating
    Bus Loading Area and three secondary locations (Student Housing, Athletic Field, Playgrounds —
    reconciling `Academy Library`'s earlier city-layout listing as a secondary location into being
    part of the main building instead, per the source material's own treatment of the library as a
    core campus room and survivor pocket). Five mermaid blueprint diagrams, same convention as the
    Hotel, Police Station, Hospital, and Foundry.
  - **New founder named: Eleanor Worthy**, Worthy Academy's founder, keeper of the Knowledge Crest —
    added to [`CANON.md`](CANON.md) → "Named Characters Confirmed" alongside Josiah Hale, Nathaniel
    Voss, and Elias Thorne (all five founders are now named except the still-`_TBD_` Faith
    Crest/Monastery founder). **New named character: Principal Diane Ashford** — the Academy's own
    Chief/Fitch-equivalent, whose fate is deliberately left unresolved, same convention.
  - **Direct crossover documents added to
    [`Locations/Police_Station.md`](Locations/Police_Station.md),
    [`Locations/Hospital.md`](Locations/Hospital.md), and
    [`Locations/Foundry_Refinery.md`](Locations/Foundry_Refinery.md):** the Highway 13
    security-detail pullback and the Academy standoff/final-broadcast material (Police Station), the
    hospital's "do not perform invasive treatment" guidance reaching the shelter (Hospital), and the
    Harris family's Foundry-side evacuation paper trail (Foundry) — satisfying the project owner's
    explicit request that all four locations' records overlap directly.
  - **16 new AI-generated room concepts** — full visual coverage for the entire new location in one
    pass (13 main-building rooms/areas plus 3 secondary locations), logged in
    [`Assets/README.md`](Assets/README.md). Several renders repeated the recurring "Ravencroft"
    naming-generation error plus new one-off mis-namings ("Holloway Academy," "Riverdale Academy,"
    "Steelgate School District," "Steelgate Elementary") — all flagged in each render's caption
    rather than adopted. Two renders (the Gymnasium's whiteboard, the Administration Office's
    "Vanguard – Personnel Request" folder, and the Founder's Hall's portrait/plaque) landed exactly
    on the intended canon details unprompted.
  - **Not done in this pass:** individual `Items/Key_Items/` writeups for this district's nine new
    key items (Administration Office Key, Isolation Wing Key, Auditorium Key, Library Key,
    Generator Fuel, Fire Axe, Principal's Office Key, Founder's Hall Key, Knowledge Crest) —
    flagged as the next natural pass, matching the Police Station, Hospital, and Foundry's own
    pattern. Also not done: scene-by-scene scripting into a `Scripts/` file, and a unique named boss
    creature (deliberately omitted per the source material's framing, but flagged in
    [`Locations/Academy.md`](Locations/Academy.md) → "Unresolved Ideas" in case that's reconsidered
    later for pacing).

- **Our Lady of Solace Monastery — the North district's main location, written in full
  (2026-08-13), and the last surface location before Chapter 3.** The project owner supplied a
  33-beat outbreak-night account for the Monastery, explicitly framed as fundamentally different
  from the previous four districts: *"Those places reveal what Vanguard did to Ravenwood in the
  modern era. The Monastery reveals something much older: Ravenwood had encountered the effects of
  the Black Vein long before Vanguard ever arrived... The Monastery isn't about religion defeating
  science. It's about memory versus arrogance."* [`Locations/Monastery.md`](Locations/Monastery.md)
  was rewritten from its original `_TBD_` placeholder into a full main-location file matching the
  other four districts' density, per [`CANON.md`](CANON.md) → "District Main-Location Design
  Standard":
  - **"Outbreak Night — What Actually Happened"** — a 33-beat timeline (the monastery's centuries
    of pre-Vanguard Black Vein observation recorded as religious language, the first ancient
    sealing, Vanguard's 1968 polite archive-access requests turning into bureaucratic pressure and
    covert underground surveying, Brother Cormac's secret hidden archive proving Vanguard was
    making the phenomenon worse, the spring water turning on Outbreak Night, Vanguard's "DO NOT
    ENTER THE LOWER MONASTERY" order, the Foundry tremor reaching the ridge and revealing Vanguard's
    illicit excavation behind the old seal, a Foundry survivor confirming the two cave systems
    connect, the monks refusing to surrender him, the hospital/monastery cross-confirmation that
    trauma worsens mutation, the Vanguard standoff and the police officer's reversal after seeing an
    old Vanguard memorandum, the crypt breach and re-sealing ("do not open the gate for the voice of
    a friend"), the monastery's division into survivor zones, Vanguard's attempt to burn the
    archive, the bells rung as a citywide warning, the discovery of the oldest record ("a vein
    without end"), proof Vanguard had monastery records before Project Ashen's modern form, the
    failed evacuation, Brother Cormac's refusal to leave, the crypt seal finally breaking, and his
    final broadcast: *"The source is beneath us. It was here before Vanguard. Do not believe they
    discovered it. They opened what others had already learned to close."*) — explicitly
    cross-referenced against [`Locations/Police_Station.md`](Locations/Police_Station.md),
    [`Locations/Hospital.md`](Locations/Hospital.md), [`Locations/Foundry_Refinery.md`](Locations/Foundry_Refinery.md),
    and [`Locations/Academy.md`](Locations/Academy.md)'s own timelines via a new "How the Monastery
    Connects to the Other Locations" table, plus a project-owner-supplied "What the Five Surface
    Locations Now Reveal" summary tying all five districts' thematic identities together as Jim
    completes the last crest.
  - **Full room/blueprint build:** Monastery Gate → Chapel (hub, gating the Library/Archive, the
    Cloister, the Bell Tower, and the Crypt Antechamber) → Guest Quarters (signature single
    encounter) → Library/Archive, plus a second branch (needs an Archive Key from the secondary
    Overlook Trail location) → the Hidden Archive → the Cloister → the Bell Tower, plus a third,
    deepest branch (needs a Crypt Antechamber Key from the secondary Hillside Cemetery location) →
    Crypt Antechamber (Vanguard's hidden excavation equipment) → the Old Seal / Crypt Depths (needs
    a Breaching Tool; this district's signature pack encounter) → the Reliquary (Faith Crest) → the
    Sealed Passage / Old Caves (a mandatory, non-combat climax reached only *after* the crest, not
    gating it — **the final surface-world scene in the game**), plus a non-gating Spring/Well
    Chamber and three secondary locations (Hillside Residential Street, Hillside Cemetery, Overlook
    Trail — pulled directly from this district's already-established city-layout notes). Five
    mermaid blueprint diagrams, same convention as the Hotel, Police Station, Hospital, Foundry, and
    Academy.
  - **New founder named: Abbot Matthias Kane**, Our Lady of Solace Monastery's founder, keeper of
    the Faith Crest — added to [`CANON.md`](CANON.md) → "Named Characters Confirmed," completing
    all five founders (Hale, Voss, Thorne, Worthy, Kane). Because the source material explicitly
    states the monastery predates the modern town, Kane's 1887 "founding" is reconciled as
    formally chartering the *current religious order* atop a much older site, not building the
    physical monastery itself — flagged explicitly in [`CANON.md`](CANON.md) rather than silently
    contradicting the "predates the town" detail. **New named character: Brother Cormac** — the
    Monastery's own Chief/Fitch/Ashford-equivalent, whose fate is deliberately left unresolved,
    same convention.
  - **Major `CANON.md` addition: a third, much older point of human contact with the Black Vein
    cave system**, predating both the 1887 Memorial Park facility and the 1968 Foundry excavation
    by generations — the monastery's own sealed ridge caves. Vanguard later covertly tunneled from
    the Foundry side to bypass the monks' seal, making this the **one case where two of
    Ravenwood's three Black Vein sites do become physically connected**, and only because Vanguard
    deliberately built that connection; this doesn't reopen the existing Memorial Park/Foundry
    non-connection, it adds a third thread. This reframes Vanguard's culpability across the whole
    game: Project Ashen wasn't an unforeseeable discovery, it was documented generations-old
    warnings that Vanguard found, catalogued, and ignored.
  - **Direct crossover documents added to
    [`Locations/Police_Station.md`](Locations/Police_Station.md),
    [`Locations/Hospital.md`](Locations/Hospital.md),
    [`Locations/Foundry_Refinery.md`](Locations/Foundry_Refinery.md), and
    [`Locations/Academy.md`](Locations/Academy.md):** the Monastery standoff/Vanguard memorandum
    (Police Station), the hospital/monastery regeneration-findings exchange (Hospital), the
    matching cave-map tunnel-junction fragment (Foundry), and the Academy's own failing PA
    broadcasts cross-referenced against the monastery's emergency bells (Academy) — satisfying the
    project owner's explicit request that all five locations' records overlap directly.
  - **15 new AI-generated room concepts** — full visual coverage for the entire new location in one
    pass (12 main-building rooms/areas plus 3 secondary locations), logged in
    [`Assets/README.md`](Assets/README.md). Two flagged generation errors: the Chapel carried over
    a "Dr. Edward Halloway" portrait and caduceus stained glass from its Hospital style-reference
    image, and the Hillside Cemetery's sign reads "Steelgate Cemetery" instead of an
    unrelated name. Several renders (the Gate/Approach's own weathered "V" plaque, the Hidden
    Archive's journal text matching its canon quote verbatim, and the Reliquary's "Abbot Matthias
    Kane, Founder" portrait/plaque) landed exactly on the intended canon details unprompted.
  - **Not done in this pass:** individual `Items/Key_Items/` writeups for this district's eight new
    key items (Library Key, Archive Key, Cloister Key, Bell Tower Key, Crypt Antechamber Key,
    Breaching Tool, Reliquary Key, Faith Crest) — flagged as the next natural pass, matching the
    Police Station, Hospital, Foundry, and Academy's own pattern. Also not done: scene-by-scene
    scripting into a `Scripts/` file, and a unique named boss creature (deliberately left open per
    the source material's own framing that "the exact creature can depend on what enemy roster
    eventually fits the location" — flagged in [`Locations/Monastery.md`](Locations/Monastery.md) →
    "Unresolved Ideas" for a final decision once the full Chapter 2 enemy roster is reviewed
    together). **This completes all five Chapter 2 main locations** (Police Station, Hospital,
    Foundry, Academy, Monastery) and all five founders/crests.

## Direction Log (continued) — Police Station full scene-by-scene scripting (2026-08-13)

> With all five Chapter 2 main locations now written at the location-design/prose level, the
> project owner's next request was to move from prose to full scripts — "time to write out the
> scripts, puzzles, dialogue, NPC etc etc for each district now. Starting with the police station."
> [`Locations/Police_Station.md`](Locations/Police_Station.md) already had a scripted critical path
> ([`Scripts/Chapter_2_Ravenwood.md`](Scripts/Chapter_2_Ravenwood.md), Scenes 22–40, written earlier
> the same day during the RE-style restructure), but several beats flagged in that file's own
> "Unresolved Ideas" were still only prose: the optional Vanguard sub-plot's four rooms, the Sally
> Port breach point, the SURVIVORS/MISSING/DECEASED whiteboard, "Emergency Public Safety Directive
> 7," and the Chief's final broadcast recording. This pass closes all of them.

- **Scenes 25–26 expanded, in place.** Scene 25 (the Bullpen) now describes two additional doors
  visible from the hub — the Vanguard Liaison Office's unmarked corporate placard (no visible lock)
  and Detective Cole's propped-open office — plus a new "Optional — the whiteboard" beat covering
  both the SURVIVORS/MISSING/DECEASED lists and the full text of "Emergency Public Safety Directive
  7." Scene 26 (Sergeant Calloway) gained an optional dialogue branch where Jim can ask about Cole's
  office (a short, restrained hook — "Cole. Yeah." — per the "environmental discovery, not
  exposition" convention already governing this sub-plot, resolving the exact open question
  [`Characters/Ruth_Calloway.md`](Characters/Ruth_Calloway.md) had flagged) and a new "Optional —
  the dispatch recorder" beat playing both the St. Dymphna Hospital exchange (already-locked text,
  now voiced for the first time) and the Chief's final broadcast in full.
- **New Scenes 41–45, appended after Scene 40.** Rather than renumber any existing scene (several
  other files already cite Police Station scene numbers directly — Dale_Pruitt.md, the Weapons/
  Items files, Chapter_1, etc. — renumbering would have cascaded), the four Vanguard sub-plot rooms
  and the Sally Port were written as new scenes at the end of the district's script, reachable
  logically from the Bullpen/Booking Corridor at any point once their gating item is found:
  - **Scene 41 — The Sally Port.** Environmental-only, per the already-resolved "no creature
    encounter" decision — the half-lowered shutter, a jammed/dropped shotgun (flavor only, not a
    pickup, so it can't be confused with the Armory's shotgun), and an optional ammo cache.
  - **Scene 42 — Detective Cole's Office.** Full search sequence (desk, then ceiling tiles) yielding
    the Vanguard Access Card and Cole's hidden folder — the missing-persons list, the security
    still, the Daniels email exchange, and his locked closing line, quoted verbatim from
    [`Characters/Aaron_Cole.md`](Characters/Aaron_Cole.md).
  - **Scene 43 — The Vanguard Liaison Office.** The V-CASE protocol binder and confidential
    watchlist; the watchlist match is deliberately the same **T. Okonkwo** background name seeded on
    the Scene 25 whiteboard as a **survivor** — the point being that being watched didn't mean being
    taken, which reads as more unsettling than a 1:1 victim match would have.
  - **Scene 44 — The Cold Cells.** The bent cell door and the unsigned handwritten note, kept
    exactly as unresolved/bodiless as the location file's prior decision specified.
  - **Scene 45 — The Vanguard Observation Booth.** The reverse angle of the existing Interview Room
    (Scene 32), confirmed as a deliberate framing choice.
- **New decision: the Chief's name is Marcus Doyle** — needed because his final-broadcast recording
  self-identifies ("This is Chief Marcus Doyle, Ravenwood Police Department..."). Chosen specifically
  to avoid any confusion with "CHIEF E. WHITAKER," the unprompted, already-flagged non-canonical
  nameplate from one AI-generated Chief's Office room render, and with Earl Whitaker at the Hotel.
  Added to [`CANON.md`](CANON.md) → "Named Characters Confirmed." His ultimate fate remains exactly
  as unresolved as before this pass — only his name changed.
- **[`Locations/Police_Station.md`](Locations/Police_Station.md) updated throughout:** a fifth
  revision note, the scene range in the header (22–40 → 22–45), scene citations added to every
  affected item in "Documents" and "Key Items," and every relevant bullet under "Unresolved Ideas"
  struck through and marked resolved/scripted rather than deleted, preserving the history of what
  was open before this pass.
- **Not done in this pass:** the same scripting treatment for the other four Chapter 2 districts
  (Hospital, Foundry, Academy, Monastery) — each still has only its location-design/prose file and
  no `Scripts/` entry of its own. Per the project owner's phrasing ("starting with the police
  station"), the plan is to repeat this exact process — full scene-by-scene dialogue, puzzle
  interaction prompts, document text, and NPC scenes — for each remaining district in turn.

## Direction Log (continued) — St. Dymphna Hospital full scene-by-scene scripting (2026-08-13)

> Second district scripted, per the project owner's follow-up ("move on to the next area gotta
> design the puzzles leading up to the emblem include lore notes etc etc"). Hospital was the
> obvious next target — the project owner had already called it "the natural next step" earlier in
> the session, and its location file (unlike the Police Station's) had **zero** `Items/Key_Items/`
> writeups yet, so this pass combined two jobs: writing the script and, for the first time, giving
> this district's key items their own files.

- **New file: [`Scripts/Chapter_2_Hospital.md`](Scripts/Chapter_2_Hospital.md), 17 scenes.** Kept
  separate from [`Scripts/Chapter_2_Ravenwood.md`](Scripts/Chapter_2_Ravenwood.md) (already 45
  scenes) rather than appended to it — restarts its own Scene 1 count, matching
  [`Scripts/README.md`](Scripts/README.md)'s existing "restarts at Scene 1 for each new chapter
  file" rule, applied here at the per-district level since Chapter 2 itself has no natural
  chapter-break between districts. Covers the full critical path (District Entry → Ambulance Bay →
  E.D. hub → Radiology → Laboratory → Administration → the Medical Arts Building backtrack →
  Surgical Wing → the boss fight → ICU → Chapel/Medical Crest) plus all optional content (the
  Morgue, Maternity Ward/Broodling, NICU, the Vanguard Quarantine Checkpoint → Psychiatric Ward
  chain, and the Parking Structure).
- **Richard Dalton's Tier 2b branch, both versions, now fully scripted** (Scene 2) — the alive
  version's panicked Ambulance Bay meeting, and a new decision for the dead version's staging
  (face-down near the bay, one arm outstretched toward the entrance he never reached), resolving
  the "not yet decided" flag on [`Characters/Richard_Dalton.md`](Characters/Richard_Dalton.md).
  **Deliberately not written:** the actual "what does Jim tell Richard" return conversation — that
  character file explicitly asks for this to stay open pending a separate decision, so Scene 2 ends
  on his request and Scene 13 (the Maternity Ward) only confirms what Jim now privately knows.
- **The Broodling and "The Surgeon" boss fight both fully staged narratively** (Scenes 10 and 13) —
  move-set-level description (the giant hand's lunge/slam plus the tranquilizer-gun's ranged
  threat; the Broodling's fast, low, hard-to-hit scrabbling) without locking specific damage/health
  numbers, which both creature files already flag as a separate, later mechanical-design pass.
- **Seven new [`Items/Key_Items/`](Items/Key_Items/README.md) files**, closing the gap the Police
  Station's own `Items/` audit didn't cover yet, since Hospital.md didn't exist until after that
  audit: Fire Axe, Laboratory Key, Administration Key, Surgical Wing Access Card, Pry Bar, Chapel
  Key, and Medical Crest — each with a new AI-generated inventory-icon concept (small, flat-shaded
  pixel-art icon on a plain dark background, matching the Police Station's own item-icon
  convention), logged in [`Assets/README.md`](Assets/README.md).
- **[`Locations/Hospital.md`](Locations/Hospital.md) updated throughout:** a new revision note, key
  item cross-links replaced (no more "not yet written" placeholders), and every resolved bullet
  under "Unresolved Ideas" struck through with a pointer to where it's now handled — same
  preserve-the-history convention used for the Police Station's own pass.
- **Not done in this pass:** the same treatment for Academy, Foundry, and Monastery — each still
  has only its location-design/prose file. Next in line per this same repeated process.

## Direction Log (continued) — splitting each district into its own script file (2026-08-13)

> The project owner's follow-up after the Hospital pass: *"Yea we should split each district into
> its own file to make it easier. Let's keep going forward with the next district."* Since
> `Chapter_2_Hospital.md` had already established the "one standalone file per district, restarting
> its own Scene 1 count" pattern, this pass retroactively applied the same split to the Police
> Station, which up to this point still lived inside `Chapter_2_Ravenwood.md` as Scenes 22–45.

- **New file: [`Scripts/Chapter_2_Police_Station.md`](Scripts/Chapter_2_Police_Station.md).** The
  Police Station's full script (all 24 scenes, dialogue and document text completely unchanged) was
  cut out of `Chapter_2_Ravenwood.md` and moved here, renumbered to its own Scene 1–24 count.
  **Renumbering map**, kept here for anyone with an old note still citing a pre-split number:
  old Scene 22→1, 23→2, 24→3, 25→4, 26→5, 27→6, 28→7, 29→8, 30→9, 31→10, 32→11, 33→12, 34→13,
  35→14, 36→15, 37→16, 38→17, 39→18, 40→19, 41→20, 42→21, 43→22, 44→23, 45→24.
- **`Chapter_2_Ravenwood.md` retitled and trimmed to "Chapter 2 — Ravenwood (Downtown & Memorial
  Park)"** — now covers only Scenes 1–21 (the street crossing, Memorial Park, and the Downtown
  introduction), the shared entry point every district route passes through before splitting off.
  Its header and closing footer were rewritten to point at the per-district files instead of
  describing an ever-growing single chapter.
- **Every cross-reference updated**, not just within the two split files themselves:
  [`Locations/Police_Station.md`](Locations/Police_Station.md) (a new sixth revision note plus
  every scene citation throughout), [`CANON.md`](CANON.md), [`MASTER_STORY.md`](MASTER_STORY.md),
  [`Scripts/README.md`](Scripts/README.md), [`Creatures/Ashen_Hound.md`](Creatures/Ashen_Hound.md),
  [`Characters/README.md`](Characters/README.md), [`Characters/Eli_Reyes.md`](Characters/Eli_Reyes.md),
  [`Characters/Ruth_Calloway.md`](Characters/Ruth_Calloway.md), and
  [`Weapons/Ranger_870_Pump_Shotgun.md`](Weapons/Ranger_870_Pump_Shotgun.md) all had their
  `Chapter_2_Ravenwood.md` + old-scene-number citations replaced with
  `Chapter_2_Police_Station.md` + the new numbers. Two internal cross-references inside the moved
  content itself (a pointer back to Memorial Park's guardhouse note, and to Downtown's library
  clipping) were upgraded from bare "(Scene N)" mentions to explicit
  `Chapter_2_Ravenwood.md`-qualified links, since a same-file implicit reference would otherwise now
  be ambiguous between the two files' own Scene 10s/20s.
- **Deliberately left untouched:** older historical log entries elsewhere in this file (e.g. "the
  originally-written Police Station, then Scenes 22–33, was too...") that narrate the *history* of
  earlier restructuring passes using superseded scene numbers — those already describe a past state
  using qualifying language ("then Scenes X"), so rewriting them to current numbers would misrepresent
  what was actually true at the time they're describing. Only "current status" references were
  updated.
- **Not done in this pass:** the same per-district file split doesn't apply yet to Academy, Foundry,
  or Monastery, since none of them have a `Scripts/` file yet at all — they'll simply be written
  directly as their own standalone files from the start, per [`Scripts/README.md`](Scripts/README.md)'s
  now-locked convention.

## Direction Log (continued) — Steelgate Refinery full scene-by-scene scripting (2026-08-13)

> Third district scripted, per the project owner's continued direction ("Let's keep going forward
> with the next district"). The Foundry was next in the original writing order (Police Station →
> Hospital → Foundry → Academy → Monastery), and — following the newly-locked convention — was
> written directly as its own standalone file from the start, with no intermediate combined-file
> stage to split out of later.

- **New file: [`Scripts/Chapter_2_Foundry.md`](Scripts/Chapter_2_Foundry.md), 17 scenes.** Covers
  the full critical path (District Entry → Loading Yard → Casting Hall hub → the Foundry Clinic →
  the Machine Shops/Loading Docks backtracks → the Vanguard Site Office → the Restricted Elevator
  descent → the Exposure Records Room → the Research Bay → the Security Checkpoint/Exposure Cohort
  fight → the Founder's Boardroom/Industry Crest → the mandatory Black Vein Cavern climax) plus the
  optional Break Room, Old Mine Workings, and Rail Yard content.
- **The Exposure Cohort's signature pack fight fully staged narratively** (Scene 13) — several
  long-term-exposed workers, steadier and more coordinated than a standard Shambler per that
  creature file's "settled/adapted" direction, without locking specific damage/health numbers
  (flagged there as a separate mechanical-design pass).
- **The Black Vein Cavern scripted as the district's true climax** (Scene 16) — deliberately placed
  after the Industry Crest is already collected rather than gating it, per
  [`Locations/Foundry_Refinery.md`](Locations/Foundry_Refinery.md)'s explicit design intent; ends
  on the final Foundry broadcast, quoted verbatim.
- **Plant Manager Daniel Fitch kept exactly as unresolved as his location-file treatment** — never
  seen on-screen alive or dead, reconstructed entirely through his office (Scene 6) and the final
  broadcast (Scene 16), same convention as the Police Station's Chief and the Hospital's Vanguard
  Liaison; no new dedicated `Characters/` file was created for him, consistent with that existing
  pattern.
- **Seven new [`Items/Key_Items/`](Items/Key_Items/README.md) files**, closing this district's own
  `Items/` gap the same way the Hospital pass did: Manager's Office Key, Restricted Elevator Access
  Card, Vanguard Site Key, Research Bay Key, Cutting Torch, Boardroom Key, and Industry Crest —
  each with a new AI-generated inventory-icon concept, logged in
  [`Assets/README.md`](Assets/README.md).
- **[`Locations/Foundry_Refinery.md`](Locations/Foundry_Refinery.md), [`CANON.md`](CANON.md),
  [`MASTER_STORY.md`](MASTER_STORY.md), [`Scripts/README.md`](Scripts/README.md), and
  [`Creatures/Exposure_Cohort.md`](Creatures/Exposure_Cohort.md) updated throughout** with the new
  script's cross-links and resolved "Unresolved Ideas" bullets, same preserve-the-history
  convention used for the two previous districts' passes.
- **Not done in this pass:** the same treatment for Academy and Monastery — each still has only its
  location-design/prose file. Two districts remain.

## Direction Log (continued) — Downtown/Memorial Park visual-coverage gap + concept art in Scripts (2026-08-14)

> The project owner flagged a real gap directly: *"there's some that's not located like Pearl's
> diner I don't see it within the locations tab,"* and separately asked *"should we add the concept
> maps to the scripts as well[?]"* Investigating confirmed both: Downtown (Pearl's Diner, the
> Public Library, City Hall) had a fully written script
> ([`Scripts/Chapter_2_Ravenwood.md`](Scripts/Chapter_2_Ravenwood.md), Scenes 18–21) but **no**
> `Locations/` file and **no** concept art at all — the only content in the entire game in that
> state. Memorial Park itself had a `Locations/` file but only one image (the Founders Memorial
> plaque's own close-up), missing its street crossing, guardhouse, and full-statue shots. And no
> script file anywhere embedded concept art directly — only `Locations/` files did.

- **New file: [`Locations/Downtown_Ravenwood.md`](Locations/Downtown_Ravenwood.md).** Assembled
  retroactively from the already-locked script (the reverse of the usual write order), covering
  Pearl's Diner, the Public Library, and City Hall as a short, deliberately **linear** stretch —
  no keys, no crest, no backtracking, unlike the five main districts. Flags one loose end pulled
  directly from the existing script: City Hall's Mayor's Office is locked and its key is never
  recovered anywhere in current material.
- **Six new room concepts** (AI-generated, style-anchored to existing district art): the street
  crossing/park entrance, the guardhouse, a full-statue Founders Memorial establishing shot, Pearl's
  Diner, the Public Library, and City Hall. Embedded in the new Downtown file and the updated
  [`Locations/Memorial_Park.md`](Locations/Memorial_Park.md). No naming/generation errors on any of
  the six — notably breaking this project's long, recurring "Ravencroft"/wrong-name pattern seen
  across nearly every other district's first-pass art.
- **New locked convention: concept art now also embedded directly in `Scripts/` files**, not just
  `Locations/` files — see [`Assets/README.md`](Assets/README.md) for the full rule. Applied
  retroactively to all four existing Chapter 2 scripts, reusing each district's own already-generated
  images rather than creating duplicates: [`Scripts/Chapter_2_Police_Station.md`](Scripts/Chapter_2_Police_Station.md)
  (22 images across its 24 scenes), [`Scripts/Chapter_2_Hospital.md`](Scripts/Chapter_2_Hospital.md)
  (15 of 17), [`Scripts/Chapter_2_Foundry.md`](Scripts/Chapter_2_Foundry.md) (16 of 17), and
  [`Scripts/Chapter_2_Ravenwood.md`](Scripts/Chapter_2_Ravenwood.md) (6 of its 21 scenes — only the
  ones with a matching room image; Memorial Park's interior-clearing scenes and Downtown's district-
  entry scene were left as-is rather than force a mismatched image in). Each embedded image is
  followed by a one-line caption pointing back to the room's `Locations/` file.
- **Deliberately not touched:** [`Scripts/Chapter_1_One_Night_Only.md`](Scripts/Chapter_1_One_Night_Only.md)
  — it's marked locked and predates this convention; revisit only if explicitly requested.
- **Not done in this pass:** the same audit hasn't been run against Academy's or Monastery's own
  `Locations/` files (both already have full room-by-room concept art from their own build-out
  passes, so this gap was specific to Downtown/Memorial Park predating the district-by-district
  convention entirely) — flagged only as a "worth a quick look eventually" item, not a known gap.

## Direction Log (continued) — Worthy Academy full scene-by-scene scripting (2026-08-14)

> Fourth district scripted, per the project owner's continued direction ("let's go on with the
> next one"). Academy was next in the original writing order (Police Station → Hospital → Foundry
> → Academy → Monastery), and was written directly as its own standalone file with the new
> "concept art embedded in Scripts" convention already in place from the start, rather than applied
> retroactively.

- **New file: [`Scripts/Chapter_2_Academy.md`](Scripts/Chapter_2_Academy.md), 17 scenes.** Covers
  the full critical path (District Entry → Front Entrance → the Gymnasium hub → the Cafeteria's
  signature encounter → the Administration Office/Harris family reveal → the Isolation Wing → the
  Student Housing/Auditorium/Library backtrack → the Athletic Field/Maintenance Basement/East Wing
  backtrack culminating in the district's Shambler pack fight → the PA/Principal's Office → Founder's
  Hall/Knowledge Crest → the mandatory Maintenance Escape Corridor climax) plus the optional Bus
  Loading Area and Playgrounds. 15 of the 17 scenes embed the room concept already generated for
  [`Locations/Academy.md`](Locations/Academy.md); only the district-entry approach and the
  Maintenance Escape Corridor (which has no dedicated room render) have none.
- **No new creature type introduced**, per the project owner's explicit framing that this
  district's horror is about people, not a monster — every encounter (Scenes 3, 4, and 12) is a
  standard Shambler, staged with different context (a volunteer, a Foundry employee, a group of
  turned Isolation Wing patients) rather than a new visual/mechanical design.
- **Principal Diane Ashford kept exactly as unresolved as her location-file treatment** — never
  seen on-screen alive or dead, reconstructed entirely through her office (Scene 13) and the final
  broadcast, same convention as Daniel Fitch and the Police Station's Chief.
- **The Harris family thread paid off across three separate rooms in one script**, deliberately —
  the Foundry's own optional evacuation slip (if found), the Administration Office's "I gave them
  the Harris family" note (Scene 5), and Student Housing's packed, unclaimed duffel bag (Scene 7),
  giving a name mentioned only in passing elsewhere a physical, personal object.
- **Nine new [`Items/Key_Items/`](Items/Key_Items/README.md) files**, closing this district's own
  `Items/` gap: Administration Office Key, Isolation Wing Key, Auditorium Key, Library Key
  (filed as `Academy_Library_Key.md`), Generator Fuel, Fire Axe (filed as `Academy_Fire_Axe.md`),
  Principal's Office Key, Founder's Hall Key, and Knowledge Crest — each with a new AI-generated
  inventory-icon concept. Two items were deliberately filed with an "Academy_" prefix rather than
  their plain in-fiction name, to avoid colliding with St. Dymphna Hospital's own Fire Axe and the
  Monastery's own (not-yet-written) Library Key — same convention already established for the
  Manager's Office Key/Manager's Key distinction.
- **[`Locations/Academy.md`](Locations/Academy.md), [`CANON.md`](CANON.md),
  [`MASTER_STORY.md`](MASTER_STORY.md), [`Scripts/README.md`](Scripts/README.md), and
  [`Assets/README.md`](Assets/README.md) updated throughout** with the new script's cross-links and
  resolved "Unresolved Ideas" bullets, same preserve-the-history convention used for the three
  previous districts' passes.
- **Not done in this pass:** the same treatment for the Monastery — the one remaining district,
  and the last surface location before Chapter 3.

## Direction Log (continued) — Concept art perspective correction pass (2026-08-14)

> Prompted by the project owner flagging that several room concepts had drifted into a flat,
> straight-on/eye-level camera framing instead of the established house style — an elevated 3/4
> top-down camera at a steep tilted angle with a clearly diamond-rotated floor/paving pattern
> receding into depth, as set by
> [`Assets/Reference/police_station_bullpen_concept.png`](Assets/Reference/police_station_bullpen_concept.png)
> and the hotel and police station concepts generally.

- **Full re-audit of every district's room concept art against the bullpen reference.** Confirmed
  several images across Steelgate Refinery and the Monastery had the flat-camera issue despite
  earlier captions claiming they were already correct; Downtown Ravenwood, the Founders Memorial,
  and the Street Crossing concepts were already compliant on review.
- **13 Foundry images regenerated:** Founder's Boardroom, Loading Yard, Clinic, Break Room/Locker
  Room, Plant Manager's Office, Vanguard Site Office, Restricted Elevator, Exposure Records Room,
  Security Checkpoint, Old Mine Workings, Loading Docks, the Black Vein Cavern, and the Rail Yard —
  all now show the elevated isometric-style camera and a receding diamond floor/ground pattern.
- **9 Monastery images regenerated:** the Gate Approach, the Cloister, the Bell Tower, the Crypt
  Antechamber, the Old Seal/Crypt Depths, the Sealed Passage/Old Caves, the Hillside Residential
  Street, the Hillside Cemetery, and the Overlook Trail — same correction, including exterior
  scenes (paths/roads now show diamond-rotated paving instead of a flat landscape view).
- **1 Memorial Park image regenerated:** the Guardhouse interior had the same flat, eye-level
  drift; regenerated to match the corrected style while keeping every scripted prop (desk, filing
  cabinet, VERN terminal, corkboard, inventory chest, "RAVENWOOD PARK" gate sign in the window).
- **[`Locations/Foundry_Refinery.md`](Locations/Foundry_Refinery.md),
  [`Locations/Monastery.md`](Locations/Monastery.md), and
  [`Locations/Memorial_Park.md`](Locations/Memorial_Park.md) caption text updated** to describe the
  corrected images and note the regeneration where a caption previously (incorrectly) claimed the
  original flat-camera version was already compliant.
- **No other districts required changes** — Police Station, the Hotel, St. Dymphna Hospital (after
  its own earlier correction pass), Worthy Academy, and Downtown Ravenwood were all already
  consistent with the reference style on this audit.

## Direction Log (continued) — Chapter 2 narrative craft review (2026-08-14)

> The project owner read the fully-scripted Police Station, Hospital, Foundry, and Academy
> chapters (plus Chapter 1 and the Downtown/Memorial Park material) as narrative documents, not
> just structurally, and gave a full craft review. Recorded here in detail because it's directional
> for every future revision pass on Chapter 2 — not a one-off note.

**What's working well:**

- **Cross-district interconnectedness is the chapter's biggest strength.** Police radio calls
  surface on the hospital side, Foundry symptoms echo into the Academy, Vanguard directives recur
  across multiple institutions, and the player keeps reconstructing one shared night from
  different vantage points — the locations read as one outbreak, not five isolated horror levels.
- **The Police Station's institutional horror lands.** Vanguard hasn't replaced the department
  with cartoon villains — it has embedded itself inside a still-mostly-normal institution and can
  invoke agreements that turn local police into containment personnel (Directive 7, ordering
  officers to prevent civilians from leaving Ravenwood, is the clearest example of this "ugly
  institutional horror"). Reyes and the K-9 material give the station an emotional core so it isn't
  *only* about conspiracy documents.
- **The Hospital may be the strongest district conceptually** — it *demonstrates* Ashen rather than
  explaining it: doctors observe trauma triggering accelerated cellular activity, staff realize
  standard treatment may worsen the condition, and the place meant to save people becomes where the
  outbreak compounds fastest. This horror flows directly from the Black Vein/Ashen rules rather
  than generic zombie-hospital imagery.
- **The Foundry establishes that this predates the outbreak night itself.** Workers reporting
  headaches, joint pain, and other symptoms *before* the outbreak, normalized by the company
  clinic, gives Vanguard's behavior real history — they had already built systems for ignoring,
  controlling, and classifying warning signs, rather than improvising a cover-up after the fact.
- **The Academy reads much better in full script form.** Making it the civilian shelter gives it a
  distinct moral horror from the other four districts; the roster request targeting former
  Steelgate employees is particularly effective because it implies Vanguard was using the shelter
  population as a searchable exposure database while presenting it as evacuation planning. It also
  keeps the district's horror about people, not an exotic monster, per the existing design intent.
- **Leaving named people unresolved works and should continue.** The Chief disappearing, Daniel
  Fitch never getting a neat body, and Cindy's robe appearing without confirming whether she's
  alive, dead, or turned all make Ravenwood feel bigger than Jim's path through it. Explicit
  instruction: **resist tying every named person into a neat conclusion.**
- **Chapter 1 still has the best personal character storytelling** — Sarah's phone call establishes
  Jim's humor, stubbornness, job, marriage, and normal life without exposition, before Ravenwood
  destroys that normality. Chapter 2 is currently stronger on worldbuilding than on personal
  character development for Jim specifically.

**Concerns to address in future revision passes:**

1. **Structural repetition is becoming visible across districts.** Several districts currently
   share a literal shape: Jim enters a central hub room, sees several locked destinations, one
   route is open, a Shambler appears. The Hospital, Foundry, and Academy all repeat this. **Keep
   the underlying navigation/level-design grammar** (it's readable and works as game design) **but
   disguise it narratively per district** so it doesn't read as "same shape, different building":
   - Hospital: frame as Jim following the collapse of triage and emergency response.
   - Foundry: frame as Jim descending through successive layers of corporate secrecy.
   - Academy: frame as Jim reconstructing where different groups of civilians were separated and
     what became of them.
   - **Critical: never have Jim's dialogue acknowledge the repeated structure itself** (no "same
     shape again" or equivalent lampshading) — the player will already recognize the pattern;
     having Jim comment on it exposes the scaffolding rather than disguising it.
2. **Jim over-narrates document discoveries.** His short, purely reactive lines
   ("...Richard." / "Oh, no." / "...Cindy.") work well and should be kept. But across many document
   interactions he immediately verbalizes the implication the player just read, which risks making
   him feel like a narrator explaining the story rather than a man surviving it. **Cut roughly
   25–35% of his post-document commentary**, prioritizing cuts where his line simply restates the
   document's meaning — let the player have the realization instead.
3. **Evidence density risks over-explaining Vanguard before the Chapter 3 reveal.** Nearly every
   room currently delivers another note, recording, roster, log, clipboard, memo, or broadcast.
   Document-heavy rooms should feel natural to their setting (police reports in a station, charts
   in a hospital, logs in the Foundry), but the cumulative effect across all five districts must
   leave the player at the Chapter 3 threshold thinking **"I understand what Vanguard did to
   Ravenwood"** — not **"I understand exactly what Vanguard discovered, why Ashen exists, what the
   Black Vein really is, and how everything works."** The underground reveal needs room to
   fundamentally recontextualize what the player thinks happened; a future pass should look at
   trimming/redistributing document density with this ceiling in mind, not just cutting Jim's
   reactions to them.
4. **Chapter 2 needs more of Jim's own personal story, not just Ravenwood's.** The chapter is
   currently stronger on worldbuilding than on advancing Jim's character. Future passes should look
   for several moments per district (not necessarily many) that push Jim's own arc forward, in the
   spirit of Chapter 1's Sarah-call approach, rather than relying solely on environmental/document
   worldbuilding.

**Project owner's per-district story-strength ratings** (a healthy spread, not a ranking to
"fix"):

| District | Strongest at |
|---|---|
| Chapter 1 | Character + atmosphere |
| Police Station | Institutional horror |
| Hospital | Ashen/body-horror logic |
| Foundry | Conspiracy/history |
| Academy | Civilian/moral horror |
| Downtown/Memorial Park | Connective mystery + atmosphere |

**New story opportunity flagged — outbreak-night chronology as a five-piece jigsaw.** The five
districts could collectively tell the complete chronology of outbreak night, each holding a
different missing piece: the Police Station knows what orders were given; the Hospital knows what
the condition did; the Foundry knows where it started; the Academy knows what happened to
civilians; and **the Monastery can know something none of the other four could possibly know**
(not yet specified — an open creative slot, not a locked detail). Finishing all five would then
feel like *solving Ravenwood*, not simply collecting five crests. This reframes the crest-collection
structure as a chronology-reconstruction mechanic rather than a purely gameplay-gating device — not
yet implemented in any script or `Locations/` file, and not yet decided what the Monastery's unique
piece is.

## Direction Log (continued) — Five Puzzle Philosophies (approved 2026-08-14)

> Follow-up to the "Chapter 2 narrative craft review" entry above, which flagged structural
> repetition across districts as a delivery problem, not a story problem. The project owner's
> answer: don't just disguise the repetition narratively — give the five crest locations five
> genuinely different **puzzle mechanics**, each built around something unique to that
> institution, with the Ravenwood Hotel's repair-and-backtrack puzzle (Power East → tool → find
> component elsewhere → repair West → new route → courtyard) kept as the *benchmark to differ
> from*, not to repeat. Explicitly locked as **"the version worth building"** — this is now the
> target design for all five main locations, not a brainstorm. See "Five Puzzle Philosophies" in
> [`CANON.md`](CANON.md) for the locked summary table; full mechanic detail for each district is
> recorded here.
>
> **Implementation status (2026-08-14):** The Police Station — called out explicitly as "the
> first place to distinguish more strongly," since its current material leans hardest into
> Resident-Evil-style keys-and-locked-rooms — has had its puzzle backbone actually rewritten in
> [`Locations/Police_Station.md`](Locations/Police_Station.md) (Storyline, Puzzles, Key Items, and
> Blueprint sections) to the new Lockdown/Route mechanic below. The other three already-scripted
> districts (Hospital, Foundry, Academy) have their new puzzle mechanics fully specified in their
> own `Locations/` files as an approved addendum, **not yet folded into their existing
> Storyline/Blueprint prose** — treat the addendum as the target design and the older
> key-based Storyline text as superseded-but-not-yet-rewritten (flagged in each file). The
> Monastery (not yet scripted at all) gets its mechanic specified directly as its actual future
> design. **None of the four already-scripted districts' `Scripts/Chapter_2_*.md` scene-by-scene
> prose has been rewritten yet** — that's the largest remaining piece of this work, tracked in
> "Things That Still Need Development," below, since each script's prose was written against the
> old key-hunt mechanic and will need real narrative reconstruction, not a find-and-replace.

**The core idea:** each district's puzzle mechanic should be built from something unique to that
institution, use a distinct interaction verb, and — as a side effect — *teach the player something
true about Ravenwood* just by being solved. Collecting all five crests should feel like *solving
Ravenwood*, not collecting five video-game tokens.

| Location | Theme | Puzzle | Verb |
|---|---|---|---|
| Ravenwood Hotel (benchmark, already built) | — | Auxiliary power repair-and-backtrack | Repair |
| Police Station | Authority / Procedure | Emergency security lockdown | Route / Unlock |
| St. Dymphna Hospital | Medicine / Containment | Negative-pressure quarantine | Contain |
| Steelgate Refinery | Industry / Machinery | Industrial casting line | Operate |
| Worthy Academy | Knowledge / Reconstruction | Ravenwood historical archive | Understand |
| Our Lady of Solace Monastery | Faith / History / Mechanical Architecture | Ancient bell/counterweight mechanism | Interpret / Activate |

### 1. Police Station — The Lockdown Puzzle (Route / Unlock)

Not a repair puzzle, not a fetch-three-keys puzzle. Jim has to reconstruct what happened during the
department's final minutes and undo its own emergency lockdown, in the correct order, to reach the
original 1887 station house — sealed because Vanguard had secretly repurposed it.

- **Setup:** the old station house is inaccessible on arrival. The modern station's central
  security console reads `EMERGENCY LOCKDOWN ACTIVE / COMMAND AUTHORIZATION INCOMPLETE / SECURE
  AREAS: 4` — four zones (Armory, Holding Cells, Evidence, Old Station) were sealed manually, from
  different stations around the building, as the department collapsed. The system can't just be
  switched off; it has to be unwound in the sequence it was triggered.
- **Discovery (reconstructing the sequence):** Dispatch/Calloway establishes when lockdown began;
  the Chief's Office logbook establishes which officer secured which section; Booking reveals one
  zone was sealed because a detainee turned; the Evidence Room shows another zone sealed later
  still; the K-9 Unit Room/Reyes reveals he was sent toward the old station *last* — meaning
  the Old Station was the final, not the first, section sealed. Jim's realization: *"These weren't
  all locked simultaneously. They were progressively sealed as the station collapsed."*
- **Mechanic:** at the central security desk, a physical/electronic zone-control board. The system
  was designed to prevent prisoners from ever having a continuous path to the exterior — so
  opening one zone can automatically re-secure another. The player has to physically route Jim
  through the building, changing security states as he moves (open Gate A, walk through, trigger
  the next control from the far side, Gate A re-secures, Gate B opens, and so on) until a path into
  the old station exists. Functionally "manipulating a prison," using the department's own
  containment logic against itself.
- **Payoff:** the old station house holds the Authority Crest, and — per the existing Vanguard
  sub-plot — evidence that Vanguard had a secret watching post over the very containment system
  Jim just solved. Thematic point: *Jim uses the department's own system of authority to reach the
  place where that authority was compromised.*

### 2. St. Dymphna Hospital — The Quarantine Puzzle (Contain)

Not a power puzzle. Built around something hospitals uniquely have: negative-pressure isolation.
The Medical Crest sits in the historic chapel/display area on the far side of a treatment wing the
outbreak caused staff to convert into sealed emergency quarantine zones — and the automated system
sealed them for good when everything went wrong.

- **System:** an emergency isolation panel controls five zones — Air Intake, Isolation Ward,
  Surgical Wing, Decontamination Corridor, Exhaust — via large analog pressure gauges
  (green/yellow/red). Two incompatible zones can't be open at once; doing so trips `PRESSURE
  FAILURE — SAFETY INTERLOCK` and locks every door. A dead doctor's instructions teach the rule
  naturally: *"Never create a positive-pressure path from Isolation into General Care."*
- **Mechanic:** the player creates safe pressure gradients rather than simply unlocking doors —
  e.g. close General Intake → vent Isolation → the gauge drops → the Isolation door releases → Jim
  crosses → he's now trapped on that side → find the manual damper → seal Isolation behind him →
  pressurize Surgical → the Surgical door opens → repeat. A room-sized valve puzzle expressed
  through hospital airflow instead of pipes/electricity.
- **Horror hooks specific to the mechanic:** opening a vent and hearing something crawling in the
  ductwork; depressurizing a ward and having plastic isolation curtains suck inward around Jim;
  glimpsing something through observation glass before a section is even opened.
- **Payoff:** the crest sits in the original hospital chapel/founder's medical exhibit. Thematic
  point, delivered by the mechanic itself rather than a note: *the hospital wasn't trying to keep
  something out — it was desperately trying to keep something in.*

### 3. Steelgate Refinery — The Casting Puzzle (Operate)

The clearest machinery opportunity of the five. Jim physically operates an industrial casting line
to free the Industry Crest — not manufacture the crest itself, *release* it from the seized
ceremonial first-casting mold it's been mounted in since the plant opened, now sealed off along
with the rest of the underground level.

- **System:** a full foundry line — Ore Hopper → Furnace → Casting Ladle → Mold/Cooling Line — with
  the crest assembly sitting inside a seized mold carriage.
- **Mechanic, in stages (machinery stages, not fetch quests):** (1) restore furnace fuel flow via
  physical gas valves, not an electrical switch — watch pressure, since too much trips a safety
  relief and too little won't sustain the burner; (2) operate the overhead crane manually
  (left/right, forward/back, lower/raise — its shadow visibly moves across the floor) to position
  the casting ladle over the correct receptacle; (3) heat the seized mold just enough to expand the
  collar holding the crest assembly, not enough to melt anything important; (4) engage the cooling
  line — water blasts the casting bed, thermal contraction snaps the seized locking collar, and the
  ancient mold separates.
- **Payoff:** the Industry Crest, and beneath the casting machinery, a descending geological access
  shaft. Thematic point: *Steelgate wasn't built here because Ravenwood needed a foundry — the
  foundry exists here because of what was underneath it* — directly reinforcing material already
  central to this district (the Black Vein Cavern, the 1968 excavation).

### 4. Worthy Academy — The Archive Puzzle (Understand)

Almost entirely mental — no generator, no big key hunt, the closest thing the game has to an
old-school mansion riddle. Principal Ashford didn't hide the Knowledge Crest randomly during the
evacuation — she used the school's own history to hide it, and the player has to learn that history
to find it.

- **Central object:** a large Ravenwood historical timeline display in the library (Founding of
  Ravenwood → Steelgate Opens → St. Dymphna Founded → RPD Established → Worthy Academy Opens →
  Monastery Built), with several plaques removed or shifted out of order. Scattered through the
  Academy: a yearbook, a founder portrait, an old newspaper, school trophies, a library book, a
  class history project — none individually gives a combination; together they let the player
  reconstruct the correct chronology.
- **Mechanic:** five movable founder plaques (one per civic institution) in the archive must be
  placed in the correct founding-chronology order (not a numeric code) — Authority → Faith →
  Industry → Medicine → Knowledge, or whatever this project's actual locked founding chronology
  turns out to be once cross-checked against `CANON.md`'s "The Founders & the Five Crests." Getting
  it right triggers no electronics — just a mechanical `CLICK` and the timeline display swinging
  outward on a physical catch.
- **Payoff:** behind the display, Principal Ashford's emergency archive and the Knowledge Crest.
  Built-in seed for later mystery: one of the historical documents used to solve the puzzle can
  quietter contradict another (e.g. official records say Steelgate opened in 1968, but another
  document proves mining activity years earlier) — **deliberately left unexplained here**, payoff
  reserved for underground in Chapter 3.
- Reinforces the Academy's existing design intent (people/records over a new monster) by making its
  puzzle itself about *learning*, not fighting or fetching.

### 5. Our Lady of Solace Monastery — The Bell Tower Puzzle (Interpret / Activate)

Should feel the oldest of the five: no electronics, no card readers, no Vanguard terminal solving
it. The Faith Crest has been reachable since the monastery's construction — the monks knew how;
Vanguard didn't design this mechanism, they merely found it.

- **System:** four bell ropes in the tower, each secretly tied to part of a mechanical combination
  lock built into the monastery itself — one raises a counterweight, one releases a floor latch,
  one moves a stone locking bar, one resets the mechanism. Long assumed to be purely ceremonial
  ringing.
- **Clues (never spelled out as a number sequence):** a mural depicting Dawn → Labor → Mourning →
  Rest, each phase under a different bell; a prayer book marking the order of daily calls; four
  cloister statues facing the four corresponding directions. The player derives the ringing order
  from these, rather than being told it directly.
- **Mechanic/execution:** each bell pull is a major, audible event (heard across Ravenwood) with
  escalating environmental payoff — first bell, nothing; second, a distant `THUNK`; third, stone
  grinding beneath the chapel; fourth, the monastery floor shifts and a circular stone seal retracts
  beneath the altar.
- **The cost:** ringing the bells draws enemies toward the monastery — solving the puzzle
  transitions directly into a survival stretch, with Jim's own realization that he's just announced
  his exact location to half the ridge.
- **Payoff:** the crypt and the Faith Crest. This location should also carry the oldest evidence
  that something beneath Ravenwood was known long before Vanguard existed, consistent with
  `CANON.md`'s existing "Ravenwood encountered Black Vein's effects generations before either
  Vanguard access point existed" material — without implying anything supernatural.

### Why this matters beyond variety

Beyond avoiding repetition, the puzzles become a teaching structure: the Hotel teaches exploration;
the Police Station teaches how the town was controlled; the Hospital teaches how Ashen behaves; the
Foundry teaches where the problem physically came from; the Academy teaches Ravenwood's history;
the Monastery teaches that Ravenwood's connection to what lies underground predates Vanguard. By
the time all five crests are returned to Memorial Park, the player has completed five lessons
preparing them to understand Chapter 3's reveal — not just collected five tokens.

## Direction Log (continued) — consistency and declutter pass (2026-08-14)

> The project owner pointed out that districts were written one by one over several sessions, so
> earlier ones (Police Station, Hospital, Foundry) don't interlink with later ones (Academy,
> Monastery, Downtown/Memorial Park) as richly as the later files reference backward — plus a
> general request for fewer visible development notes and a less "generated" feel across the
> design documents.

- **Cross-linking audit.** Confirmed the asymmetry: Monastery's outbreak-night material already
  cross-references the Police Station, Hospital, and Foundry three times each, but those three
  files only referenced Monastery once each before this pass (now two, for the Police Station,
  after the Lockdown Puzzle rewrite below added an Interview Room cross-reference). More notably,
  Downtown Ravenwood and Memorial Park — written last — weren't referenced back from Hospital,
  Foundry, or Academy at all. Added one natural reciprocal document cross-reference to each: the
  Foundry's Manager's Office now references the same newspaper clipping Jim reads first at
  Downtown's library; the Hospital's records desk now has a partial version of City Hall's Carl
  Hess broadcast; the Academy's registration table now has a torn evacuation map matching City
  Hall's own crossed-out whiteboard. Not an exhaustive pass — a few well-chosen links rather than
  forcing every possible connection.
- **Declutter pass on `Locations/Police_Station.md`, `Hospital.md`, `Foundry_Refinery.md`,
  `Academy.md`, and `Monastery.md`.** Each file's header previously stacked several multi-paragraph
  "Revision note" blockquotes (proposal dates, "pending review" tags, what changed and why) directly
  in the design document itself. Condensed each to a short pointer at this file for full history,
  since that history already lives here in full. Room-concept image captions were similarly
  over-explaining generation attempts inline; this pass didn't rewrite all of them, but the Police
  Station's full rewrite (below) sets the target: a short line describing what the image shows,
  not a log of how many times it was regenerated.
- **What this pass did not do:** rewrite any dialogue. The project owner's separate note that
  Jim's dialogue and NPC voice should read as more natural/less AI-generated is a `Scripts/`-level
  concern, not a `Locations/`-level one — tracked as its own item in "Things That Still Need
  Development," below, since it requires reading and rewriting actual scene prose across four
  large script files rather than restructuring reference documents.

## Direction Log (continued) — puzzle-design refinement pass (2026-08-14)

> Follow-up review after the Five Puzzle Philosophies redesign: confirmed the carbon-copy problem
> is fixed and the interconnected-chronology goal is largely achieved, then flagged refinements
> before the script rewrite phase. Applied directly to the `Locations/` files where concrete enough
> to act on now; the rest is guidance for whoever rewrites the scripts.

**Applied in this pass:**

- **Varied the opening rhythm per district**, since all five previously described themselves in the
  same "central hub, see several sealed points at once" terms. Police Station keeps its Bullpen hub
  as-is (a security console genuinely belongs there). Hospital's Triage Hall now pulls Jim deeper in
  before the sealed wings become visible. The Foundry's Casting Hall now dominates the room
  immediately as visible, seized machinery — the mystery is the dead machine, not four locked
  doors. The Academy is now explicitly the least hub-like of the five, following the shelter's
  aftermath outward rather than cataloguing exits. The Monastery's Chapel was already softened
  during the puzzle redesign itself.
- **Foundry: the three old key-chain rooms now feed the Casting Line puzzle directly** — the
  Manager's Office holds the furnace pressure log, the Vanguard Site Office holds the crane
  override, and the Restricted Elevator is where the cooling main was shut off — so exploring the
  plant and solving the puzzle are the same activity instead of a key hunt bolted onto it.
- **Academy: redundant clues, not five mandatory ones.** Eight historical objects exist; any four
  or five are enough to solve the chronology, so attentive players can solve it early and unsure
  players can keep searching — an actual deduction puzzle rather than "five keys wearing paper
  costumes."
- **Monastery: aggressively removed the old mandatory key chain** (Library, Cloister, Bell Tower,
  Reliquary Keys, and the Breaching Tool) now that the Bell Tower Puzzle makes it redundant — the
  critical path is key-free end to end. Kept the Archive Key (Overlook Trail) and Crypt Antechamber
  Key (Hillside Cemetery) as clearly optional, reward-only backtracks; the Crypt Antechamber is now
  an explicit dead end (Vanguard's own failed attempt to drill past the mechanism), not a shortcut.
- **Police Station: demoted the bolt-cutter chain to optional.** The Fire Station's bolt cutters
  now open a padlocked locker *inside* the Evidence Room (bonus loot + the Courthouse key), not the
  room's own door — the Lockdown Puzzle alone carries the critical path, so the district's
  memorable sentence stays "I had to undo the lockdown sequence," not "I had to find the bolt
  cutters."

**Not yet applied — guidance for the script rewrite phase:**

- **Introduce deliberate messiness into the cross-district chronology.** The crossover documents
  currently resolve a little too cleanly — nearly everyone eventually figures out Vanguard is
  lying. A future pass should preserve some instances of a transmission that never gets through,
  one location misunderstanding something another already knows, Jim learning the answer to a
  question whose asker died never knowing it, or two records that contradict each other because
  neither side had the full picture — so the crossovers feel discovered, not engineered.
- **Per-district storytelling material, not five flavors of memo:** Police = reports/radio/
  procedure; Hospital = bodies/treatment spaces/medical observations; Foundry = machinery/worker
  belongings/records; Academy = human remnants/PA/personal notes (already the locked convention);
  Monastery = architecture/murals/old texts/ritual objects. Worth auditing document choices against
  this table during the script rewrite, alongside the existing document-density concern from the
  narrative craft review.
- **Jim's personal arc should track how deep into Ravenwood he's gone, not just which district
  he's in.** Since district order is open, this should key off **emblem count carried**, not a
  fixed location: early on he's still trying to understand what's happening; by the third emblem
  he's actively connecting things across districts; by the fourth he's stopped being surprised by
  Vanguard; by the fifth he barely reacts to another atrocity — not from apathy, but exhaustion and
  focus. This is a `Scripts/`-level concern (Jim's dialogue/interiority), not a `Locations/`-level
  one, and should be threaded through the same rewrite pass that fixes his over-narration.

## Direction Log (continued) — synchronization pass: canon/doc contradictions (2026-08-14)

> A full-branch audit (Locations, CANON, MASTER_STORY, character material, existing scripts)
> concluded the story design itself is in good shape — most remaining problems are consistency/
> implementation gaps between documents rather than story problems. The verdict: "the branch no
> longer has a story-concept problem, it has a synchronization problem." Everything below was
> either fixed directly in this pass or explicitly logged as the next major task.

**Fixed in this pass:**

- **The Monastery/open-order contradiction — the most important fix.** `CANON.md`/`MASTER_STORY.md`
  lock all five districts as fully open-order, but the Monastery's own material repeatedly called
  itself "the last surface location before Chapter 3" — those two claims can't both be literally
  true if a player visits the Monastery first. **Resolved:** the Monastery stays mechanically
  open-order (visitable anytime, most of it explorable, Faith Crest obtainable whenever reached),
  but its deepest section — the Sealed Passage / Old Caves and Brother Cormac's final broadcast —
  now stays sealed until Jim holds **four or more crests total**, regardless of visit order or
  when the Faith Crest itself was collected. This guarantees the Monastery's revelation always
  functions as the narrative bridge into Chapter 3 without forcing a specific visit order. See
  [`Locations/Monastery.md`](Locations/Monastery.md) and
  [`MASTER_STORY.md`](MASTER_STORY.md).
- **MASTER_STORY.md's "fully scripted" claims corrected.** It previously said Police/Hospital/
  Foundry/Academy were "fully scripted" in one place and "not yet written scene-by-scene" in
  another — genuinely contradictory, and exactly the kind of thing that would mislead a future
  pass into treating the wrong version as canon. Changed to "script exists — puzzle/progression
  rewrite pending" for all four, matching what `CANON.md` and the `Locations/` files already said.
- **Old mandatory key chains removed from Hospital, Foundry, and Academy**, not just flagged as
  superseded — the same treatment already applied to the Monastery. New hard rule applied
  consistently: *the district's signature puzzle carries the mandatory critical path; keys exist
  primarily for optional rooms, shortcuts, supplies, lore, or small subloops.* Concretely: the
  Hospital's Laboratory/Administration/Chapel are now unlocked and the old Radiology → Lab →
  Administration key chain is gone (Radiology's dead orderly now holds a piece of the isolation
  manual instead of a key); the Foundry's Manager's Office and Vanguard Site Office are now
  unlocked (their old keys retired; the Vanguard Site Key now opens only an optional bonus
  cabinet); the Academy's Library and Auditorium are now unlocked, and the Knowledge Crest moved
  from Founder's Hall's display case (now empty, with a note from Ashford explaining why) to the
  Library's own hidden archive, revealed by solving the Archive Puzzle.
- **Five Puzzle Philosophies locked as final**, per explicit direction not to keep reinventing them.
- **CANON.md's mandatory central-hub rule loosened.** All five districts previously had to open on
  "central hub, see several locked points at once," which was itself becoming a repetition risk.
  Now: "a recognizable anchor space or traversal structure the player learns and revisits" — a true
  hub where it fits (Police, Foundry), something else where it doesn't (Hospital's branching
  corridors, the Academy's spreading aftermath, the Monastery's vertical spiral).
- **Jim's Chapter 2 arc locked to crest count**, not district order, with a full 0–5 breakdown (see
  [`Characters/Jim_Mercer.md`](Characters/Jim_Mercer.md)) — Survival → Suspicion → Pattern → Anger
  → Resolve → Acceptance — plus the explicit instruction that his dialogue should thin out, not
  escalate, as the count rises.
- **Zombie Conglomerate presence locked to crest count** instead of random appearance (see
  [`Creatures/Zombie_Conglomerate.md`](Creatures/Zombie_Conglomerate.md)) — distant sighting at 1,
  blocks a street at 2, audible before visible at 3, forces alternate routes at 4, owns portions of
  Downtown at 5.
- **Foundry wording fix.** "The rail yard tracks lead into the mountain — the physical point Black
  Vein entered Ravenwood" contradicted Black Vein being a natural formation that predates any
  human access point. Changed throughout to "the primary modern industrial access point into the
  Black Vein cave network."

**Logged, not yet applied — the next major task:**

- **The Chapter 2 script rewrite itself.** Police Station, Hospital, Foundry, and Academy all have
  existing scene-by-scene scripts written against the old key-hunt mechanics; none has been
  rewritten to match its new puzzle philosophy yet. This is explicitly the largest remaining piece
  of work and should be the next major pass, per the audit's own conclusion: keep adding lore, and
  the risk is the documents drift out of sync faster than they get reconciled.
- **Deliberate messiness in the cross-district chronology**, a per-district storytelling-material
  table, and other script-level items — already tracked above under "puzzle-design refinement
  pass" and "narrative craft review."
- **Locked and not to be redesigned further** (per the audit's own list): Black Vein being natural;
  Vanguard rediscovering rather than creating it; five founders/five crests; the Memorial Park
  mechanism; the Hotel's puzzle; the Five Puzzle Philosophies; each district's thematic identity;
  the interconnected outbreak-night chronology; Jim/Sarah framing; Jim's ambiguous ending; the
  Monastery's historical perspective. Future passes should treat these as settled and focus on
  synchronization (scripts, item files, cross-references) rather than reopening them.
- **A caution worth carrying into the script rewrite:** Vanguard currently touches nearly every
  system in the city (police protocols, hospital infrastructure, Foundry worker monitoring, exposure
  cohort tracking, Academy shelter rosters, Monastery records, tunnel projects, emergency power,
  containment systems, medical retrieval, armed security, communications suppression, government
  pressure). Individually plausible, collectively at risk of reading as "Vanguard scripted every
  moment of the disaster" rather than an organization that exploited a real one. The rewrite should
  let some civic failures be genuinely mundane — panic, storm damage, ordinary bad judgment calls —
  so Vanguard reads as opportunistic rather than omniscient.

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
- **Chapter 2 narrative-craft revision pass** (per "Chapter 2 narrative craft review," above) — not
  yet started. Concretely: (1) narratively disguise the Hospital/Foundry/Academy's shared
  hub-and-locked-doors structure per district without changing the underlying level design, and
  make sure Jim's dialogue never lampshades the repetition; (2) trim ~25–35% of Jim's
  post-document commentary that just restates what the player already read, across all four
  scripted districts; (3) review overall document/evidence density chapter-wide against the "player
  should understand *what* Vanguard did, not exactly *how* Ashen/Black Vein work" ceiling ahead of
  Chapter 3; (4) add a handful of Jim-personal-story beats per district, not only worldbuilding;
  (5) decide what unique piece of the outbreak-night chronology the Monastery alone can know, per
  the "outbreak-night chronology as a five-piece jigsaw" idea above, and thread it into the
  not-yet-written Monastery script; (6) give Jim a personal arc that escalates with emblem count
  rather than fixed district order (still trying to understand → connecting things → no longer
  surprised by Vanguard → barely reacting, from exhaustion not apathy), per "puzzle-design
  refinement pass," above; (7) introduce deliberate messiness into the cross-district crossovers
  (missed transmissions, one-sided misunderstandings, contradictory records) so they read as
  discovered rather than engineered.
- **Dialogue/voice naturalism pass** (per "consistency and declutter pass," above, and echoing the
  narrative-craft review's point about Jim's over-narration) — not yet started. The actual scene
  prose in `Scripts/Chapter_2_{Police_Station,Hospital,Foundry,Academy}.md` (and eventually the
  Monastery's future script) should be reviewed line-by-line for dialogue/description that reads
  as generated rather than written — stilted phrasing, over-explanation, document reactions that
  just restate what was read — and rewritten to sound like something a specific, tired,
  frightened person would actually say. This is a large task best scoped per-district rather than
  attempted in one pass, and should be coordinated with the Jim-over-narration trim already tracked
  above so the two aren't done twice.
- **Five Puzzle Philosophies — script rewrite: COMPLETE for all five districts (2026-08-14).**
  All five `Locations/` files fully describe their new puzzle mechanics, and **all five
  `Scripts/Chapter_2_*.md` files now match them**:
  [`Scripts/Chapter_2_Police_Station.md`](Scripts/Chapter_2_Police_Station.md) (Lockdown Puzzle),
  [`Scripts/Chapter_2_Hospital.md`](Scripts/Chapter_2_Hospital.md) (Quarantine Puzzle),
  [`Scripts/Chapter_2_Foundry.md`](Scripts/Chapter_2_Foundry.md) (Casting Puzzle),
  [`Scripts/Chapter_2_Academy.md`](Scripts/Chapter_2_Academy.md) (Archive Puzzle, with
  [The Matron](Creatures/The_Matron.md) as boss), and
  [`Scripts/Chapter_2_Monastery.md`](Scripts/Chapter_2_Monastery.md) (Bell Tower Puzzle, written
  from scratch since it had no prior script, with [The Penitent](Creatures/The_Penitent.md) as
  boss and a conditional branch at the Sealed Passage depending on crest count). Along the way this
  pass caught and fixed two contradictions the puzzle-design pass itself had introduced (the
  Foundry's Industry Crest existing in two places at once; the Academy's stale Library Key), and
  resolved the Monastery's last open creature question by naming its standard-tier new creature
  **the Cave-Touched** (no dedicated `Creatures/` file yet — inline description only in
  [`Locations/Monastery.md`](Locations/Monastery.md)). All five rewrites trimmed Jim's dialogue and
  removed the old self-aware "same shape as X, different building" lines the narrative review
  flagged.
  **Remaining follow-up work, not yet done:** (1) audit `Items/Key_Items/` for the several retired
  keys flagged inline in each `Locations/` file — delete or repurpose their writeups (Police
  Station's "Armory Zone Override," Hospital's "Backup Damper Control," Foundry's retired
  Manager's Office Key, Academy's retired Library Key); (2) a dedicated dialogue/pacing pass across
  all five scripts applying the narrative-craft review's remaining items in full (Jim's
  over-narration trim was applied loosely during each rewrite but not measured against the
  25–35% target precisely; his crest-count arc should be checked scene-by-scene, not just noted in
  passing; deliberate messiness in crossovers hasn't been added anywhere yet; the per-district
  storytelling-material table hasn't been audited against final document choices; the caution
  against over-attributing every civic failure to Vanguard hasn't been specifically checked); (3) a
  final consistency pass across all five `Locations/` files, checking for the same kind of "two
  answers for one puzzle" drift caught twice during this pass — five districts redesigned quickly
  in sequence makes a third undiscovered slip plausible; (4) give the Cave-Touched a proper
  `Creatures/` file if the Monastery's own bestiary needs more than the current inline description.
- **Creature Distribution System (locked 2026-08-14).** Per the project owner's direction: every
  district has Shamblers themed to that location (police uniforms, hospital gowns, work coveralls,
  shelter clothing, monastic robes), every district's main location has one boss-tier encounter
  (not just the Hospital), and each district's new creature type unlocks into the wider city as a
  roaming hazard once discovered, scaling with crest count the same way the Zombie Conglomerate and
  Jim's own arc do. Bosses assigned: Police Station → **Diesel, the Alpha Ashen Hound** (existing
  creature, promoted to boss scale); Hospital → **The Surgeon** (already locked); Foundry → **The
  Foreman** (new — the Exposure Cohort's longest-exposed member, see
  [`Creatures/Exposure_Cohort.md`](Creatures/Exposure_Cohort.md)); Academy → **The Matron** (new —
  see [`Creatures/The_Matron.md`](Creatures/The_Matron.md), designed to preserve the district's
  "people, not a monster" identity despite overriding its earlier "no new creature type" lock);
  Monastery → **The Penitent** (new — see [`Creatures/The_Penitent.md`](Creatures/The_Penitent.md),
  a monk sealed away centuries ago, tied directly to the district's own locked pre-Vanguard
  backstory). The city-wide unlock mechanic itself (detection, spawn rules, how "sparse at first,
  more often later" actually works) is not yet designed — flagged alongside the Zombie
  Conglomerate's own open combat/detection gaps.

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
