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
  large plaque with **five recessed pentagonal slots**. Inscription: *"WHAT WAS DIVIDED SHALL BE
  WHOLE. WHAT WAS HIDDEN SHALL BE OPENED. — THE FOUNDERS OF RAVENWOOD — 1887 —"* Each slot bears
  a faint engraved label: **ORDER, KNOWLEDGE, INDUSTRY, FAITH, MEDICINE.** The statue sits in a
  water basin; draining the basin (by filling all five slots) reveals a submerged door/staircase
  beneath it, descending into the Vanguard facility.
- **Each of the five founders built one civic institution and kept one emblem.** The five
  founders of Ravenwood are the same five founders of Vanguard BioSystems — the town and the
  company are one shared history, not two that later collided.
- The five emblems are cast-metal pentagon sections (fit together into a complete pentagon), each
  bearing a relief portrait of its founder, the founder's name, and a symbol of their institution.
  They were made together with the statue as the facility's original (crude, deliberate) access
  control system; over generations the original purpose was forgotten and the emblems became
  civic artifacts, kept out of tradition. A short founding-record document at the Academy covers
  this in-world.
- **Crest / district / slot reference table:**

| Direction | Crest Name | Location | Statue Slot Label | Institution Symbol |
|---|---|---|---|---|
| Southwest | Authority Crest | [Ravenwood Police Station](Locations/Police_Station.md) | ORDER | Key |
| Southeast | Knowledge Crest | [Worthy Academy](Locations/Academy.md) | KNOWLEDGE | Torch |
| Northeast | Medical Crest | [St. Dymphna Hospital](Locations/Hospital.md) | MEDICINE | Serpent/Caduceus |
| Northwest | Industry Crest | [Steelgate Refinery](Locations/Foundry_Refinery.md) | INDUSTRY | Anvil |
| North | Faith Crest | [Our Lady of Solace Monastery](Locations/Monastery.md) | FAITH | Cross (or similar) |

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

## Creature Classification: Ashen Mutant

**[The Maw](Creatures/The_Maw.md)** — a heavily mutated, territorial stalker/ambush predator
encountered in the Ravenwood Hotel, classified as an "Ashen Mutant" — is the first confirmed
example of this classification tier. It's responsible for both Cindy Sweets' Room 106 abduction
and Gerta's death. Whether "Ashen Mutant" applies more broadly (e.g. to the Caretaker) is not yet
confirmed.

## Survivor System (design rule, applies from Chapter 2 onward)

- **Tier 1 — Key story survivors:** a small number of fully developed characters, essential to the
  narrative, whose existence and role are fixed regardless of player action.
- **Tier 2 — Conditional survivors:** existence/condition/fate depends on player sequencing.
  Confirmed example: a surviving Police Station officer is alive (interactive, has information) if
  Jim visits the Police Station first; if Jim visits another district first, that officer has
  turned by the time Jim reaches the station. Rule: the player always gets the needed information
  either way (directly from the survivor, or via notes/environmental clues from the dead version);
  no survivor's death ever hard-blocks progression; the game never explicitly blames the player.

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
