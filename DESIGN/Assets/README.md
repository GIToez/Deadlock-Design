# Assets

Reference images, concept art, and gameplay screenshots/GIFs for Deadlock Protocol. These are
visual reference material, not story content — cross-link to them from the relevant
`Locations/`, `Characters/`, `Creatures/`, or `Scripts/` file with standard markdown image syntax:

```markdown
![Ravenwood Hotel Lobby — full layout reference](../Assets/Screenshots/ravenwood_hotel_lobby.png)
```

## Suggested organization

- **`Screenshots/`** — actual in-engine/gameplay captures (stills or GIFs). These are the most
  reliable source of truth for art style, camera framing, and what the player actually sees —
  more trustworthy than prose descriptions when the two disagree. If a screenshot contradicts
  something written elsewhere, flag it rather than silently rewriting the screenshot's intent.
- **`Reference/`** — concept art, mood boards, or AI-generated placeholder visuals used for
  discussion rather than as ground truth.

## How to add a file

Cursor cloud agents can't save images pasted directly into chat to disk — only files pushed as
real commits to the branch (the same way `AI.json` and the story `.docx` were added) become
accessible here. Push new images/GIFs into `DESIGN/Assets/Screenshots/` or `DESIGN/Assets/Reference/`
directly (e.g. via the GitHub web UI), using a short, descriptive filename
(`cindy_jumpscare.gif`, `ravenwood_hotel_lobby_overview.png`).

## Current files

_None yet — first uploads pending._
