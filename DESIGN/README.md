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

15. **Never create a new branch for Deadlock design work unless explicitly told to.** All design
    documentation changes should continue landing on the existing working branch/PR
    (`cursor/design-docs-structure-e231` →
    [PR #1](https://github.com/GIToez/Deadlock-Design/pull/1)) rather than spinning up a fresh
    branch per request.
    - Note: as a Cursor cloud agent, changes still go through a pull request rather than being
      pushed straight to `main` directly — that review step is a platform-level constraint, not a
      per-task choice. "No new branches" is honored by continuing to reuse one branch/PR for all
      of this work instead of creating additional ones.
