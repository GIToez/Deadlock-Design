# Shambler

## Concept

The game's **standard, base-tier infected** — the ordinary "zombie" the player will encounter
constantly, everywhere, for the whole game. Everything else (Earl Whitaker's first-reveal
encounter, Officer Pruitt, Della Marsh, and named bosses like the Caretaker) is a variation,
escalation, or named/scripted instance built on top of this baseline; the Shambler itself is the
default population of infected Ravenwood.

## Origin

A person infected with **Black Vein** (see [`CANON.md`](../CANON.md)) who has progressed to the disease's common,
early/mid infection state — mutated just enough to become violently hostile and physically wrong,
but not into one of the more severe mutation-stage creatures (like the Caretaker) that the game
treats as unique, named encounters.

## Appearance

Not fully detailed yet as a distinct design spec (see [`STORY_NOTES.md`](../STORY_NOTES.md) — this was flagged during
the original docx audit as a documentation gap: it's referenced by name but was never given its
own write-up). Behaviorally consistent traits observed across every infected encountered so far:
pale, "wrong" eyes; blood around the mouth; jaw sometimes hanging at an unnatural angle; stiff,
locked-in, non-human movement that lacks the small unconscious adjustments a living person makes.

## Behavior

Aggressive toward the living. Movement is deliberate but **not intelligent** in the way the
Caretaker is — the design notes for that boss explicitly define shamblers by contrast: *"Unlike
shamblers: the caretaker is intelligent enough to pursue and corner the player aggressively."*
Shamblers are the baseline the game's mutation-stage creatures are meant to read as a step above.
In practice on-screen so far: they wander, they notice the player at range and close in, and they
can sometimes be avoided in the open rather than fought (see the Chapter 2 street-crossing scene).

## Gameplay Role

The bread-and-butter combat encounter of the entire game — manageable one-on-one, meant to be
handled with the baseball bat and, later, the handgun. In the Ravenwood Hotel (Chapter 1), they're
placed as corridor/room encounters — sometimes an ambush timed to an item pickup (the Utility
Room screwdriver), sometimes just a room the player wasn't expecting one in, and once, deliberately,
as a **two-Shambler pincer** (second-floor west hallway, Scene 35) that removes the player's usual
option to just retreat — rather than an open avoid-or-engage choice, since the hotel's tight
interiors don't really allow for that. Once the game opens up outdoors (Chapter 2 onward), that
changes: used to gate/populate open spaces (e.g. the four shamblers inside Memorial Park on first
arrival) and to give the player real agency (avoid vs. engage, as established explicitly in Chapter
2's street crossing).

## Encounter Progression

- First **directly depicted on-screen**: throughout the Ravenwood Hotel during the East/West Wing
  power-restoration loop (Chapter 1) — nine total, spread across both wings: seven one-on-one
  placements (second-floor east hallway, Dining Hall, Utility Room, Lounge/Recreation, Main Bar,
  Boiler Room, West Wing Service Corridor) plus a **two-Shambler pincer ambush** in the
  second-floor west hallway (Scene 35) — the chapter's first no-clean-retreat combat moment,
  sprung from two guest-room doors on opposite sides of the player. Deliberately not in every room,
  so placement stays unpredictable rather than a checklist. See
  [`Locations/Ravenwood_Hotel.md`](../Locations/Ravenwood_Hotel.md) → "Creatures Encountered" for
  the full room-by-room list. (This retcons an earlier draft where Shamblers were only referenced
  by name in Chapter 1, not actually fought — see [`STORY_NOTES.md`](../STORY_NOTES.md), approved
  directly by the project owner, 2026-08-13.)
- Also referenced by name during the Caretaker's design notes in the same chapter, contrasting the
  Caretaker's pursuit intelligence against baseline Shambler behavior.
- The lone infected during the Chapter 2 street crossing
  ([`Scripts/Chapter_2_Ravenwood.md`](../Scripts/Chapter_2_Ravenwood.md), Scene 3) — the player's first explicit choice to avoid or
  engage a shambler in open, non-corridor space.
- Populates Memorial Park on first arrival (four shamblers — [`Scripts/Chapter_2_Ravenwood.md`](../Scripts/Chapter_2_Ravenwood.md),
  Scene 6) before the park is secured as a safe hub.
- Expected to recur throughout the five districts and the rest of the city (not yet scripted).

## Major Appearances

- [`Scripts/Chapter_1_One_Night_Only.md`](../Scripts/Chapter_1_One_Night_Only.md), Scenes 30, 31, 32, 35 (×2, pincer ambush),
  37 (×3), and 39 — nine total corridor/room encounters throughout the hotel.
- Referenced by name (not shown) in [`Scripts/Chapter_1_One_Night_Only.md`](../Scripts/Chapter_1_One_Night_Only.md), Scene 44 (Caretaker
  boss design notes).
- [`Scripts/Chapter_2_Ravenwood.md`](../Scripts/Chapter_2_Ravenwood.md), Scenes 3 and 6.

## Story Significance

None beyond establishing Black Vein's basic infection presentation — shamblers are population,
not plot. Named/scripted infected (Earl, Officer Pruitt) behave consistently with this baseline
(stiff, locked-in movement; "wrong" eyes) even though they're narratively distinct, named
characters rather than anonymous shamblers — they read as the same underlying infection state,
just with a face and a story attached.

## Open Design Gap

A full combat design spec (health, specific attack patterns, sound design, visual variants) has
not been written yet — flagged in [`STORY_NOTES.md`](../STORY_NOTES.md). This file establishes the concept/lore/behavior
baseline; a follow-up pass should add the mechanical specifics once combat design work begins.
