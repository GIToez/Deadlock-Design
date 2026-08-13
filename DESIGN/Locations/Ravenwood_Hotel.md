# Ravenwood Hotel

> Content in this file is compiled from two sources:
> [`Deadlock Protocol - Story Design Rebuild.docx`](../Deadlock%20Protocol%20-%20Story%20Design%20Rebuild.docx)
> (original material) and [`AI.json`](../AI.json) (a later planning conversation that revisited
> and fixed several issues in the docx). Where they disagree, [`AI.json`](../AI.json)'s resolution is used — see
> [`CANON.md`](../CANON.md) ("Retcons") for the specific list. The full scene-by-scene script for this chapter
> lives in [`Scripts/Chapter_1_One_Night_Only.md`](../Scripts/Chapter_1_One_Night_Only.md); this file is the higher-level design summary.
>
> Note: earlier material referred to this content as a "Prologue" followed by a separate
> "Chapter 1." Per a later structural decision, **the Prologue has been folded into Chapter 1 —
> "One Night Only"** — there is no separate prologue; the hotel is Chapter 1 in its entirety.

## Purpose in the Overall Story

The Ravenwood Hotel is Chapter 1 of the game — **"One Night Only."** It establishes the
protagonist (Jim Mercer), his relationship with Sarah, and the hotel's cast of stranded guests
during a calm, grounded pre-outbreak night — then serves as the setting for the outbreak's opening
escalation, the "Deadlock Protocol" title-drop, the player's first combat and first firearm, and
the first boss encounter (The Caretaker). The chapter ends with the player's first exit from an
interior space into the streets of Ravenwood, leading directly into Chapter 2 (Memorial Park).

## Arrival / Setup

- Jim Mercer — retired military, now a telecommunications field engineer driving to a relay site
  that's been offline three days — drives into Ravenwood through a heavy storm along Highway 13,
  talking to Sarah by phone. Road signs pass: BLACKWATER, COUNTY LINE, RAVENWOOD — 2 MILES.
