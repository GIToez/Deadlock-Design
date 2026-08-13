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
- **Directly alongside a character/creature/location file** is also fine and used in practice —
  e.g. `Characters/spr_cindy_jumpscare.gif` sits right next to `Characters/Cindy_Sweets.md` and is
  embedded directly in it. Use whichever placement makes more sense for a given asset; there's no
  requirement to funnel everything into this folder specifically.

## How to add a file

Cursor cloud agents can't save images pasted directly into chat to disk — only files pushed as
real commits to the branch (the same way `AI.json` and the story `.docx` were added) become
accessible here. Push new images/GIFs into `DESIGN/Assets/Screenshots/` or `DESIGN/Assets/Reference/`
directly (e.g. via the GitHub web UI), using a short, descriptive filename
(`cindy_jumpscare.gif`, `ravenwood_hotel_lobby_overview.png`).

## Current files

- **`Reference/founders_memorial_plaque_concept.png`** — AI-generated concept art for the
  Founders Memorial's medallion-plaque (Memorial Park, Chapter 2): the central pentagon "V" hub
  and the five wedge slots, two shown filled/glowing and three empty, for visual reference only —
  not a literal in-game screenshot. Referenced from
  [`CANON.md`](../CANON.md) and [`Locations/Memorial_Park.md`](../Locations/Memorial_Park.md).
- **`Reference/ashen_hound_concept.png`** — AI-generated concept art for the
  [Ashen Hound](../Creatures/Ashen_Hound.md) ("Diesel," the Municipal Garage K-9 encounter,
  Chapter 2). Referenced from `Creatures/Ashen_Hound.md`.

One other asset has been uploaded, placed directly alongside its character file instead:
`Characters/spr_cindy_jumpscare.gif`, embedded in
[`Characters/Cindy_Sweets.md`](../Characters/Cindy_Sweets.md).

## Convention: concept art for new enemies and bosses

Once a new enemy or boss creature's design is written up in `Creatures/`, generate one piece of
concept art for it as standard practice going forward (not just for one-off cases like the
Founders Memorial). Guidelines:

- **Filename:** `Reference/<creature_name>_concept.png`, lowercase with underscores, matching the
  creature's `Creatures/<Name>.md` filename (e.g. `Ashen_Hound.md` → `ashen_hound_concept.png`).
- **Base the prompt strictly on what's already locked** in the creature's own file (Appearance,
  Behavior) plus [`CANON.md`](../CANON.md)'s general infected traits (pale/clouded eyes, "wrong"
  stiff movement or, for fast types, low predatory posture) — don't invent new canon-affecting
  details in the image prompt alone. If the generated image suggests a good new visual detail not
  yet written down (e.g. the Ashen Hound's visible dark vein-like discoloration, a nod to "Black
  Vein" itself), fold it back into the creature's own Markdown file afterward so the prose and the
  art stay in sync — the image should never be the only place a design detail lives.
- **Style:** moody digital concept-art painting, desaturated/muted palette, dramatic low-key
  lighting — consistent with both existing reference images. These are mood/reference art, not
  literal in-game screenshots (2.5D top-down), and should say so explicitly wherever embedded.
- **Embed it directly in the creature's own file** (top or near the Appearance section) with a
  one-line caption explaining what it shows and that it's reference art, then add it to the
  "Current files" list above.
- This same convention applies to bosses (e.g. a future Founders Memorial-style piece for a major
  district boss) and to major unique creatures generally, not just recurring enemy classes.
