# Ashen Hound

> Proposed (2026-08-13) as the game's second infected-creature classification, introduced in the
> Southwest District (Municipal Garage) to answer the "at least one major encounter" requirement
> each district needs per [`AI.json`](../AI.json)'s city-design notes. Treat this as a draft pending
> review, same as any new creature type.

## Concept

The game's first **fast** infected type — a deliberate contrast to the [Shambler](Shambler.md)'s
slow, deliberate movement. Introduced as a pair (named individuals **Diesel** and **Baxter**,
Ravenwood PD's K-9 unit dogs) rather than a single unique encounter, establishing "Ashen Hound" as
a recurring creature class the other districts can draw on, not a one-off boss.

## Origin

A domestic animal (specifically, in this first appearance, a police service dog) infected with
**Black Vein** (see [`CANON.md`](../CANON.md)). Presented as evidence that Black Vein isn't
exclusively a human-infection agent — it crosses to at least some animals, and does so with a
different mutation profile than it produces in humans: speed and aggression over the Shambler's
slow-and-relentless presentation.

## Appearance

Larger than the source animal, musculature visibly wrong beneath a hide gone patchy and
ash-gray — the same "wrong" quality as human infected, expressed differently. Eyes carry the same
pale, clouded look established across every other infected creature. Moves low to the ground, head
level with its shoulders rather than raised.

## Behavior

Fast, low, and — critically — **pack-hunting**: Diesel and Baxter circle rather than approach in a
straight line, splitting up to flank instead of both closing from the same direction. This is a
deliberate design contrast with every enemy encountered so far (Shamblers, the Caretaker, The
Maw), none of which hunt cooperatively. Vocalizes with a low, wet growl before committing to a
charge, giving the player an audio tell distinct from a Shambler's silence-until-it's-close
approach.

## Gameplay Role

The Southwest District's signature encounter (per [`AI.json`](../AI.json)'s "at least one major
encounter or boss" rule for each district) — a genuine difficulty/pacing spike introduced right
after the player has just been rewarded with the shotgun (see
[`Scripts/Chapter_2_Ravenwood.md`](../Scripts/Chapter_2_Ravenwood.md), Scene 27), so the timing is
deliberate: new weapon, immediately tested against an enemy type the bat and handgun alone would
struggle with. Not framed as a full boss fight on the Caretaker's scale — no phases, no unique
arena mechanic — just a hard, fast, two-on-one fight in a cluttered vehicle yard that punishes
standing still.

## Encounter Progression

- First (and so far only) appearance: Municipal Garage / Impound Lot, Southwest District
  ([`Scripts/Chapter_2_Ravenwood.md`](../Scripts/Chapter_2_Ravenwood.md), Scene 32) — found via
  their unit transport van, kennel doors open, leash chewed through.
- Expected to recur as a creature class in later districts (not yet decided which ones); this file
  establishes the baseline for any future Ashen Hound encounters so they don't need to be
  redesigned from scratch.

## Major Appearances

- [`Scripts/Chapter_2_Ravenwood.md`](../Scripts/Chapter_2_Ravenwood.md), Scene 32 (Diesel and
  Baxter, Municipal Garage).

## Story Significance

Minor but deliberate: confirms Black Vein affects animals as well as humans, without turning that
into a larger plot point yet. Diesel's collar tag gives the encounter a small, specific moment of
sadness (Jim reads it; doesn't check the second dog's) consistent with the game's general approach
to infected who were people — or, here, someone's working animal — before the outbreak.

## Open Design Gap

No formal combat spec (health, attack patterns, exact speed/range values) has been written yet —
same gap flagged for the Shambler in its own file. This entry establishes concept/lore/behavior
only.