- The neon Ravenwood Hotel sign ("EST. 1956 — VACANCY") emerges through the rain. Jim parks his
  Jeep in the hotel lot.

  ![Hotel exterior — wide parking lot, Jim's Jeep, the police cruiser near the street](../Assets/Screenshots/ravenwood_hotel_exterior_parking_lot.webp)
  ![Hotel exterior — front entrance, circular fountain courtyard/walkway](../Assets/Screenshots/ravenwood_hotel_exterior_fountain_entrance.webp)

  > Reference screenshots uploaded by the project owner (2026-08-13) — in-engine mockups. The
  > second image adds a specific detail not previously scripted: a circular fountain courtyard
  > forming the pedestrian walkway between the parking lot and the front doors (with a carved
  > "RAVENWOOD HOTEL" sign at its base, separate from the neon marquee already established). This
  > reads as additive detail rather than a contradiction — a large hotel plausibly has both a
  > parking lot and a fountain drive/walkway — but flagging it here since it wasn't in the original
  > script.
- A police cruiser is seen pulled over near the entrance — **Officer Dale Pruitt** dealing with an
  unclearly-seen, subtly-twitching detained driver (Pruitt's unnamed exposure point) — an early,
  deniable hint of the outbreak.
- Optional parking-lot interactions: open the trunk (survey equipment, tools, and Jim's own
  belt-clipped flashlight — his standard field-engineer everyday-carry, part of his starting
  loadout rather than a pickup — see [`CANON.md`](../CANON.md) → "Player Starting Equipment"),
  examine the hotel sign, examine a storm drain (metallic rattling echoes below, then silence),
  approach the police stop (Pruitt waves Jim inside).
- A second phone call with Sarah occurs under the hotel awning before Jim enters.
- Jim enters through heavy (non-automatic) glass double doors into the lobby.

## Storyline

### Night One (Pre-Outbreak)

- **Lobby Introduction.** Jim meets night clerk **Earl Whitaker** at reception and is given
  **Room 104** ("end of the west hall"). The lobby is populated with other stranded guests:
  **Cindy Sweets** (west lounge couch, Room 106), **Maria & Richard Dalton** (east waiting area,
  Maria visibly pregnant, Room 118), and **Janeth Caldwell** (reading near a hallway lamp, Room
  112). A distant thud from upstairs is heard once, mid-conversation — Earl explains it as the old
  building settling/storm pressure and genuinely believes it; nothing about him should read as
  suspicious or foreknowing.
- **Free Exploration.** The player can freely revisit and talk to Cindy, the Daltons, Janeth, and
  Earl (all optional, deepening characterization before the outbreak), and explore the **Main
  Bar** (unattended), the **Recreation Room** (pool table, dart board, empty), and find **The Red
  Room** speakeasy lounge locked behind a "PRIVATE EVENT CLOSED" placard. The player can also
  proactively knock on **Room 106** any time before going to bed — Cindy answers in her robe for
  an optional, genuinely flirtatious scene that settles into an easier rapport once she learns
  he's married, before the mood shifts into her mentioning hearing "scratching" in the walls (an
  early, deniable hint of The Maw). A hallway glimpse of
  the hotel maid **Gerta** pushing a cleaning cart is a brief, ordinary, non-interactive beat.
- **Room 104.** Jim settles into his room (double bed, TV, rotary phone, small bathroom). Optional
  interactions include looking out the window (briefly seeing something move near the
  crashed-cruiser-to-be area), watching TV (a weather report is interrupted by a burst of police
  chatter warning officers to avoid direct contact — then reverts to normal), and texting Sarah,
  which fails to send ("No signal"). Jim goes to bed; rain and thunder continue; fade to black
  with **no warning sound beforehand** — the outbreak wakes him with nothing to brace for.

### The Outbreak

- **The Wake-Up.** A civil emergency siren and flashing red light jolt Jim awake with no warning.
  Screaming, breaking glass, and gunshots are audible outside and downstairs. A distorted
  loudspeaker announces an emergency quarantine.
- **Second Floor Hallway.** The hallway is in chaos; panicked guests flee. Jim finds **Janeth
  Caldwell** crouched, terrified, refusing to go downstairs. (Optionally, Cindy Sweets can be
  found at her door beforehand, uneasy about noises downstairs — this encounter happens *before*
  Jim goes to bed, not during the outbreak itself.)
- **Lobby Reveal.** Descending to the lobby, Jim finds it wrecked. **Earl Whitaker** is crouched
  over a guest's body, feeding — the game's **first confirmed infected reveal**. Earl rises and
  attacks.
- **First Survival.** Jim grabs a **baseball bat** from the wrecked lounge furniture and fights
  off Earl — the player's first combat encounter.
- **Janeth's Death / Police Cruiser Crash.** As Janeth runs for the front doors, a police cruiser
  crashes violently through the entrance, killing her and permanently blocking the front exit.
- **"Deadlock Protocol."** Over the wrecked cruiser's radio, "Deadlock Protocol is now in effect"
  is announced — the game's title card. This is the end of the "night before" section and the
  start of the chapter's second half.
- **Manager's Office.** Jim searches Earl's body for a **Manager's Key**, unlocks the staff
  hallway, and reaches the **Manager's Office** — the chapter's first safe room, containing a
  **VERN** terminal (see [`CANON.md`](../CANON.md) — VERN is a city-wide save network, not hotel-specific) that
  unlocks save functionality. Optional reads here include the guest ledger (confirming room
  numbers for Jim, Cindy, Janeth, and the Daltons) and an unsigned incident report noting a guest
  (Maria Dalton) was transported to **St. Dymphna Hospital** — the first in-fiction reference to a
  location beyond the hotel.
- **East Wing Power Restoration.** A breaker panel has three switches (Lobby / East Wing / West
  Wing). East Wing powers up cleanly; West Wing immediately trips a blown fuse — Jim will need a
  **screwdriver** to open the fuse housing and a replacement fuse before it can be fixed. A
  maintenance notice reveals the courtyard is the intended emergency evacuation route, but
  requires full auxiliary power.
- **Room 106 / Cindy's Abduction.** Before heading to the East Wing, Jim goes up the Grand
  Staircase and swings by Cindy's room on the second-floor **west** hallway to check on her. The
  door bursts open — Cindy Sweets, barefoot and bleeding, reaches for Jim before something drags
  her violently back inside; the door slams. See Scene 29 in
  [`Scripts/Chapter_1_One_Night_Only.md`](../Scripts/Chapter_1_One_Night_Only.md) for the full beat.
- **East Wing Retrieval Loop.** East Wing power unlocks the **East Public Stairwell** at the far
  end of the second-floor east hallway. Jim descends it into the East Wing's ground-floor service
  areas — the **Dining Hall**, the **Kitchen**, and its adjoining **Pantry/Storage** and **Walk-in
  Freezer** — finding a **screwdriver** in the **Utility Room**, then the **Laundry/Linen Room**
  (see "Gerta's Death," below), and finally the **East Wing Maintenance Closet**, where a
  handwritten note explains the replacement fuse was relocated to the West Wing. A barricaded
  service door behind the closet clears by hand, opening a **permanent shortcut straight back to
  the Lobby** — Jim never has to walk this loop again.
- **Gerta's Death.** In the Laundry/Linen Room, Jim finds Gerta's body — killed by **The Maw**, the
  same presence that dragged Cindy Sweets into Room 106 shortly before — see
  [`Creatures/The_Maw.md`](../Creatures/The_Maw.md) and
  [`Characters/Gerta.md`](../Characters/Gerta.md).
- **West Wing Maintenance Room.** Back through the Lobby shortcut and up to the second-floor west
  hallway again — quiet now, Room 106 undisturbed since Jim last stood there — to a small, unlocked
  room near the **West Public Stairwell** (not power-gated — it was simply shut, not locked). Jim
  recovers the **auxiliary fuse** here.
- **West Wing Power Restoration.** Back at the breaker panel, the screwdriver opens the fuse
  housing; Jim installs the fuse and activates the West Wing breaker, restoring power hotel-wide
  and bringing the **courtyard access system online**.
- **West Wing Ground Floor.** With West Wing power on, the **West Public Stairwell** (locked until
  now) opens, leading down to the **Lounge/Recreation** area. Jim moves through the West Wing's
  ground floor — **Piano Area**, **Lounge**, the **Main Bar** (with the **Red Room** opening
  directly off it), **Liquor Storage** — and its back-of-house (**Boiler Room**, **Staff
  Room/Storage**) — to the **West Wing Service Corridor** at the rear.
- **Courtyard Security Office.** Reached via the **West Wing Service Corridor**. Jim activates the
  courtyard access system remotely from here.
- **The Red Room (optional).** A self-contained speakeasy lounge opening directly off the **Main
  Bar**. Untouched by the outbreak's chaos — an eerily undisturbed room with a solitary singer,
  **Della Marsh** ("Della M." on stage — a four-year weekly Red Room performer), at the microphone.
  She's revealed, on approach, to be dead and infected; she attacks once Jim gets close (an
  optional mini-boss encounter). The Red Room has its own entrance and exit off the Bar — it
  doesn't lead anywhere else.
- **First Firearm.** Passing back through the lobby near the crashed cruiser, an infected police
  officer — **Officer Dale Pruitt**, the same officer seen at the start of the game — bursts from
  the vehicle and attacks. Defeating him yields the game's **first firearm** (a handgun) and
  ammunition, plus his field notepad and a printed dispatch advisory (see Key Items/Documents).
- **Hotel Courtyard / Fennimore's Body.** Jim exits the hotel into the courtyard for the first
  time — the player's first time outdoors since the outbreak began. The north gate's manual
  release is missing its crank handle. Near the gate, Jim finds the body of **Fennimore**, the
  hotel's night-shift security guard (previously only known from his locker in the West Wing Staff
  Room). A note on him explains he found **Roy Bullock** transforming, chained the maintenance shed
  shut himself, and tried to escape through the gate — only to discover he'd need the crank handle
  he'd personally locked away in the East Wing Housekeeping Closet. Jim takes the key off his body.
  See [`Characters/Fennimore.md`](../Characters/Fennimore.md).
- **East Wing Housekeeping Closet.** A mandatory return trip through the second-floor east
  hallway — the same stretch Jim walked once already, uneventfully, on the way to the East Public
  Stairwell (see "East Wing Retrieval Loop," above). Between Rooms 114 and 116, unlocking the
  closet triggers a **two-Shambler pincer ambush** from both flanking rooms — the chapter's first
  genuinely surrounded moment, and the payoff for a hallway the player had no reason to remember.
  Inside: the **Gate Crank Handle**.
