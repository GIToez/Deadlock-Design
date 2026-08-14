# Deadlock Protocol — Canon

> Only important, established facts that must not be casually changed belong here.
> Keep this document concise. Do not duplicate the entire storyline — see [`MASTER_STORY.md`](MASTER_STORY.md)
> for the full narrative.
>
> If another document contradicts this file, report the contradiction rather than silently
> changing canon.

> **Source note:** Two source materials exist for this game:
> [`Deadlock Protocol - Story Design Rebuild.docx`](Deadlock%20Protocol%20-%20Story%20Design%20Rebuild.docx)
> (uploaded first) and [`AI.json`](AI.json) (an older AI planning conversation, uploaded
> second, covering the same material plus much more — Memorial Park, the five districts, the
> crest/emblem system, and character names). Where the two disagree, **[`AI.json`](AI.json) is treated as the
> newer, more authoritative source**, because it is a later iterative pass that explicitly revisits
> and fixes problems found in the earlier material (see "Retcons" below for the specific list).

## Presentation & Perspective

Deadlock Protocol is a **2.5D top-down survival horror game** (this was stated as early as the
first message of `AI.json`'s planning conversation but never actually made it into a design
document until now — flagging that gap here for traceability). Two concrete implications for
future writing, confirmed by reference screenshots from the project owner (2026-08-12):

- **The camera does not show a wide, cinematic view of a room.** It stays close to the player
  character — in the reference screenshots, roughly half of the Ravenwood Hotel lobby is visible
  at once, not the whole room. Scene descriptions should generally reflect what's near/visible to
  Jim as he moves, not an omniscient wide shot of an entire space, unless a moment is explicitly
  meant to be a wider vista/cutscene beat (e.g. the Overlook Trail scene in Chapter 2, which is
  already written as a deliberate, singular exception).
- **There is no implied 3D camera movement** (pans, dollies, over-the-shoulder shots, etc.).
  Description should read as what's visible from a fixed top-down/isometric perspective near the
  player, not as film-style shot direction.
- This does not mean characters/creatures lack visual detail on-screen — the reference
  screenshots show clearly readable character and creature sprites (clothing, posture, attack
  animation) even at this camera distance — it specifically means **scale of visibility**, not
  detail fidelity, is the thing to watch for in future prose.

See [`README.md`](README.md) → "Presentation & Camera" for the corresponding writing rule, and
[`Assets/`](Assets/README.md) for reference screenshots once uploaded.

## District Main-Location Design Standard (locked 2026-08-13; puzzle-mechanic clause revised 2026-08-14)

Each of the five districts' **main location** (Police Station, Hospital, Academy, Refinery,
Monastery) is a substantial, interconnected exploration space — explicitly modeled on classic
survival-horror "mansion/police station" density (Resident Evil's Spencer Mansion and RPD are the
direct reference points for *scope and interconnection*, not for the specific mechanic every
district should use), not a short, mostly-linear pass. Concrete implications:

