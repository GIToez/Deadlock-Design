# Deadlock Protocol — Story Design Documentation

This folder contains the story-design documentation for Deadlock Protocol.

## Structure

```
DESIGN/
├── MASTER_STORY.md      # Human-readable master storyline (beginning to end)
├── CANON.md              # Locked, established facts only — concise
├── STORY_NOTES.md        # Brainstorming / unresolved ideas — not canon
├── Characters/           # One file per significant recurring character
├── Creatures/             # One file per important creature type / major unique creature
├── Locations/             # One file per major location (complete design for that location)
├── Weapons/               # One file per weapon (stats, description, concept art)
├── Items/                 # One file per consumable/utility item (effects, description, concept art)
└── Scripts/               # Programmer-facing, scene-by-scene game scripts (dialogue + actions)
```

## AI Story Rules

When working on Deadlock story content:

1. Read [`CANON.md`](CANON.md) first.
2. Read [`MASTER_STORY.md`](MASTER_STORY.md) for overall context.
3. Read the relevant location, character, and creature documents for the part of the story
   being discussed.
4. Search the `DESIGN/` folder for additional relevant information when needed.
5. Never silently retcon established information.
6. If two documents conflict, report it rather than resolving it silently.
7. Do not invent missing facts and present them as existing canon.
8. New ideas should remain proposals (in [`STORY_NOTES.md`](STORY_NOTES.md)) until explicitly approved.
9. Once an idea is explicitly approved, update the appropriate document(s).
10. Preserve existing material unless a rewrite is specifically requested.
11. Prioritize story continuity over inventing something new.
12. This is a survival-horror **video game**, not a novel — story development should consider
    gameplay, exploration, pacing, puzzles, encounters, and player agency.

## Content Rating & Tone

13. **Deadlock Protocol is a mature-rated (M) game. Do not self-censor by default.** Explicit
    violence, blood, and gore; strong profanity in dialogue; and nudity are all permitted where
    the scene calls for it — this is a survival-horror game, not a "teen"-rated one, and
    sanitized reactions to horrific things read as less real, not more tasteful. This applies to
    all future scene and dialogue writing (new districts, Chapter 3, the Epilogue, and any
    revisions).
    - This does not mean escalating content gratuitously for its own sake — it means not
      dialing back intensity, language, or physical detail that the scene already calls for.
    - Existing "locked" material (`Scripts/Chapter_1_One_Night_Only.md`) was written before this
      direction was given and reads comparatively restrained (e.g. Jim's strongest reaction on
      the page is "...Jesus Christ."). Per rule 10, it hasn't been rewritten to match — ask if you
      want a punch-up pass on it specifically.

## Presentation & Camera

14. **This is a 2.5D top-down game — write scenes accordingly.** The camera stays close to the
    player and shows roughly a room's-width of space at a time, not a wide cinematic view of an
    entire location, and there is no implied 3D camera movement (no pans, dollies, over-the-
    shoulder shots). When describing a scene, favor what's near/visible to Jim as he moves rather
    than an omniscient wide shot — unless a moment is explicitly meant to be a deliberate wider
    vista/cutscene beat (rare; flag it as such when it happens). See
    [`CANON.md`](CANON.md) → "Presentation & Perspective" for the full note and reference
    screenshots in [`Assets/`](Assets/README.md) once uploaded.

## Repository / Workflow Rules

15. **Work directly on `main`, and only `main` (locked 2026-08-13, supersedes the original
    branch/PR-based version of this rule).** The project owner explicitly instructed: "From now on
    we work on the main branch in only the main branch." All design documentation changes —
    including new folders/files, edits, and asset additions — should be committed and pushed
    straight to `main`. Do not create feature branches or pull requests for this work going
    forward. (The earlier working branch, `cursor/design-docs-structure-e231`, was merged into
    `main` via [PR #1](https://github.com/GIToez/Deadlock-Design/pull/1) and
    [PR #2](https://github.com/GIToez/Deadlock-Design/pull/2) and then deleted — there is no longer
    a separate working branch to reuse.)

## Visual Asset Pipeline (locked 2026-08-13)

16. **Every new scene/room, new enemy/creature, new named character, new weapon, and new item gets
    a matching visual render as part of finishing it — not as a separate follow-up pass.** This is
    a permanent rule, not a one-off request, so animators/artists always have something concrete to
    work from and the whole cast/world stays visually consistent as it grows:
    - **New room or scene** → a room concept image, following the convention in
      [`Assets/README.md`](Assets/README.md) → "Convention: room concept art" (style-anchored to
      the real in-engine Hotel screenshots in `Assets/Screenshots/`).
    - **New enemy or creature** → concept art, following [`Assets/README.md`](Assets/README.md) →
      "Convention: concept art for new enemies and bosses."
    - **New named character** (including ones never seen alive on-screen) → a reference portrait,
      following [`Characters/README.md`](Characters/README.md) → "Convention: reference portraits
      for named characters" — this is the PixelLab `create_image_pro` two-step pipeline
      specifically, confirmed 2026-08-13 to be what actually matches the project's house style;
      don't substitute a generic image generator for it.
    - **New weapon or item** → a small pixel-art inventory icon, following
      [`Weapons/README.md`](Weapons/README.md) → "Convention: concept art for weapons" or
      [`Items/README.md`](Items/README.md) → "Convention: concept art for items" — a distinct,
      simpler icon style from the room/creature painterly convention above, confirmed against
      actual in-game item-icon references (2026-08-13, see
      [`STORY_NOTES.md`](STORY_NOTES.md)). The project owner may also upload real in-game icons
      directly for specific weapons/items instead of generating them — check each file/folder's
      current status before generating one, so a generated placeholder doesn't get made redundant.
    - Each convention document is the source of truth for exact style/technical details (filename
      patterns, sizes, prompt templates) — this rule just states that the step is mandatory, not
      optional, going forward.