- **Fennimore, Reanimated.** Returning to the courtyard, Jim finds Fennimore's body gone — he's
  turned, and attacks from behind the fountain. An ordinary Shambler fight, played straight, with
  no unique mechanics.
- **Gate Crank / Boss Fight.** Jim works the rusted manual crank — real effort, no quick fix — and
  the grinding noise draws **The Caretaker** (Roy Bullock, the hotel's longtime maintenance man,
  mutated by the outbreak) out of the shed **mid-crank, gate still only partway open**. The noise,
  not the gate opening, is what triggers the reveal. Boss fight across the courtyard; afterward,
  Jim finishes cranking the gate open.
- **Chapter End.** Jim exits the hotel grounds through the fully-opened gate onto a public
  street — directly across from Memorial Park — beginning Chapter 2.

## Important Rooms / Areas

**Ground floor — Lobby / center**

- **Lobby** — West Lounge (Cindy), East Waiting Area (the Daltons), Reception (Earl), the Grand
  Staircase up to the guest floor. Wrecked mid-chapter by the police cruiser crash.

  ![Lobby concept — west lounge, reception desk, east waiting area, grand staircase](../Assets/Reference/hotel_lobby_concept.png)

  > AI-generated concept art (2026-08-13), style-anchored to the Manager's Office/Dining Hall
  > reference screenshots — see [`Assets/README.md`](../Assets/README.md) → "Convention: room
  > concept art." Rough staging idea for the room's layout described in Scene 5, not a locked
  > floor plan.