- **Target scope: roughly 2–3 hours of gameplay per main location** — comparable in depth to the
  Ravenwood Hotel (Chapter 1's 46-scene main location), not to the shorter, faster secondary
  locations within the same district.
- **Each district's puzzle mechanic must be distinct — see "Five Puzzle Philosophies," below
  (revised 2026-08-14).** The original version of this standard called for "multiple specific key
  items... the way RE's suit-symbol keys each open exactly one thing" uniformly across all five
  districts. That's now explicitly **not** the standard — a uniform key-hunt across all five
  districts was identified as a repetition risk (see [`STORY_NOTES.md`](STORY_NOTES.md) → "Chapter
  2 narrative craft review"). The Hotel's repair-and-backtrack puzzle is the **benchmark to differ
  from**, and each of the five crest locations gets its own puzzle philosophy built from something
  unique to that institution (see below) — physical keys are still fine as *one ingredient* within
  a district's mechanic (the Police Station's Lockdown puzzle still uses a few), but no district
  should be a pure "find the item shaped like the lock" hunt end to end.
- **Backtracking across the whole district is still the point, not a flaw.** A main location's
  secondary locations (e.g. the Police Station's Fire Station, Municipal Garage, City Courthouse)
  should stay woven into the same interlocking puzzle, not fully separate optional side content —
  clues/tools found at one building should often be required to progress at another, forcing the
  player to physically walk the district multiple times.
- **A recognizable anchor space or traversal structure the player learns and revisits** (loosened
  2026-08-14 from a stricter "every district needs a central hub that visibly gates several locked
  points at once" rule, which was itself becoming a repetition risk — five districts each opening
  on "enter foyer, catalogue locked doors" reads as the same rhythm even with different puzzles
  behind it). A true hub is still the right shape where it fits the institution — the Police
  Station's security console genuinely belongs in one room, and the Foundry's seized casting line
  is naturally a hub by virtue of dominating the room it's in. Other districts can use a different
  shape entirely: a branching corridor system the player gradually gets swallowed by (the
  Hospital), a spreading complex explored by following an aftermath outward rather than sizing up
  a foyer (the Academy), or a vertical progression the player spirals through (the Monastery's
  Chapel → Cloister/Library → Bell Tower → Crypt). What must stay true regardless of shape: the
  player should be able to see, at some point before the end, roughly how much of the district is
  left to solve.
- **The emblem itself is the last thing found**, behind the deepest/most gated point of the
  location — a reward for finishing the loop, not something encountered early or in passing.
- This standard is **retroactive**: the Police Station, originally scripted before this standard
  was locked, has since been rewritten to match it (2026-08-13) and fully scene-by-scene scripted —
  [`Scripts/Chapter_2_Police_Station.md`](Scripts/Chapter_2_Police_Station.md), Scenes 1–24,
  including a full room-connectivity blueprint at
  [`Locations/Police_Station.md`](Locations/Police_Station.md) matching
  [`Locations/Ravenwood_Hotel.md`](Locations/Ravenwood_Hotel.md)'s existing convention. St. Dymphna
  Hospital, Steelgate Refinery, and Worthy Academy have since received the same treatment
  ([`Scripts/Chapter_2_Hospital.md`](Scripts/Chapter_2_Hospital.md),
  [`Scripts/Chapter_2_Foundry.md`](Scripts/Chapter_2_Foundry.md),
  [`Scripts/Chapter_2_Academy.md`](Scripts/Chapter_2_Academy.md)); the one remaining district (the
  Monastery) should be written to the same bar (dense main location, a full blueprint, its own
  standalone script file) from the start, built directly around its own puzzle philosophy below
  rather than a key hunt. See [`STORY_NOTES.md`](STORY_NOTES.md) for the full restructuring
  history — **as of 2026-08-14, the four already-scripted districts' `Scripts/` files still
  reflect the old key-hunt mechanic and have not yet been rewritten to match the puzzle
  philosophies below; only the Police Station's `Locations/` file has been updated so far.**

### Five Puzzle Philosophies (locked 2026-08-14)

Each crest location uses a mechanic built from something unique to that institution, with its own
interaction verb — full design detail for each is in
[`STORY_NOTES.md`](STORY_NOTES.md) → "Five Puzzle Philosophies":

| Location | Puzzle | Verb |
|---|---|---|
| Ravenwood Hotel (benchmark, already built) | Auxiliary power repair-and-backtrack | Repair |
| Police Station | Emergency security lockdown — undo the department's own self-triggered lockdown in the correct sequence | Route / Unlock |
| St. Dymphna Hospital | Negative-pressure quarantine — create safe pressure gradients through sealed isolation zones | Contain |
| Steelgate Refinery | Industrial casting line — operate furnace, crane, and cooling stages to free the crest from a seized mold | Operate |
| Worthy Academy | Ravenwood historical archive — reconstruct the true founding chronology to open a hidden mechanical catch | Understand |
| Our Lady of Solace Monastery | Ancient bell/counterweight mechanism — interpret non-numeric clues into the correct bell-ringing order | Interpret / Activate |

Beyond avoiding repetition, each puzzle also teaches the player something true about Ravenwood
just by being solved: the Hotel teaches exploration, the Police Station teaches how the town was
controlled, the Hospital teaches how Ashen behaves, the Foundry teaches where the problem
physically came from, the Academy teaches Ravenwood's history, and the Monastery teaches that
Ravenwood's connection to what lies underground predates Vanguard.

## Fundamental Premise

Deadlock Protocol follows **Jim Mercer** — retired military (communications/logistics), now a
civilian **telecommunications field engineer** for a regional contractor — traveling alone through
rural Appalachia during a severe storm, headed to a relay site that has been offline for three
days. Flooding and poor visibility force him off Highway 13 into the isolated mountain town of
**Ravenwood**, where he checks into the **Ravenwood Hotel** for what he believes will be a single
overnight stay. The town has already begun collapsing due to an outbreak, and the game escalates
from grounded, slow-burn horror into full quarantine horror over the course of one night.

## Player Starting Equipment

Jim carries a **heavy-duty flashlight** clipped to his belt from the very start of the game — part
of his default loadout as a field engineer's everyday-carry, not something picked up in play. This
was locked (2026-08-12) specifically to close a gap where he had no personal light source for
Chapter 1's dark, powerless spaces despite the hotel's outage. Established in
[`Scripts/Chapter_1_One_Night_Only.md`](Scripts/Chapter_1_One_Night_Only.md) (Scene 2); Chapter 2's
originally-planned "first flashlight" pickup ([`Scripts/Chapter_2_Ravenwood.md`](Scripts/Chapter_2_Ravenwood.md), Scene 2) was
changed to spare flashlight batteries instead, since he already has his own.

## Origin of the Outbreak

The collapse of Ravenwood is tied to an outbreak connected to **Vanguard BioSystems** and
**"Project Ashen."** The mutagen/infectious agent is named **Black Vein**. Ravenwood and Vanguard
share the same five founders (see "The Founders & the Five Crests" below) — the town was not an
incidental host; it was built by the same people who built Vanguard, and the underground facility
beneath Memorial Park was constructed at the same time as the town itself (1887). The exact
mechanism of the outbreak (how containment failed, why it happened now) is not yet established —
see [`STORY_NOTES.md`](STORY_NOTES.md).

**Black Vein is a natural formation, not something Vanguard manufactured or imported (proposed
2026-08-13, pending review).** It runs through the natural cave system beneath the mountains
around Ravenwood — the 1887 Memorial Park facility was built directly on top of it as the town's
original, oldest access point. A second, later access point was established at
**[Steelgate Refinery](Locations/Foundry_Refinery.md)** starting in **1968**, when Vanguard began
using the working industrial site as long-term cover to excavate toward the same vein network from
a different direction. The two sites are **not physically connected** — Vanguard deliberately
compartmentalized them, so nothing Jim finds/experiences at the Foundry in Chapter 2 provides a
shortcut into Chapter 3's facility, or vice versa. This means Ravenwood's outbreak has two
supporting origin threads rather than one: the original 1887 facility (Chapter 3's reveal) and a
separate, decades-long industrial exploitation/exposure operation at the Foundry (see
[`Locations/Foundry_Refinery.md`](Locations/Foundry_Refinery.md) → "Outbreak Night"), both
converging on the same underlying phenomenon.

**Ravenwood encountered Black Vein's effects generations before either Vanguard access point
existed (proposed 2026-08-13, pending review).** [Our Lady of Solace Monastery](Locations/Monastery.md),
built on the northern ridge around a natural spring and cave system centuries before the modern
town, documented strange occurrences in its own archives — malformed/aggressive animals, unnaturally
rapid wound healing, hardened growths, survivable injuries that should have been fatal — long
before anyone had the scientific language to describe them, recorded instead as religious/folkloric
language ("The Mercy That Should Not Be Asked For," "the stone that mends wrongly"). At some
unrecorded point, the monks deliberately sealed the deepest of those caves and let the practical
memory fade into forbidden-crypt tradition. This makes the Monastery's ridge caves a **third,
much older point of human contact with the same underlying cave system** — distinct from, and
originally unconnected to, both the 1887 Memorial Park facility and the 1968 Foundry excavation.
Vanguard later obtained the monastery's historical archives (see
[`Locations/Monastery.md`](Locations/Monastery.md) → "Outbreak Night") and covertly tunneled from
the Foundry side to bypass the monks' old seal entirely — the only case where two of Ravenwood's
Black Vein sites become physically connected, and only because Vanguard deliberately built that
connection. This does not change the 1887/1968 sites' own compartmentalization from each other,
above; it adds a third thread, reframing Vanguard's culpability from "made an unforeseeable
scientific discovery" to "found generations of documented warnings, understood them, and proceeded
anyway."

## Major Character Relationships

- [Jim Mercer](Characters/Jim_Mercer.md) is married/partnered to
  **[Sarah Mercer](Characters/Sarah_Mercer.md)** ("love you" is exchanged on both sides of
  every call). Sarah is off-site for the events of the game, reachable only by phone during the
  drive and at the hotel parking lot — after that, **Deadlock Protocol cuts all external
  communication in and out of Ravenwood**, and there is no contact between them for the rest of
  the game. The whole game takes place over one night; Sarah is asleep for most of it, unaware.
- Late in the game, before descending into the underground facility (Chapter 3), Jim finds a way
  to send **one outbound message** to Sarah — one-sided, he doesn't know if it gets through. He
  sends it anyway.
- Sarah arrives in Ravenwood days later, looking for Jim — this is the game's **Epilogue** and a
  sequel hook (the intended sequel would be played from Sarah's perspective).

## Major Story Structure

The story is told in three chapters plus an epilogue:

1. **Chapter 1 — One Night Only.** The Ravenwood Hotel (absorbs what earlier material called the
   "Prologue" — driving in, checking in, the outbreak beginning — the whole thing is now Chapter
   1, not a separate prologue). Opens on Highway 13; closes on Jim stepping through the hotel's
   north courtyard gate onto the street.
2. **Chapter 2 — Ravenwood.** The city. Jim crosses the street into Memorial Park (the permanent
   safe hub), then explores five open-order districts recovering five founders' emblems. Closes
   on all five emblems being returned to the Founders Memorial statue, the water basin draining,
   and a hidden staircase being revealed.
3. **Chapter 3 — What Was Hidden.** The underground Vanguard facility beneath Memorial Park.
   Project Ashen and Black Vein are revealed. Jim sends his one message to Sarah before the
   finale. The facility is destroyed (or partially destroyed). **Jim's fate is left deliberately
   ambiguous.**
4. **Epilogue — One More Night.** Sarah arrives at the outskirts of Ravenwood days later, looking
   for Jim, and goes through the quarantine perimeter anyway. No resolution of Jim's fate — a
   clean hook for a sequel starring Sarah.

See [`MASTER_STORY.md`](MASTER_STORY.md) for the full progression and [`Locations/Ravenwood_Hotel.md`](Locations/Ravenwood_Hotel.md) for complete
hotel-chapter detail.

## The Founders & the Five Crests

- **[Memorial Park](Locations/Memorial_Park.md)** (est. 1891 per its own archway; the central
  Founders Memorial statue is dated 1887 — the statue predates the park's formal establishment, or
  the park was built around it — not yet reconciled, see [`STORY_NOTES.md`](STORY_NOTES.md)) is
  Ravenwood's central hub, reached directly across the street from the
  [Ravenwood Hotel](Locations/Ravenwood_Hotel.md).
- At its center stands the **Founders Memorial**: a ~10-foot bronze female civic statue holding a
  large circular medallion-plaque, divided into a small central **five-sided pentagon hub**
  surrounded by **five trapezoidal wedge-shaped recesses** arranged like a compass rose (one wedge
  sits due north/top, the rest spaced evenly around it at the other four confirmed directions).
  Inscription: *"WHAT WAS DIVIDED SHALL BE WHOLE. WHAT WAS HIDDEN SHALL BE OPENED. — THE FOUNDERS
  OF RAVENWOOD — 1887 —"* Each recess bears a faint engraved label: **ORDER, KNOWLEDGE, INDUSTRY,
  FAITH, MEDICINE.** The small central hub bears a single weathered letter **"V"** — an
  unexplained, deniable early visual hint at the Vanguard connection, sitting in plain sight on an
  1887 civic monument. See concept art:
  [`Assets/Reference/founders_memorial_plaque_concept.png`](Assets/Reference/founders_memorial_plaque_concept.png)
  (two wedges shown filled, three shown empty, for reference — not a literal screenshot). The
  statue sits in a water basin; draining the basin (by filling all five recesses) reveals a
  submerged door/staircase beneath it, descending into the Vanguard facility.
- **Each of the five founders built one civic institution and kept one emblem.** The five
  founders of Ravenwood are the same five founders of Vanguard BioSystems — the town and the
  company are one shared history, not two that later collided.
- **Each emblem is a separate, physical wedge-shaped piece that inserts into and completely fills
  its matching recess** — not a marking that appears on the existing stone, but a distinct object
  slotted into an empty socket, like a puzzle piece. Once inserted, a visible seam/lip remains
  where the emblem's edge meets the surrounding medallion frame, so it always reads as something
  placed there rather than part of the original surface. Each emblem bears a relief portrait of
  its founder, the founder's name, and a symbol of their institution. They were made together with
  the statue as the facility's original (crude, deliberate) access control system; over
  generations the original purpose was forgotten and the emblems became civic artifacts, kept out
  of tradition. A short founding-record document at the Academy covers this in-world.
- **The directional hint lives in the statue's empty wedge slots, not in the emblems themselves.**
  Each wedge's position on the medallion (top/north, upper-right/northeast, lower-right/southeast,
  lower-left/southwest, upper-left/northwest) points in the general compass direction of the
  district its emblem belongs to. Jim can read this directly off the statue at Memorial Park at
  any time, before collecting anything — it's a hint built into the monument itself, not something
  revealed only after finding a given emblem.
- **Crest / district / slot reference table:**

| Direction | Crest Name | Location | Statue Slot Label | Institution Symbol | Wedge Position |
|---|---|---|---|---|---|
| North | Faith Crest | [Our Lady of Solace Monastery](Locations/Monastery.md) | FAITH | Cross | Top |
| Northeast | Medical Crest | [St. Dymphna Hospital](Locations/Hospital.md) | MEDICINE | Serpent/Caduceus | Upper-right |
| Southeast | Knowledge Crest | [Worthy Academy](Locations/Academy.md) | KNOWLEDGE | Torch | Lower-right |
| Southwest | Authority Crest | [Ravenwood Police Station](Locations/Police_Station.md) | ORDER | Key | Lower-left |
| Northwest | Industry Crest | [Steelgate Refinery](Locations/Foundry_Refinery.md) | INDUSTRY | Anvil | Upper-left |

- **The Faith Crest's founder, Abbot Matthias Kane, did not found the Monastery building itself —
  he formally established its current religious order in 1887 (proposed 2026-08-13, pending
  review).** Per [`Locations/Monastery.md`](Locations/Monastery.md), the physical monastery, its
  spring, and its cave system predate the founders' era by centuries; Kane's 1887 role (matching
  the other four founders' own institution-founding year) was consolidating and formally
  chartering "Our Lady of Solace" as the monastery's modern order atop that much older site,
  which is why he's credited on the Faith Crest despite the building predating him — a deliberate,
  flagged reconciliation, same convention as Memorial Park's own unresolved 1887/1891 date
  tension (see [`STORY_NOTES.md`](STORY_NOTES.md)).
- Jim learns about the emblems through **environmental discovery, not exposition**: guardhouse
  notes at Memorial Park (written by a park groundskeeper who never understood the statue, but
  recalls a historian once telling him to "look at the police station... there's something on the
  wall inside the main hall") plus finding the first emblem himself at the Police Station — the
  natural first destination, being closest to the park.
- District exploration order is **fully open** from the start of Chapter 2. The single unlocked
  south park gate creates only a soft suggestion (Police Station first), never a hard requirement.

## VERN Terminals

**VERN** = *Vanguard Emergency Response Node*. VERN terminals are a **city-wide save-point
network** found throughout Ravenwood (not hotel-specific) — the game's only save mechanic. They
are part of pre-existing Ravenwood emergency infrastructure, which itself is a subtle, unexplained
early hint that Vanguard's reach into the town predates the outbreak.

## Vanguard's Grip on Ravenwood PD (proposed 2026-08-13, pending review)

> Proposed by the project owner as a deliberate reframe of the Police Station: **the officers are
> not secretly Vanguard villains.** They're real Ravenwood cops who believe they're protecting
> their town. Vanguard spent years turning the department into an unofficial containment arm
> without most officers realizing how far they'd already crossed the line. See
> [`Locations/Police_Station.md`](Locations/Police_Station.md) for where this is physically
> discovered in-game, and [`Characters/Aaron_Cole.md`](Characters/Aaron_Cole.md) for the detective
> whose investigation is the primary discovery trail. Treat this whole section as a proposal
> pending full review, same as any new canon addition — but built to not contradict anything
> already locked (Sergeant Calloway, the shotgun, the Authority Crest, Diesel/Baxter, and all four
> buildings are all explicitly unchanged).

- **The Ravenwood–Vanguard Public Safety Agreement.** Years before the outbreak, Vanguard began
  funding the Ravenwood Police Department — not cartoonishly, but through completely reasonable-
  looking support: new cruisers, upgraded radios, body armor, station renovations, overtime
  reimbursement, medical coverage, donations to injured officers' families, and a Vanguard-funded
  emergency-response training program. A small town's department became quietly dependent on that
  money — Vanguard ends up effectively owning the department's emergency-response capability
  without ever technically owning the department itself.
- **The Vanguard Public Safety Liaison Program.** A non-sworn Vanguard liaison is permanently
  stationed inside the police station, with his own office — and, per department legend, a badge
  that opens more doors than the Chief's. Not yet named; his own fate on the night of the outbreak
  is deliberately unresolved (see `Locations/Police_Station.md`).
- **V-CASE classification.** Police are never told what Black Vein actually is. Vanguard trains
  officers to recognize "acute industrial neurochemical exposure resulting in violent psychosis" —
  anyone displaying specific symptoms is classified a **V-CASE (Vanguard Containment Case)** and
  stops being treated as an ordinary citizen: isolated, restrained, kept away from hospitals,
  handed directly to a Vanguard response team, filed under a generic public-intoxication/
  psychiatric-hold charge, with body-camera footage destroyed or sealed. Officers believe Vanguard
  is taking these people for specialized medical treatment. They're actually being fed into
  **Project Ashen**.
- **The Cold Cells.** The station's old basement holding area — originally drunk tanks and
  evidence storage — was quietly renovated by Vanguard (officially "TEMPORARY MEDICAL HOLDING,"
  nicknamed "the Cold Cells" by the cops): heavy steel doors, floor drains, no windows, restraint
  rings built into the walls, negative-pressure ventilation, all Vanguard-supplied. V-CASEs were
  held there until Vanguard arrived at night and the prisoner disappeared — no transfer paperwork,
  no court appearance, no hospital record. See `Locations/Police_Station.md` for its in-game
  placement (gated behind a **Vanguard Access Card**, not part of the mandatory Authority Crest
  chain).
- **The confidential watchlist.** Vanguard supplies the department a watchlist of people flagged
  for repeated hospital visits, unusual injuries, neurological symptoms, mine/refinery employment,
  homelessness, or reporting strange things near Vanguard property — framed to officers as
  possible industrial theft/sabotage suspects. During routine stops, officers check names against
  it and radio a code (e.g. *"Dispatch, confirm a 13-Black"*) if there's a match; Vanguard is
  notified and sometimes requests a hold. The department has unknowingly spent years feeding
  people into Project Ashen this way.
- **Vanguard's own interrogation room.** An ordinary-looking interview room (table, two chairs,
  camera, one-way glass) conceals a small Vanguard control booth behind the observation glass —
  medical equipment, injectors, blood-collection supplies, restraints hidden under the chair.
  Vanguard requested certain suspects be questioned there, ostensibly gathering information about
  "industrial accidents." In fact, some of the "interrogations" were testing whether extreme
  stress can trigger Black Vein exposure symptoms — experiments, not interviews.
- **The town as a field study.** In neighborhoods near Black Vein contamination zones,
  Vanguard-directed police to *increase* patrols rather than evacuate — deliberately gathering data
  on how early-stage exposure affects aggression under environmental stress, while residents'
  complaints about strange behavior were dismissed by the department itself as an ordinary drug
  problem. **This is offered as a strong contributing thread toward the still-open "how containment
  failed / why now" question** (see "Origin of the Outbreak," above) — plausible, not a full
  answer; the exact mechanism remains explicitly reserved for Chapter 3.
- **Discovery trail:** primarily [Detective Aaron Cole's](Characters/Aaron_Cole.md) abandoned
  investigation — missing-persons cases he connected via the shared "V-CASE TRANSFERRED" marking,
  a Vanguard security image proving at least one "transferred" person was still alive but
  monstrously mutated, and his own disappearance after Vanguard used an internal-affairs
  investigation to discredit and remove him rather than risk a more visible move against him. Per
  the game's established "environmental discovery, not exposition" convention (see "The Founders &
  the Five Crests," above), this is meant to be pieced together through found documents/notes, not
  delivered via an NPC dialogue dump.

## Named Characters Confirmed (beyond the core hotel cast)

- **[Della Marsh](Creatures/Della_Marsh.md)** ("Della M." on stage) — the Red Room lounge singer;
  local Ravenwood performer, four-year weekly residency. Infected/deceased by the time Jim finds
  her.
- **Roy Bullock** — real name of "[the Caretaker](Creatures/The_Caretaker.md)," the hotel's
  longtime maintenance man, mutated by the outbreak. The hotel had **no direct Vanguard
  presence** — it was simply caught in the outbreak's radius like the rest of town.
- **[Officer Dale Pruitt](Characters/Dale_Pruitt.md)** — Ravenwood PD, night shift; the same
  officer seen at the hotel parking lot at the start of the game and later found infected inside
  the crashed cruiser. The person he pulled over in the parking lot was already in early
  infection stages (his exposure point); that person is never named or seen clearly and remains
  anonymous.
- **[Fennimore](Characters/Fennimore.md)** — the hotel's night-shift security guard. Never seen
  alive; found dead near the courtyard's north gate after chaining the maintenance shed shut on
  discovering Roy Bullock transforming. Reanimates and is fought as a Shambler when Jim returns to
  the courtyard. His full first name is never confirmed on-screen.
- **[Sergeant Ruth Calloway](Characters/Ruth_Calloway.md)** — Ravenwood PD desk sergeant; the
  Southwest District's Tier 2 conditional survivor (see "Survivor System," below). Alive and
  interactive if the Police Station is Jim's first district; already turned otherwise.
- **[Corporal Eli Reyes](Characters/Eli_Reyes.md)** — Ravenwood PD's K-9 unit handler. Never seen
  alive; found dead in the station's K-9 Unit Room, the Armory Key still on his belt, killed by his
  own K-9 partners (see Ashen Hound, below) after they turned.
- **[Detective Aaron Cole](Characters/Aaron_Cole.md)** — Ravenwood PD detective who secretly
  investigated Vanguard's role in a string of local disappearances; discredited via an internal-
  affairs setup and disappeared before the outbreak. Never seen alive or dead — known only through
  his abandoned office and the investigation he hid from Vanguard. See "Vanguard's Grip on
  Ravenwood PD," above.
- **Chief Marcus Doyle** — Ravenwood PD's chief of police (name decided 2026-08-13, needed for his
  self-identification in the final-broadcast recording found in Records/Dispatch — see
  [`Scripts/Chapter_2_Police_Station.md`](Scripts/Chapter_2_Police_Station.md), Scene 5). Never seen
  alive or dead; known through his own Chief's Office logbook (last entry: going to check on Corporal Reyes
  himself) and that recording (publicly overriding Vanguard's containment order, ending on gunfire
  and static). His ultimate fate stays deliberately unresolved, same convention as Cole and the
  Vanguard Liaison. Deliberately distinct from "CHIEF E. WHITAKER," an unprompted, non-canonical
  nameplate that appeared in one AI-generated Chief's Office room concept — see
  [`Locations/Police_Station.md`](Locations/Police_Station.md) for that flag.
- **Marshal Josiah Hale** — the Ravenwood Police Department's first peace officer (1887); one of
  Ravenwood/Vanguard's five founders. His name and portrait appear on the **Authority Crest**,
  recovered from a display case in the old 1887 station house.
- **Dr. Nathaniel Voss** — St. Dymphna Hospital's founding physician (1887); one of
  Ravenwood/Vanguard's five founders. His name and portrait appear on the **Medical Crest**,
  recovered from a display case in the hospital's own chapel — see
  [`Locations/Hospital.md`](Locations/Hospital.md).
- **Elias Thorne** — Steelgate Refinery's founder (1887); one of Ravenwood/Vanguard's five
  founders. His name and portrait appear on the **Industry Crest**, recovered from a display case
  in the Refinery's own founder's boardroom — see
  [`Locations/Foundry_Refinery.md`](Locations/Foundry_Refinery.md). The remaining two founders'
  names are not yet decided (a damaged in-world document at the Police Station defers them
  intentionally — see [`Locations/Police_Station.md`](Locations/Police_Station.md)); when chosen,
  they should feel consistent with Hale's, Voss's, and Thorne's period-appropriate naming.
- **Plant Manager Daniel Fitch** — Steelgate Refinery's manager on the night of the outbreak; a
  Vanguard collaborator by omission for years (confidentiality agreements, ignored irregularities)
  rather than by malice, who breaks with Vanguard once he understands what "evacuation poses an
  unacceptable contamination risk" actually means. See
  [`Locations/Foundry_Refinery.md`](Locations/Foundry_Refinery.md) → "Outbreak Night." His
  ultimate fate is deliberately unresolved, same convention as the Police Station's Chief and the
  Hospital's Liaison.
- **Eleanor Worthy** — Worthy Academy's founder (1887); one of Ravenwood/Vanguard's five founders,
  the source of the school's own name. Her name and portrait appear on the **Knowledge Crest**,
  recovered from a display case in the Academy's own Founder's Hall — see
  [`Locations/Academy.md`](Locations/Academy.md).
- **Principal Diane Ashford** — Worthy Academy's principal on the night of the outbreak, the
  closest thing the shelter has to a single leader across its ensemble of teachers, officers, and
  parents; makes the Academy's final, unanswered emergency broadcast. See
  [`Locations/Academy.md`](Locations/Academy.md) → "Outbreak Night." Her ultimate fate is
  deliberately unresolved, same convention as Fitch, the Police Station's Chief, and the
  Hospital's Liaison.
- **Abbot Matthias Kane** — Our Lady of Solace Monastery's founder (1887, in the reconciled sense
  described under "The Founders & the Five Crests," above — the monastery building and caves
  predate him by centuries). His name and portrait appear on the **Faith Crest**, recovered from
  the Monastery's own Reliquary — see [`Locations/Monastery.md`](Locations/Monastery.md). **All
  five founders' names are now established:** Josiah Hale (Order), Nathaniel Voss (Medicine),
  Elias Thorne (Industry), Eleanor Worthy (Knowledge), and Matthias Kane (Faith).
- **Brother Cormac** — the Monastery's senior monk and archivist on the night of the outbreak; the
  one who secretly built the hidden archive proving Vanguard's decades of documented Black Vein
  warnings, and who stays behind to keep the old crypt seal closed and the archive out of
  Vanguard's hands. See [`Locations/Monastery.md`](Locations/Monastery.md) → "Outbreak Night." His
  ultimate fate is deliberately unresolved, same convention as Fitch, Ashford, the Police
  Station's Chief, and the Hospital's Liaison.
- (The character/founder additions above are new as of 2026-08-13 — see
  [`Scripts/Chapter_2_Police_Station.md`](Scripts/Chapter_2_Police_Station.md), Scenes 1–24, and
  [`STORY_NOTES.md`](STORY_NOTES.md) for context on what was proposed versus already locked.)

## Creature Classification: Ashen Mutant

**[The Maw](Creatures/The_Maw.md)** — a heavily mutated, territorial stalker/ambush predator
encountered in the Ravenwood Hotel, classified as an "Ashen Mutant" — is the first confirmed
example of this classification tier. It's responsible for both Cindy Sweets' Room 106 abduction
and Gerta's death. Whether "Ashen Mutant" applies more broadly (e.g. to the Caretaker) is not yet
confirmed.

**[Ashen Hound](Creatures/Ashen_Hound.md)** — a distinct, separate classification (new,
2026-08-13): Black Vein's presentation in an infected animal (specifically a domestic dog) rather
than a human, producing a fast, pack-hunting profile instead of the slow "Ashen Mutant"/Shambler
baseline. Shares the "Ashen" naming convention (tied to Black Vein's visual/thematic signature) but
is not itself a variant of "Ashen Mutant," which this document uses specifically for human
mutation-stage creatures.

## Creature Classification: Apex Mutation

**[The Zombie Conglomerate ("the Zombie King")](Creatures/Zombie_Conglomerate.md)** — a new,
separate classification tier (proposed 2026-08-13): a mass of dozens (eventually many more)
individually-infected bodies fused together by unchecked Ashen mutation into a single rolling,
grasping entity, "not born, but built." Unlike every other creature so far, it is explicitly
**unkillable and un-fightable by design** — a roaming, unpredictable environmental hazard rather
than a combat encounter, first appearing in Chapter 2 after Jim recovers his first emblem. See its
file for a locked-canon conflict in its source concept art (an incompatible multi-week sighting
timeline) and a proposed resolution, not yet approved.

## Survivor System (design rule, applies from Chapter 2 onward)

- **Tier 1 — Key story survivors:** a small number of fully developed characters, essential to the
  narrative, whose existence and role are fixed regardless of player action.
- **Tier 2 — Conditional survivors:** existence/condition/fate depends on player sequencing.
  Confirmed example: **[Sergeant Ruth Calloway](Characters/Ruth_Calloway.md)**, the Police
  Station's desk sergeant, is alive (interactive, has information) if Jim visits the Police Station
  first; if Jim visits another district first, she has turned by the time Jim reaches the station.
  Rule: the player always gets the needed information either way (directly from the survivor, or
  via notes/environmental clues from the dead version); no survivor's death ever hard-blocks
  progression; the game never explicitly blames the player. (Her alternate/"already turned" scene
  is described but not yet scripted — see [`Locations/Police_Station.md`](Locations/Police_Station.md).)
  - **Tier 2b — Threshold conditional survivors (new, 2026-08-13):** a variant gated by *how many
    emblems Jim is carrying* rather than strictly "first district visited or not." Confirmed
    example: **[Richard Dalton](Characters/Richard_Dalton.md)**, at St. Dymphna Hospital, is alive
    (Jim meets him fleeing the building looking for help for Maria) if the Hospital is Jim's first
    or second district (i.e. he's carrying zero or one emblem on arrival); if Jim already holds two
    or more emblems, Richard has already run out and been killed, and Jim finds his body instead.
    Same underlying rule as Tier 2 above (information/outcome is always recoverable either way, no
    hard-blocked progression) — the only difference is the specific condition checked.

## Retcons — superseded docx content (per [`AI.json`](AI.json), the newer source)

These items appeared in [`Deadlock Protocol - Story Design Rebuild.docx`](Deadlock%20Protocol%20-%20Story%20Design%20Rebuild.docx) and have been explicitly
revised or removed in the later [`AI.json`](AI.json) planning pass. Recorded here rather than silently
changed, per the "report contradictions" rule:

- **Earl Whitaker's pre-outbreak "hesitation"/foreshadowing** (listening for something, his
  dismissal "landing wrong") is removed. Earl is now written as a plainly ordinary, unsuspecting
  night clerk with no foreknowledge — his death is meant to land harder *because* he was never
  suspicious. His "town gets strange when the weather turns" line is likewise cut as a horror
  cliché.
- **The muffled scream** Jim hears before falling asleep in Room 104 is removed from canon — Room
  104 now ends on rain/thunder/fade-to-black with no warning before the outbreak wakes him.
- **The East Wing maintenance-closet/screwdriver duplication** (flagged independently during this
  project's own audit, and by the user during the [`AI.json`](AI.json) session) is resolved the same way in
  both places: **one pickup only, in the East Wing** (matches what's already written in
  [`Locations/Ravenwood_Hotel.md`](Locations/Ravenwood_Hotel.md)).
- **The Red Room no longer connects to the Courtyard Security Office.** In the docx, the Red
  Room's backstage was the route into the Security Office (making it secretly mandatory despite
  being labeled optional, and architecturally implausible — a security office reachable only
  through a speakeasy lounge). This is fixed: the **Red Room is fully self-contained**, entered
  directly off the Main Bar, with no backstage route to anywhere, and the **Courtyard Security
  Office is reached via a separate West Wing service corridor.** The "deadbolted front door"
  detail from the docx is removed entirely — see
  [`Locations/Ravenwood_Hotel.md`](Locations/Ravenwood_Hotel.md) for the corrected room layout.
- Jim's occupation (**not established at all in the docx**) is now locked: retired military
  (comms/logistics) turned telecommunications field engineer.
- The mutagen name is locked as **Black Vein** (a "Dark Vein" variant name was briefly considered
  and rejected in favor of the original term).
- **The hotel's second-floor service crossover and "West Wing Maintenance Office" are retired
  (2026-08-12).** This was an interim design (written into this project's own scripts, not sourced
  from the docx or [`AI.json`](AI.json)) that assumed a player-inaccessible service floor
  connecting the East and West Wings. After the project owner shared a real architectural floor
  plan for the hotel (ground floor + guest floor only), the entire East/West Wing
  power-restoration route was rebuilt to match: no second floor, no crossover, a barricaded
  East Wing shortcut door back to the Lobby, and a small unlocked **West Wing Maintenance Room**
  on the guest floor (not the old "West Wing Maintenance Office," which is gone). The **Laundry
  Room also moved from the West Wing (behind the Main Bar) to the East Wing**, next to the Utility
  Room — Gerta's death scene moved with it. See [`STORY_NOTES.md`](STORY_NOTES.md) → "Direction
  Log" for the full resolution and [`Locations/Ravenwood_Hotel.md`](Locations/Ravenwood_Hotel.md)
  for the corrected room list and blueprint diagrams.

*Sources: [`Deadlock Protocol - Story Design Rebuild.docx`](Deadlock%20Protocol%20-%20Story%20Design%20Rebuild.docx) (original material); [`AI.json`](AI.json) (the
planning conversation that produced the retcons and the Memorial Park / district / crest system
above — see [`STORY_NOTES.md`](STORY_NOTES.md) for open questions raised by that same conversation, and
`Scripts/` for the scene-by-scene material it produced).*
