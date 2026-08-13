# Memorial Park

> Content in this file is drawn from [`AI.json`](../AI.json) (planning conversation), which is the only source
> covering this location. Full scene-by-scene script: [`Scripts/Chapter_2_Ravenwood.md`](../Scripts/Chapter_2_Ravenwood.md) (covers the
> street crossing, the park, the guardhouse, and the Founders Memorial in full; the interior of
> Memorial Park itself is fully scripted — the five districts reached from it are not yet).

## Purpose in the Overall Story

Memorial Park is Chapter 2's central hub — the game's **permanent safe base** for the remainder
of the story. It's where the player first learns (indirectly, through environmental discovery)
about the five-crest mechanism that structures the rest of Chapter 2, and it's the location the
player returns to constantly between districts to save, restock, and fast-travel.

## Arrival / Setup

- Jim exits the Ravenwood Hotel's north courtyard gate onto a public street. For the first time
  since the outbreak began, he's outside the hotel. The street is blocked in both directions by
  raised retractable emergency **bollards** (a locked "RAVENWOOD EMERGENCY MANAGEMENT — BOLLARD
  SYSTEM — ACTIVE — AUTHORIZATION REQUIRED" panel denies him), forcing a short **linear** street
  crossing straight ahead to the park. A lone standard infected ("shambler") is encountered along
  the way — avoidable or engageable, player's choice.
- **A blood trail**, starting right at the courtyard gate, runs roughly parallel to Jim's path
  toward the park before thinning out and going wide of the south gate itself, ending at
  **[Cindy Sweets](../Characters/Cindy_Sweets.md)'s** torn, empty, hotel-issue robe in the hedges
  along the outer fence. No body, no further trail — this continues her unresolved Chapter 1
  thread without answering it. See
  [`Scripts/Chapter_2_Ravenwood.md`](../Scripts/Chapter_2_Ravenwood.md), Scene 3.
- The park's south gate stands open beneath a stone archway reading "MEMORIAL PARK — EST. 1891."
  Jim enters.

## Storyline

- **Clearing the Park.** The park interior is quiet in a *wrong* way — empty of people, but not
  of infected. Four infected are present on arrival (one on the western fence path, one near a
  central-path bench, one near a large oak tree by the guardhouse, one inside the guardhouse
  itself, requiring the door to be opened to engage). No reinforcements arrive — the perimeter
  fence is intact and the other three gates are locked from the outside. Once all four are dealt
  with, the park is secure.
- **Securing the South Gate.** Jim finds a sliding bolt mechanism on the inside of the south gate
  and locks it — securable/reopenable by Jim at any time, but nothing gets in from outside without
  force from here on.
- **The Guardhouse.** A small room near the south gate: desk, filing cabinet, a wall-mounted VERN
  terminal (Terminal 02), and a bolted-down inventory chest. Activating VERN unlocks save
  functionality and the chest simultaneously. A corkboard holds a park maintenance schedule
  (routine, no story content), a laminated park map (added to inventory — shows the four gates and
  the central monument), and a two-page handwritten note from the park's groundskeeper (see
  Puzzles / how Jim learns about the crests, below). A **bollard override keycard** ("STREET
  INFRASTRUCTURE OVERRIDE — SECTOR 4 — MEMORIAL PARK PERIMETER") sits on the desk.
- **The Founders Memorial.** Jim approaches the central monument: a ~10-foot bronze female civic
  statue in a water basin, holding a large circular medallion-plaque — a small five-sided pentagon
  hub at the center (bearing a single weathered letter "V"), surrounded by five trapezoidal
  wedge-shaped recesses arranged like a compass rose, each with a faint engraved label (ORDER,
  KNOWLEDGE, INDUSTRY, FAITH, MEDICINE — see [`CANON.md`](../CANON.md) for the full
  crest/location/wedge-position mapping; concept art at
  [`Assets/Reference/founders_memorial_plaque_concept.png`](../Assets/Reference/founders_memorial_plaque_concept.png)).
  Each recess is an empty socket meant to hold a separate, physical emblem piece — when filled, the
  emblem sits *in* the recess as a distinct object with a visible seam at its edge, not a marking
  on the existing stone. An inscription runs the plaque's outer rim: *"WHAT WAS DIVIDED SHALL BE
  WHOLE. WHAT WAS HIDDEN SHALL BE OPENED. — THE FOUNDERS OF RAVENWOOD — 1887 —"* All five recesses
  are empty on arrival. Examining the water basin, Jim notices a faint seam in the submerged stone
  base — the suggestion of a door — and concludes the basin needs to be drained (i.e., all five
  recesses filled) before whatever's underneath can be reached.
- **Opening the City.** Returning to the street with the keycard, Jim lowers the bollards. The
  street opens in both directions and Ravenwood's open-world exploration phase begins.

## Important Rooms / Areas

- **South Gate** — Jim's entry point; only gate unlocked on arrival; can be bolted shut from
  inside once the park is cleared.
- **North / East / West Gates** — locked from the outside on arrival; function as **fast-travel
  shortcuts between city sections once unlocked from the city side** during district exploration
  (not direct entrances to the five main locations — the city itself must still be navigated).
- **The Guardhouse** — first safe room of Chapter 2; VERN terminal, inventory chest, corkboard
  documents, bollard override keycard.
- **The Founders Memorial / central water basin** — the five-emblem mechanism; will eventually
  drain to reveal a staircase underground (Chapter 3).
- Per the wider city map ([`STORY_NOTES.md`](../STORY_NOTES.md)), Memorial Park also contains benches, walking paths,
  and public restrooms per its own park map, though these are not individually scripted.

## Characters Encountered

None named — the park is deliberately deserted of survivors on arrival, reinforcing its "safe but
eerie" first impression.

## Creatures Encountered

- **Standard infected ("Shamblers")** — four inside the park on arrival; one on the street during
  the crossing. This is the confirmed first on-screen depiction of the base infected type
  referenced in passing during the hotel chapter.

## Puzzles

- **Bollard Override.** The street bollards deny access on arrival; the override keycard, found
  naturally on the guardhouse desk while clearing/exploring the park, lowers them.
- **How Jim learns about the crests (no exposition dump).** The groundskeeper's note says he's
  never understood the statue's five slots in nineteen years working the park, but recalls a
  historian once telling him "look at the police station... there's something on the wall inside
  the main hall you might find interesting." Combined with the plaque's five empty, labeled slots
  and the park map's four gates, this is enough for the player (and Jim) to reasonably head to the
  Police Station — the closest district — without ever being told outright what to do.
- **The statue's slots are the game's built-in directional hint.** Each empty wedge's position on
  the pentagon points in the general compass direction of the district its emblem belongs to (e.g.
  the wedge facing southwest belongs to the Police Station) — see [`CANON.md`](../CANON.md) →
  "The Founders & the Five Crests" for the full slot/direction/district table. This is readable
  directly off the statue on the very first visit, not something that only unlocks after finding
  an emblem elsewhere — the player can, in principle, work out the general direction of all five
  districts before ever leaving the park.

## Key Items

- **Bollard Override Keycard** — found on the guardhouse desk; lowers the street bollards.
- **Ravenwood Memorial Park Map** — found on the guardhouse corkboard; added to inventory.

### Documents (full text — see [`Scripts/Chapter_2_Ravenwood.md`](../Scripts/Chapter_2_Ravenwood.md))

- Road closure barrier notice (street, on the way to the park).
- Park maintenance schedule (guardhouse corkboard).
- Park map (guardhouse corkboard).
- Groundskeeper's two-page handwritten note (guardhouse corkboard) — the key document pointing
  toward the Police Station and the emblem mechanism.
- Founders plaque inscription and five slot engravings (central monument).

## Major Scripted Events

- Clearing the four infected inside the park on first arrival.
- Securing the south gate.
- Activating the VERN terminal / discovering the Founders Memorial for the first time.
- Lowering the bollards and opening the city.

## Boss Encounters

None at Memorial Park itself.

## Crest Progression

Memorial Park is the **return point** for the five-crest mechanic, not a source of a crest
itself. See [`CANON.md`](../CANON.md) ("The Founders & the Five Crests") for the full system. All five emblems
must be recovered from the five districts and inserted into the Founders Memorial plaque to drain
the water basin and reveal the staircase into the underground Vanguard facility (Chapter 3).

## Exit / Progression to Next Area

Once the street bollards are lowered, all of Ravenwood opens up. Exploration order for the five
districts is fully open, though the Police Station (Southwest, closest to the park) is the
natural first destination given the guardhouse note and its proximity. See [`STORY_NOTES.md`](../STORY_NOTES.md) for
the city map and the secondary-location list for each district, none of which are written
scene-by-scene yet.