- **Manager's Office** — the chapter's first safe room; VERN save terminal, guest ledger,
  incident report, breaker panel. Reached via the Staff Hallway off the Lobby (Manager's Key).

  ![Manager's Office — VERN terminal, Employee Records, safe, desk reference](../Assets/Screenshots/ravenwood_hotel_managers_office_vern.webp)
  ![Manager's Office — breaker/generator panel and duty reports board](../Assets/Screenshots/ravenwood_hotel_managers_office_breaker.webp)

  > Reference screenshots uploaded by the project owner (2026-08-13) — in-engine mockups, the most
  > reliable source of truth for art style and prop density in this room. Confirms the wall-mounted
  > VERN terminal exactly as described in [`CANON.md`](../CANON.md), plus an Employee Records
  > filing cabinet, a safe, and a desk nameplate reading "E. Whitaker" (not previously scripted —
  > plausibly Earl's own desk, given his 32-year tenure, though this isn't confirmed in the script
  > and shouldn't be treated as locked without follow-up). The second image shows a large panel
  > that's very likely the breaker panel described in the script, though it wasn't explicitly
  > labeled as such in the reference.
- **Breaker Panel** (inside Manager's Office) — Lobby / East Wing / West Wing power switches;
  central hub for the power-restoration puzzle.
- **Grand Staircase** — the main stairs between the Lobby and the guest floor above; used
  repeatedly during the power-restoration puzzle in both directions.

**Guest floor (accessible the whole chapter — not power-gated)**

- **Room 104** — Jim's guest room; the "night before" scene.

  ![Room 104 — bed, nightstand, rotary phone](../Assets/Screenshots/ravenwood_hotel_room104_bedroom_a.webp)
  ![Room 104 — TV, radiator, chair](../Assets/Screenshots/ravenwood_hotel_room104_bedroom_b.webp)
  ![Room 104 — bathroom](../Assets/Screenshots/ravenwood_hotel_room104_bathroom.webp)

  > Reference screenshots uploaded by the project owner (2026-08-13) — in-engine mockups matching
  > Scene 15 almost exactly (rotary phone, lamp, TV, bathroom mirror all present as scripted).
- **Room 106** — Cindy Sweets' room; site of her abduction jumpscare, triggered while crossing the
  west hallway toward the West Wing Maintenance Room.

  ![Room 106 concept — Cindy's guest room, suitcase, robe, personal effects](../Assets/Reference/hotel_room106_concept.png)

  > AI-generated concept art (2026-08-13), style-anchored to the Room 104 reference screenshots.
  > Same base guest-room layout as 104, personalized with Cindy's belongings — not a scripted
  > inventory of her room's contents.
- **Room 112** — Janeth Caldwell's room. **Room 118** — Maria & Richard Dalton's room.
- **Rooms 114 and 116** — otherwise-unremarkable guest rooms flanking the Housekeeping Closet;
  source of the second-floor east hallway's two-Shambler pincer ambush on the *second* pass through
  (see "Housekeeping Closet," below). Closed and uneventful on the first pass.
- **Housekeeping Closet** — between Rooms 114 and 116, on the guest floor's east hallway. Locked on
  the first pass (Scene 30); unlocked later with the key taken off Fennimore's body. Source of the
  **Gate Crank Handle** needed to open the courtyard's north gate.

  ![Housekeeping Closet concept — linen shelves, locked wire cage with the gate crank handle](../Assets/Reference/hotel_housekeeping_closet_concept.png)

  > AI-generated concept art (2026-08-13). Flagged inaccuracy: the render put a door number
  > ("305") on the closet door, which doesn't fit its canonical location — a supply closet on the
  > guest floor (2F) between Rooms 114/116, not a numbered guest room on a third floor. Ignore the
  > door number; everything else (linen shelves, the locked wire cage holding the crank handle,
  > the maintenance tag) matches the scripted contents.
- **West Wing Maintenance Room** — a small, simply-shut (not locked) room near the West Public
  Stairwell; source of the replacement **auxiliary fuse**.

  ![West Wing Maintenance Room concept — supply shelves, workbench, box of electrical parts with the replacement fuse](../Assets/Reference/hotel_west_maintenance_room_concept.png)

  > AI-generated concept art (2026-08-13), style-anchored to the Manager's Office breaker-panel
  > reference screenshot.
- **East Public Stairwell** — at the end of the guest floor's east hallway; unlocked by East Wing
  power; the only way down into the East Wing's ground-floor service areas on the first trip.
- **West Public Stairwell** — at the end of the guest floor's west hallway, beside the Maintenance
  Room; locked until West Wing power is restored, then opens onto the West Wing's ground floor.

**East Wing — ground floor, service areas (reached via the East Public Stairwell)**

- **Dining Hall**, **Kitchen**, **Pantry/Storage**, **Walk-in Freezer** — the hotel's dining and
  food-service wing; minor exploration content.

  ![Dining Hall — full room, round table set for service, buffet counter](../Assets/Screenshots/ravenwood_hotel_dining_hall.png)
  ![Dining Hall — buffet detail and the door through to the Kitchen](../Assets/Screenshots/ravenwood_hotel_dining_hall_kitchen_door.png)
  ![Kitchen — wall fixtures (stove, walk-in freezer, sinks)](../Assets/Screenshots/ravenwood_hotel_kitchen_fixtures.png)
  ![Kitchen — full room, with the door through to the Dining Hall](../Assets/Screenshots/ravenwood_hotel_kitchen_full.png)

  > Reference screenshots uploaded by the project owner (2026-08-13) — in-engine mockups. Confirm
  > the Dining Hall/Kitchen connection exactly as scripted (Scene 31) and visibly place a Medkit
  > icon on the Kitchen's wall, consistent with the game's established item iconography.
- **Utility Room** — source of the **screwdriver**.

  ![Utility Room concept — water heater, pumps, breaker panels, pegboard tools, workbench](../Assets/Reference/hotel_utility_room_concept.png)

  > AI-generated concept art (2026-08-13), style-anchored to the Manager's Office reference
  > screenshots.
- **Laundry/Linen Room** — industrial washers/dryers, laundry carts. Site of Gerta's death (killed
  by **The Maw**) — see [`Creatures/The_Maw.md`](../Creatures/The_Maw.md) and
  [`Characters/Gerta.md`](../Characters/Gerta.md).

  ![Laundry Room concept — washers/dryers, laundry carts, staff uniform rack](../Assets/Reference/hotel_laundry_room_concept.png)

  > AI-generated concept art (2026-08-13). Kept deliberately restrained on Gerta's body/wound
  > detail for this reference render — see [`Characters/Gerta.md`](../Characters/Gerta.md) for the
  > scripted description of the scene itself.
- **East Wing Maintenance Closet** — a handwritten note here reveals the auxiliary fuse was
  relocated to the West Wing. A barricaded service door behind it clears by hand, opening a
  **permanent shortcut straight back to the Lobby**.

**West Wing — ground floor (reached via the West Public Stairwell, once unlocked)**

- **Lounge/Recreation** — pool table, dart board; minor pre-outbreak atmosphere beat.
- **Piano Area** — a small nook off the Lounge.
- **Main Bar** — unattended pre-outbreak; wrecked later.

  ![Main Bar concept — bar counter, neon signs, overturned stools, wrecked lounge seating](../Assets/Reference/hotel_main_bar_concept.png)

  > AI-generated concept art (2026-08-13), style-anchored to the Dining Hall reference screenshot.
- **The Red Room** — self-contained optional speakeasy lounge opening directly off the Main Bar;
  site of the Della Marsh encounter. Does not connect to the Security Office.

  ![Red Room concept — velvet curtains, cocktail tables, spotlighted stage, upright piano](../Assets/Reference/hotel_red_room_concept.png)

  > AI-generated concept art (2026-08-13, re-rendered same day to fix a flat top-down camera
  > mismatch — see [`STORY_NOTES.md`](../STORY_NOTES.md) "Room concept art style-consistency pass").
  > Della Marsh herself intentionally left out of this render — see
  > [`Characters/Della_Marsh.md`](../Characters/Della_Marsh.md) if/when it exists, or
  > [`Scripts/Chapter_1_One_Night_Only.md`](../Scripts/Chapter_1_One_Night_Only.md) Scene 38 for her
  > scripted description.
- **Liquor Storage** — off the Bar; minor exploration content.
- **Boiler Room**, **Staff Room/Storage** — West Wing back-of-house.
- **West Wing Service Corridor** — a staff-only route at the rear of the West Wing leading to the
  Courtyard Security Office.
- **Courtyard Security Office** — controls courtyard gate access; reached via the West Wing
  Service Corridor.

  ![Courtyard Security Office concept — CCTV monitor bank, security terminal, emergency lockdown panel, courtyard access control](../Assets/Reference/hotel_security_office_concept.png)

  > AI-generated concept art (2026-08-13), style-anchored to the Manager's Office breaker-panel
  > reference screenshot.

**Exterior**

- **Hotel Courtyard** — fountain, chained-shut maintenance shed, and the north exit gate to the
  street/Memorial Park. The gate is a heavy steel-framed double gate retrofitted at some point as
  the hotel's designated fire-code emergency exit — electrically motorized, with a required manual
  crank override for exactly this kind of power-failure scenario. Site of Fennimore's body (and
  later his reanimation) and the Caretaker (Roy Bullock) boss fight.

  ![Hotel Courtyard concept — rain, fountain, perimeter fence, north gate with manual release, maintenance shed](../Assets/Reference/hotel_courtyard_concept.png)

  > AI-generated concept art (2026-08-13, re-rendered same day as a straight top-down aerial to
  > match the exterior parking-lot/fountain-entrance reference screenshots exactly — see
  > [`STORY_NOTES.md`](../STORY_NOTES.md) "Room concept art style-consistency pass"). Fennimore's
  > body and the shed's warped doors are not visible at this framing — see Scene 42 for the
  > scripted beat-by-beat reveal.

## Blueprint (Room Connectivity)

> Not a to-scale architectural floor plan — a **relational** diagram of how rooms connect, and
> what's in each one, derived directly from `Storyline` and `Scripts/Chapter_1_One_Night_Only.md`
> above. Split into one diagram per floor/area (a single combined diagram rendered too cramped to
> read clearly) — read them top to bottom; each one notes where it picks up from the previous.
> Solid arrows are direct, always-available connections; dashed arrows are connections gated
> behind a story condition (a key, restored power, a blood trail appearing post-outbreak, etc.) —
> the label on the arrow says what unlocks it.
>
> Legend: 👤 NPC · ☠️ enemy/infected/boss · 🗝️ key item · 📄 document · 💾 save point (VERN) ·
> ⚡ power/breaker · 🚪 gate/access control · 🔧 manual/mechanical (non-power) puzzle · ⛲ fountain.
>
> **Shape/color key** — every hallway/corridor/stairwell is its own node (nothing is folded into
> a single "West Wing" black box); the shape and color just tell you *what kind* of node you're
> looking at at a glance:
>
> - 🟣 **rectangle, purple** — a room with actual content (NPCs, items, enemies, events).
> - 🟡 **pill/stadium, amber** — a hallway, corridor, stairwell, or crossover — a pure connector
>   you pass through, not a destination.
> - 🟢 **rectangle, green** — a safe room (save point).
> - 🔴 **rectangle, red** — a boss or mini-boss encounter room.
> - 🔵 **pill, blue** — exterior space (street, gate, parking lot approach).
> - ⚪ **dashed grey pill** — a pointer back to a node that's defined in full on another diagram
>   (e.g. "(see Diagram 1)") — not a new physical space, just a stitch point between diagrams.

> **Floor note:** the hotel is two floors only — a ground floor and a guest floor above it — no
> second guest-inaccessible floor, no service crossover between wings. The guest floor is freely
> walkable the entire chapter; the *stairwells* down to the ground floor are what's power-gated
> (see Diagram 2).

### 1. Exterior → Lobby (ground floor, center)

```mermaid
flowchart TD
    HWY(["Highway 13<br/>fixed shot — no player control"])
    LOT["Parking Lot<br/>👤 Officer Pruitt + stopped driver"]
    ENTRY(["Hotel Entry"])
    LOBBY["🏨 LOBBY<br/>👤 Cindy · Maria · Richard · Janeth · Earl<br/>☠️ Earl & Officer Pruitt turn infected<br/>🗝️ Baseball Bat · Manager's Key · Handgun<br/>💥 cruiser crash blocks front exit"]
    STAFFH(["Staff Hallway<br/>needs Manager's Key"])
    MGROFF["🛡️ MANAGER'S OFFICE — safe room<br/>💾 VERN Terminal · ⚡ Breaker Panel<br/>📄 Guest Ledger · Incident Report"]
    GRANDSTAIR(["Grand Staircase<br/>↕ to Diagram 2 (Guest Floor)"])
    ECLOSETREF(["East Wing Maintenance Closet<br/>(see Diagram 3 — shortcut once cleared)"])

    HWY --> LOT --> ENTRY --> LOBBY
    LOBBY --> STAFFH --> MGROFF
    LOBBY --> GRANDSTAIR
    LOBBY <-. barricade cleared by hand .-> ECLOSETREF

    classDef room fill:#EDEBFF,stroke:#7C6EE0,color:#1a1a2e
    classDef hallway fill:#FFF3D6,stroke:#D9A404,color:#3a2e00
    classDef safe fill:#DFF5E1,stroke:#2E9E4F,color:#0d2b12,stroke-width:2px
    classDef exterior fill:#E3F0FF,stroke:#4A76C9,color:#0d1f3a
    classDef ref fill:#F5F5F5,stroke:#999999,color:#444444,stroke-dasharray:3 3
    class HWY,LOT exterior
    class ENTRY,STAFFH,GRANDSTAIR hallway
    class LOBBY room
    class MGROFF safe
    class ECLOSETREF ref
```

### 2. Guest Floor (not power-gated — freely walkable all chapter)

```mermaid
flowchart TD
    GRANDSTAIRREF(["Grand Staircase<br/>(up from Diagram 1)"])
    EHALL(["East Hallway"])
    R112["Room 112 — Janeth"]
    R118["Room 118 — Maria & Richard"]
    R114_116["Rooms 114 & 116<br/>☠️ ×2 — pincer ambush<br/>(2nd pass only, see Diagram 5)"]
    HOUSEKEEP["Housekeeping Closet<br/>🗝️ Gate Crank Handle<br/>🔒 needs key from Fennimore's body (Diagram 5)"]
    EPUBSTAIR(["East Public Stairwell<br/>🚪 East Wing power<br/>↓ to Diagram 3"])
    WHALL(["West Hallway"])
    R104["Room 104<br/>Jim's room"]
    R106["Room 106<br/>☠️ The Maw — Cindy's abduction"]
    WMAINTROOM["West Wing Maintenance Room<br/>🗝️ Auxiliary Fuse<br/>(unlocked — just shut, not power-gated)"]
    WPUBSTAIR(["West Public Stairwell<br/>🚪 West Wing power<br/>↓ to Diagram 4"])

    GRANDSTAIRREF --> EHALL
    GRANDSTAIRREF --> WHALL
    EHALL --> R112
    EHALL --> R118
    EHALL --> R114_116
    R114_116 --> HOUSEKEEP
    EHALL -. East Wing power .-> EPUBSTAIR
    WHALL --> R104
    WHALL --> R106
    WHALL --> WMAINTROOM
    WHALL -. West Wing power .-> WPUBSTAIR

    classDef room fill:#EDEBFF,stroke:#7C6EE0,color:#1a1a2e
    classDef hallway fill:#FFF3D6,stroke:#D9A404,color:#3a2e00
    classDef ref fill:#F5F5F5,stroke:#999999,color:#444444,stroke-dasharray:3 3
    class GRANDSTAIRREF ref
    class EHALL,WHALL,EPUBSTAIR,WPUBSTAIR hallway
    class R104,R106,R112,R118,WMAINTROOM,R114_116,HOUSEKEEP room
```

### 3. East Wing — ground floor (reached via the East Public Stairwell)

```mermaid
flowchart TD
    EPUBSTAIRREF(["East Public Stairwell<br/>(down from Diagram 2)"])
    DINING["Dining Hall"]
    KITCHEN["Kitchen"]
    PANTRY["Pantry/Storage"]
    FREEZER["Walk-in Freezer"]
    UTILITY["Utility Room<br/>🗝️ Screwdriver"]
    LAUNDRY["🧺 Laundry/Linen Room<br/>☠️ Gerta's body — killed by The Maw"]
    ECLOSET["East Wing Maintenance Closet<br/>📄 Note: fuse relocated to West Wing"]
    LOBBYREF(["🏨 Lobby<br/>(see Diagram 1 — shortcut once cleared)"])

    EPUBSTAIRREF --> DINING --> KITCHEN
    KITCHEN --> PANTRY
    KITCHEN --> FREEZER
    KITCHEN --> UTILITY --> LAUNDRY --> ECLOSET
    ECLOSET <-. barricade cleared by hand .-> LOBBYREF

    classDef room fill:#EDEBFF,stroke:#7C6EE0,color:#1a1a2e
    classDef hallway fill:#FFF3D6,stroke:#D9A404,color:#3a2e00
    classDef ref fill:#F5F5F5,stroke:#999999,color:#444444,stroke-dasharray:3 3
    class EPUBSTAIRREF,LOBBYREF ref
    class DINING,KITCHEN,PANTRY,FREEZER,UTILITY,LAUNDRY,ECLOSET room
```

### 4. West Wing — ground floor (reached via the West Public Stairwell, once unlocked)

```mermaid
flowchart TD
    WPUBSTAIRREF(["West Public Stairwell<br/>(down from Diagram 2)"])
    LOUNGE["Lounge/Recreation"]
    PIANO["Piano Area"]
    BAR["Main Bar<br/>wrecked later"]
    REDROOM["🎤 Red Room — optional, off the Bar<br/>☠️ Della Marsh — mini-boss<br/>📄 Booking slip · Personal note"]
    LIQUOR["Liquor Storage"]
    BOILER["Boiler Room"]
    STAFFRM["Staff Room/Storage"]
    WCORR(["West Wing Service Corridor"])
    SECOFF["Courtyard Security Office<br/>🚪 activates courtyard gate<br/>↓ to Diagram 5 (Courtyard)"]

    WPUBSTAIRREF --> LOUNGE
    LOUNGE --> PIANO
    LOUNGE --> BAR
    BAR --> REDROOM
    BAR --> LIQUOR
    LOUNGE --> BOILER --> STAFFRM --> WCORR --> SECOFF

    classDef room fill:#EDEBFF,stroke:#7C6EE0,color:#1a1a2e
    classDef hallway fill:#FFF3D6,stroke:#D9A404,color:#3a2e00
    classDef boss fill:#FFE0E0,stroke:#C0392B,color:#3a0d0d,stroke-width:2px
    classDef ref fill:#F5F5F5,stroke:#999999,color:#444444,stroke-dasharray:3 3
    class WPUBSTAIRREF ref
    class WCORR hallway
    class LOUNGE,PIANO,BAR,LIQUOR,BOILER,STAFFRM,SECOFF room
    class REDROOM boss
```

### 5. Courtyard

```mermaid
flowchart TD
    SECOFFREF(["Courtyard Security Office<br/>(from Diagram 4)"])
    COURT["Hotel Courtyard<br/>⛲ Fountain"]
    GATEBOX["North Gate — Manual Release<br/>🔧 needs Gate Crank Handle<br/>📄 placard: handle stored per protocol"]
    FENNIMORE["Fennimore's Body<br/>🗝️ Housekeeping Closet Key<br/>📄 his note<br/>↑ to Diagram 2 (Housekeeping Closet)"]
    FENNREANIM["Fennimore, Reanimated<br/>☠️ Shambler<br/>(on return from Diagram 2)"]
    SHED["Maintenance Shed<br/>☠️ THE CARETAKER / Roy Bullock — BOSS<br/>📄 Maintenance log<br/>🚪 bursts open mid-crank, drawn by noise"]
    GATE(["North Gate, fully open<br/>→ Ravenwood streets / Memorial Park, Chapter 2"])

    SECOFFREF --> COURT
    COURT --> GATEBOX
    COURT --> FENNIMORE
    FENNIMORE -. backtrack for crank handle .-> FENNREANIM
    FENNREANIM --> SHED --> GATE

    classDef room fill:#EDEBFF,stroke:#7C6EE0,color:#1a1a2e
    classDef boss fill:#FFE0E0,stroke:#C0392B,color:#3a0d0d,stroke-width:2px
    classDef exterior fill:#E3F0FF,stroke:#4A76C9,color:#0d1f3a
    classDef ref fill:#F5F5F5,stroke:#999999,color:#444444,stroke-dasharray:3 3
    class SECOFFREF ref
    class COURT,GATEBOX,FENNIMORE room
    class SHED,FENNREANIM boss
    class GATE exterior
```

## Characters Encountered

- **[Jim Mercer](../Characters/Jim_Mercer.md)** — protagonist/player character. Retired military
  (comms/logistics), now a telecommunications field engineer.
- **[Sarah Mercer](../Characters/Sarah_Mercer.md)** — Jim's partner; phone contact only, ending
  after the parking-lot call (see [`CANON.md`](../CANON.md) — no contact resumes until the
  Epilogue).
- **[Earl Whitaker](../Characters/Earl_Whitaker.md)** — hotel night clerk; checks Jim in; becomes
  the chapter's first infected. An ordinary, unsuspecting man with no foreknowledge of the
  outbreak — his death should land harder for it.
- **[Cindy Sweets](../Characters/Cindy_Sweets.md)** — guest, Room 106; present pre-outbreak, later
  heard/glimpsed during the outbreak, dragged away in a jumpscare mid-chapter. Fate beyond that
  scene is not yet established.
- **[Maria Dalton](../Characters/Maria_Dalton.md)** and **[Richard Dalton](../Characters/Richard_Dalton.md)** —
  guests, Room 118, expecting a child; leave for St. Dymphna Hospital shortly before the outbreak
  begins (per the incident report). Their fate is intended to be resolved later, at the hospital,
  once that chapter is written.
- **[Janeth Caldwell](../Characters/Janeth_Caldwell.md)** — guest, Room 112; present pre-outbreak
  and during the initial panic; killed on-screen by the crashing police cruiser.
- **[Gerta](../Characters/Gerta.md)** — hotel maid; a single brief, ordinary hallway encounter
  pre-outbreak. Later found dead in the Laundry Room, killed by The Maw — see below.
- **[Officer Dale Pruitt](../Characters/Dale_Pruitt.md)** — Ravenwood PD; seen at the parking lot
  at the start of the chapter, and again (infected) inside the crashed cruiser later.
- **[Fennimore](../Characters/Fennimore.md)** — hotel night-shift security guard; never seen alive.
  Established through his West Wing Staff Room locker, then his body and note in the courtyard,
  then his reanimated Shambler fight. His choice to chain the maintenance shed shut is why it's
  sealed (and straining) by the time Jim reaches it.

## Creatures Encountered

- **Earl Whitaker (infected)** — the chapter's first infected; a named character rather than a
  generic creature type — see [`Characters/Earl_Whitaker.md`](../Characters/Earl_Whitaker.md).
- **Officer Dale Pruitt (infected)** — named character, not a generic creature type — see
  [`Characters/Dale_Pruitt.md`](../Characters/Dale_Pruitt.md).
- **[Della Marsh](../Creatures/Della_Marsh.md)** ("the Red Room Singer," infected) — optional
  mini-boss in the Red Room.
- **[The Caretaker](../Creatures/The_Caretaker.md) / Roy Bullock** (infected) — the chapter's
  boss, fought in the courtyard. See full AI/phase design below.
- **[The Maw](../Creatures/The_Maw.md)** — classification: Ashen Mutant; a heavily mutated,
  territorial stalker/ambush predator whose torso splits open into an enormous feeding mouth.
  Glimpsed only in fragments; responsible for dragging Cindy Sweets into Room 106 and for killing
  Gerta in the Laundry Room. Not directly fought in Chapter 1 by design.
- **[Shambler](../Creatures/Shambler.md)** — the game's standard base-tier infected, populating the
  hotel throughout the East and West Wing power-restoration loops (not just referenced by name, as
  originally written — see [`STORY_NOTES.md`](../STORY_NOTES.md) for that retcon). Deliberately not
  in every room, to keep the placement unpredictable rather than a checklist. Confirmed placements,
  one Shambler each unless noted:
  - Second-floor east hallway (Scene 30, before the East Public Stairwell) — this pass is
    otherwise deliberately uneventful; Rooms 114/116 and the Housekeeping Closet are noted but
    unremarkable here, on purpose (see the pincer ambush below).
  - Dining Hall (Scene 31).
  - Utility Room (Scene 32) — ambushes the player right as the screwdriver is picked up.
  - Lounge/Recreation (Scene 37, first room reached off the West Public Stairwell).
  - Main Bar (Scene 37).
  - Boiler Room (Scene 37).
  - West Wing Service Corridor (Scene 39).
  - **East Wing Housekeeping Closet (Scene 43) — two Shamblers, a pincer ambush**, from Rooms 114
    and 116. Not a first-visit surprise — the player already walked this exact stretch of hallway
    once, uneventfully, in Scene 30. This is the payoff for that forgettable first pass: the
    player's instinctive retreat from the first door puts them directly in front of the second one.
    First genuinely surrounded, no-clean-retreat moment of the chapter.
  - **Fennimore, reanimated (Scene 44)** — a named/story-relevant Shambler rather than a generic
    one; see [`Characters/Fennimore.md`](../Characters/Fennimore.md). Mechanically an ordinary
    fight, no unique mechanics.
  - Not placed in: Manager's Office, Kitchen, Pantry, Walk-in Freezer, Laundry/Linen Room, East
    Wing Maintenance Closet, either guest-floor hallway near Room 106, the West Wing Maintenance
    Room, Piano Area, Liquor Storage, Staff Room, or the Red Room — kept clear so the emotionally
    heavier beats (Gerta, Cindy, the fuse pickups) and quieter breather rooms aren't crowded out by
    combat.

## Puzzles

- **Power Restoration (East Wing → West Wing).** Flip East Wing power at the breaker panel → head
  up to check on Cindy Sweets in Room 106 first (see "Room 106 / Cindy's Abduction," above) →
  descend the newly-unlocked East Public Stairwell → work through the East Wing's ground-floor
  service areas (Dining Hall → Kitchen → Pantry/Freezer → Utility Room, where the **screwdriver**
  is found → Laundry/Linen Room → East Wing Maintenance Closet, where a note reveals the fuse was
  relocated to the West Wing) → clear the barricaded shortcut door back to the Lobby by hand →
  head back up to the guest floor and across to the **West Wing Maintenance Room** (near the West
  Public Stairwell, simply shut, not power-gated) to recover the **auxiliary fuse** → return to
  the breaker panel, use the screwdriver to open the fuse housing, install the fuse, and activate
  West Wing power. This also unlocks the **West Public Stairwell**, opening the route down into
  the West Wing's ground floor and, eventually, the Courtyard Security Office.
- **Courtyard Gate Release.** Deliberately *not* another power-restoration puzzle — by this point
  the hotel's power is already fully back on, so a second "fix the electricity" beat would be
  redundant. Instead: the north gate's manual release is missing its crank handle → Jim finds
  **Fennimore's** body near the gate, with a note explaining he stored the handle himself in the
  East Wing Housekeeping Closet (hotel security protocol) and the key to it on his belt → a
  mandatory return trip through the second-floor east hallway (Rooms 114/116) to retrieve it,
  triggering a **two-Shambler pincer ambush** → back to the courtyard, where **Fennimore has
  reanimated** and has to be put down again → Jim fits the crank handle and works the rusted
  mechanism by hand. The grinding noise — not the gate finishing opening — is what draws
  **The Caretaker** out of the shed mid-crank, gate still only partway open, beginning the boss
  fight. Jim finishes opening the gate after defeating him.

## Key Items

- **Manager's Key** — taken from Earl Whitaker's body; opens the staff hallway to the Manager's
  Office.
- **Baseball Bat** — Jim's first weapon, grabbed from wrecked lobby furniture during the Earl
  Whitaker attack.
- **Screwdriver** — found in the East Wing's Utility Room; its only use is opening the fuse
  housing at the breaker panel (both to confirm the blown West Wing fuse and to install the
  replacement).
- **Auxiliary Fuse** — recovered from the West Wing Maintenance Room (guest floor, near the West
  Public Stairwell); installed at the breaker panel to restore West Wing power.
- **Handgun** — the game's first firearm, taken from Officer Pruitt inside the crashed cruiser
  (Scene 41). Any Handgun Ammunition collected earlier automatically loads into it — see below.
- **Housekeeping Closet Key** — taken from Fennimore's body in the courtyard (Scene 42); opens the
  Housekeeping Closet on the guest floor's east hallway, between Rooms 114 and 116 (Scene 43).
- **Gate Crank Handle** — found in the Housekeeping Closet (Scene 43); the manual override needed
  to work the courtyard's north gate release by hand (Scenes 45–46).

### Consumables (optional, non-mandatory)

- **Medkit** — the game's standardized healing item name (see
  [`STORY_NOTES.md`](../STORY_NOTES.md) for the naming decision). Found in: a guest-room suitcase
  on the second-floor east hallway (Scene 30), the East Wing Pantry (Scene 31), the West Wing
  Liquor Storage (Scene 37), and the West Wing Staff Room locker (Scene 37) — four total.
- **Handgun Ammunition** — found before the handgun itself, which is a deliberate genre-standard
  pattern (stockpile ready for when the gun arrives). Found in: the East Wing Utility Room supply
  drawer (Scene 32), the West Wing Staff Room locker (Scene 37), and the Courtyard Security Office
  desk drawer (Scene 40) — three total, plus what's taken directly from Officer Pruitt's body.

### Documents (full text written — see [`Scripts/Chapter_1_One_Night_Only.md`](../Scripts/Chapter_1_One_Night_Only.md) for verbatim content)

- Emergency lockdown notice (breaker panel) — courtyard is the evacuation route, requires full
  auxiliary power.
- Guest ledger (Manager's Office) — room assignments for Jim, Cindy, Janeth, Maria & Richard.
- Incident report (Manager's Office) — Maria Dalton transported to St. Dymphna Hospital, 11:42 PM.
- Maintenance note (East Wing Maintenance Closet, signed "R.B.") — points to the West Wing fuse
  relocation.
- Maintenance log (West Wing Maintenance Room, signed "R.B.") — explains why the spare fuse stock
  ended up on the guest floor after a basement flood. Along with the East Wing note, this is a
  subtle, unconfirmed early hint at Roy Bullock's identity (only his initials, not his full name)
  — see the courtyard shed log below for where his full name is actually confirmed.
- VERN terminal label (Manager's Office) — "RAVENWOOD MUNICIPAL EMERGENCY NETWORK / VANGUARD
  EMERGENCY RESPONSE NODE — TERMINAL 07."
- **Della Marsh's booking slip and personal note** (Red Room backstage, Scene 38) — establishes
  her as a real person (four-year residency; a note to her mother, written as she began feeling
  unwell).
- **Roy Bullock's maintenance log** (courtyard shed, post-Caretaker fight, Scene 45) — years of
  routine entries ending with him noticing sirens and "something in the air" the night of the
  outbreak; the only place his name ("Roy") is confirmed on-screen. No longer references a
  generator (retired along with that puzzle) — the Wednesday entry now covers routine maintenance
  on the gate's manual release gearbox instead.
- **Fennimore's note** (found on his body, courtyard, Scene 42) — explains he found Roy Bullock
  transforming, chained the maintenance shed shut himself, and was trying to escape through the
  gate when he discovered the crank handle was exactly where he'd stored it — the East Wing
  Housekeeping Closet, between Rooms 114 and 116. Unsigned; his full first name is never confirmed
  anywhere.
- **Officer Pruitt's field notepad and a printed dispatch advisory** (found on his body, Scene 41)
  — his own account of the traffic stop that exposed him, and Ravenwood PD's Class 4
  public-health-emergency advisory referencing "Deadlock Protocol" standing by pending
  authorization. The notepad's cover ("OFFICER D. PRUITT — RAVENWOOD PD") is the only place his
  full name is confirmed on-screen.

## Major Scripted Events

- Lobby reveal: Earl Whitaker feeding on a guest (first infected reveal).
- Police cruiser crashes through the front entrance, killing Janeth Caldwell and blocking the
  main exit.
- "Deadlock Protocol is now in effect" radio announcement / title card.
- Cindy Sweets' Room 106 jumpscare and abduction (by The Maw).
- Gerta's death, discovered in the Laundry Room (by The Maw) — see [`Characters/Gerta.md`](../Characters/Gerta.md).
- Della Marsh (Red Room singer) reveal — appears to be a survivor, then turns.
- Officer Pruitt jumpscare from inside the crashed cruiser.
- Fennimore's body found near the courtyard gate, with his note revealing he chained the shed shut.
- **East Wing Housekeeping Closet pincer ambush** (Scene 43) — two Shamblers from Rooms 114 and
  116, the chapter's first no-clean-retreat combat moment, paying off a deliberately forgettable
  first pass through the same hallway in Scene 30.
- Fennimore's reanimation, discovered on returning to the courtyard (Scene 44).
- Maintenance shed breach revealing The Caretaker (Roy Bullock) — triggered by the noise of Jim
  working the gate's manual crank, mid-effort, gate still only partway open.

## False Alarms / Tension Beats (no threat, no combat)

A handful of noise/object scares placed in otherwise-quiet optional rooms, so tension stays up even
where there's nothing to fight — the player shouldn't be able to tell "empty room" from "real
threat" purely from the buildup:

- **Walk-in Freezer** (Scene 31) — a stack of boxes, undermined by melt, collapses loudly as Jim
  enters. Nothing follows the noise.
- **East Wing Maintenance Closet** (Scene 34) — a metallic clang through the ceiling vents while
  Jim reads the fuse-relocation note. Whatever it is, it doesn't come down here.
- **Piano Area** (Scene 37) — a loosened framed photo falls off a shelf behind Jim as he stands up
  from the piano bench.

## Boss Encounters

### The Caretaker / Roy Bullock (Hotel Courtyard)

A mutated former hotel maintenance man — the player's first major mutation encounter, designed as
a physical intimidation boss demonstrating that infection can progress into monstrous forms.
Unlike baseline infected ("shamblers"), the Caretaker actively pursues and corners the player.
Triggered by the noise of Jim working the gate's manual crank by hand, not by any power being
restored — he breaches the shed **mid-crank**, meaning the fight plays out with the north gate
still only partway open in the background (a visible, unresolved reminder of the way out, not yet
usable).

- **Phase 1 — Stalk:** deliberate, heavy, unstoppable-feeling advance; wide pathing; destroys
  obstacles; occasional intimidation pauses.
- **Phase 2 — Aggression:** close-range attacks (overhead slam, wide horizontal arm swing,
  shoulder charge, corner grab attempts); high damage, heavy knockback, long recovery windows the
  player is meant to exploit.
- **Phase 3 — Enraged (low health):** faster, more reckless, repeated slam combos, reduced
  stagger; courtyard floodlights flicker violently, destabilizing visibility.
- **Weaknesses:** headshots, environmental spacing, and attack-recovery windows. The
  recently-acquired handgun is highly valuable here; melee remains possible but risky.
- **Arena hazards:** flooded pavement, hedge choke points, the partially-open gate mechanism,
  fountain obstacles, low visibility during rain bursts.

## Crest Progression

Not applicable to this location directly. The five-crest structure (see [`CANON.md`](../CANON.md)) applies to
five outer districts of Ravenwood reached via Memorial Park, not to the Hotel itself.

## Exit / Progression to Next Area

Defeating the Caretaker clears the way for Jim to finish working the gate's manual crank — left
only partway open when the boss interrupted him mid-effort. Jim exits the hotel grounds through
the fully-opened gate onto a public street, directly across from **Memorial Park** — the chapter's
end and the start of Chapter 2. See [`Locations/Memorial_Park.md`](Memorial_Park.md).
