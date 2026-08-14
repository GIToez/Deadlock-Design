# Downtown Ravenwood

> A new (2026-08-14) `Locations/` file for the Downtown intro stretch of Chapter 2 — Pearl's Diner,
> the Ravenwood Public Library, and City Hall — which previously existed only as scenes inside
> [`Scripts/Chapter_2_Ravenwood.md`](../Scripts/Chapter_2_Ravenwood.md) (Scenes 19–21) with no
> matching `Locations/` entry or concept art of its own. Flagged by the project owner directly:
> *"there's some that's not located like Pearl's diner I don't see it within the locations
> tab."* Unlike the five main districts, Downtown is a short, **linear** stretch (no keys, no
> backtracking, no crest) — the story's first look at the wider city, between Memorial Park and the
> open-order district phase. See [`Locations/Memorial_Park.md`](Memorial_Park.md) for the park
> itself, which this file picks up immediately after.

## Purpose in the Overall Story

The player's first extended look at Ravenwood beyond the hotel and the park — three ordinary civic
buildings (a diner, a library, a government building) that establish the city as a real, lived-in
place before Jim ever reaches the five open-order districts. Each stop plants a specific piece of
foreshadowing (the library's Black Vein survey map and North Ridge animal-death clipping; City
Hall's official emergency-response recordings) without yet explaining what any of it means.

## Arrival / Setup

Jim reaches Downtown immediately after lowering Memorial Park's street bollards — see
[`Locations/Memorial_Park.md`](Memorial_Park.md) → "Exit / Progression to Next Area". The scale of
the outbreak becomes visible for the first time: swinging traffic lights (some still cycling,
others dead), a car alarm wailing somewhere deeper in the city, smoke rising from a building two
streets east.

## Storyline

- **Pearl's Diner.** A classic 24-hour roadside diner on the corner of Main Street and Caldwell
  Avenue — neon sign still buzzing unevenly, front windows partially shattered, door hanging open.
  Recently abandoned rather than long-dead: coffee cups still on the counter, a half-eaten plate at
  a booth, a jukebox still quietly cycling through songs. A handwritten note taped to the register
  explains the owner left to check on a specific family on Dellwood Street. Supplies available:
  food items, a Medkit behind the counter, a flashlight in the lost-and-found box.

  ![Pearl's Diner — room concept](../Assets/Reference/downtown_pearls_diner_concept.png)

  > AI-generated room concept (2026-08-14). Matches the scripted checkerboard floor, neon "Pearl's
  > Diner" signage, counter stools, and jukebox closely — the diner's name rendered correctly and
  > legibly, unlike several earlier districts' recurring AI naming errors.
- **The Ravenwood Public Library.** A 1930s civic building on Jefferson Street, one door hanging
  open. Dark except for red emergency exit lighting; tall shelves cast long shadows over an
  overturned reading room. The reference section at the rear holds the first hint of Black Vein by
  name: a geological survey map of the mountain region with tunnel sections circled in red pen and
  clinical marginal notes, plus a bound newspaper archive whose most recent edition reports the
  Steelgate Refinery's "temporary closure" and unusual animal deaths near North Ridge — both later
  confirmed as real warning signs rather than coincidence (see
  [`Locations/Foundry_Refinery.md`](Foundry_Refinery.md) and
  [`Locations/Police_Station.md`](Police_Station.md) → "The Interview Room").

  ![Ravenwood Public Library — room concept](../Assets/Reference/downtown_public_library_concept.png)

  > AI-generated room concept (2026-08-14). Matches the scripted overturned reading tables,
  > scattered books, librarian's cart, and children's reading corner closely.
- **City Hall.** Dominates the north end of the downtown plaza — stone columns, wide steps, a flag
  still flying from the rooftop in the storm. The main entrance is barricaded from the inside with
  visible furniture; a side maintenance entrance remains accessible. Inside: a locked mayor's office
  (second floor, key required, not yet recovered), a city council chamber, and a basement emergency
  operations room still partially active on backup power — active radio equipment, a hand-drawn
  evacuation-route whiteboard with every route crossed out one by one, and a personal recorder left
  on the desk holding Deputy Administrator Carl Hess's three audio-log entries tracking the official
  government response collapsing in real time.

  ![City Hall — room concept](../Assets/Reference/downtown_city_hall_concept.png)

  > AI-generated room concept (2026-08-14). Matches the scripted barricaded main lobby, Council
  > Chambers signage, and the Emergency Operations room's crossed-out evacuation-route whiteboard
  > closely.

## Important Rooms / Areas

- Pearl's Diner (supplies: food, Medkit, flashlight)
- Ravenwood Public Library (lore: geological survey map, newspaper archive)
- City Hall — Main Lobby (barricaded), Council Chambers, Mayor's Office (locked, key not yet
  recovered), Emergency Operations Room (basement, active radio + audio log)

## Characters Encountered

None named — Downtown is deliberately empty of survivors on this pass, consistent with
[`AI.json`](../AI.json)'s original framing of this stretch as scene-setting rather than a combat or
NPC beat.

## Creatures Encountered

None scripted in this stretch — Downtown is a quiet, exploratory interlude between Memorial Park
and the first open-order district.

## Puzzles

None — this is a deliberately linear, non-gated stretch. No keys, no locks, no backtracking; the
one locked door (the Mayor's Office) is left unresolved rather than turned into a puzzle here.

## Key Items

None. Downtown yields lore/documents and ordinary supplies only, no key/puzzle items.

### Documents

- Pearl's own handwritten note (register) — she went to check on the Hargrove family on Dellwood
  Street.
- Geological survey map (library reference section) — Black Vein circled by name, in a precise,
  clinical hand predating the outbreak.
- Bound *Ravenwood Gazette* newspaper archive (library reference section) — "STEELGATE REFINERY
  ANNOUNCES TEMPORARY CLOSURE" and "UNUSUAL ANIMAL DEATHS REPORTED NEAR NORTH RIDGE," both dated
  three weeks before the outbreak.
- Carl Hess's three-entry audio log (City Hall, Emergency Operations Room) — the official
  government response, ending on Deadlock Protocol's authorization.
- Hand-drawn evacuation-route whiteboard (City Hall, Emergency Operations Room) — every route
  crossed out, one by one.

## Major Scripted Events

- Reading the geological survey map and newspaper archive at the library — the game's first
  explicit, in-world mention of "Black Vein" by name.
- Playing Carl Hess's audio log at City Hall — the last official government account of the night,
  ending mid-collapse.

## Boss Encounters

None.

## Crest Progression

Not applicable — Downtown is not one of the five crest districts.

## Exit / Progression to Next Area

After City Hall, Jim leaves the downtown grid and reaches the Southwest District — see
[`Scripts/Chapter_2_Ravenwood.md`](../Scripts/Chapter_2_Ravenwood.md), Scene 22, continuing into
[`Scripts/Chapter_2_Police_Station.md`](../Scripts/Chapter_2_Police_Station.md).

## Unresolved Ideas

- The Mayor's Office (City Hall, second floor) is locked and its key never recovered anywhere in
  the currently-written material — a deliberate loose end, not yet decided whether it should ever
  be opened.
- Whether Downtown deserves any optional combat/survivor content of its own, or should stay exactly
  as quiet and exploratory as it's currently written — not decided; flagged rather than changed
  without direction.
- Full scene-by-scene script already exists ([`Scripts/Chapter_2_Ravenwood.md`](../Scripts/Chapter_2_Ravenwood.md),
  Scenes 18–21) and predates this file; this `Locations/` writeup was assembled retroactively from
  that script, matching the reverse of how most other locations were written (script written after
  the `Locations/` file). Flagged in case any future edit to one drifts out of sync with the other.
