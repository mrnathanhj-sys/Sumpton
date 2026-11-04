# Sumpton Underworld Map

An interactive, RPG-style map of Sumpton, the underworld beneath Dumpton, built from the *Sumpton Schematic* draw.io file.

- **Tap a mission** (hexagon) to see where it leads and open its mission brief PDF.
- **Tap a realm** (or its banner) to read its lore from *Realms of Sumpton*.
- **Missions** button opens a searchable index plus every pack and reference PDF.
- Drag to pan, scroll or pinch to zoom. Links like `#temple-of-the-crucifish` or `#realm-drowned` open straight to that entry.

## Publishing on GitHub Pages

1. Repo **Settings → Pages**.
2. **Source:** Deploy from a branch → `main` / root → Save.
3. The site appears at `https://mrnathanhj-sys.github.io/Sumpton/` after a minute.

## Updating

Everything lives in `index.html`:

- `NODES`: missions (position, realm, `pdf` = Google Drive file ID).
- `REALMS`: realm shapes and lore text.
- `EDGES`: routes between missions.
- `TRACKER`: realm completion status from the Game Tracker sheet.

Missions without a brief in the Game Tracker (Forgotten Riches, Gambit's Jeopardy, The God King) show a "no brief linked" note; add a `pdf` ID to link them.
