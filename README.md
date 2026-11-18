# The Void — website (17 Nov 2026: textured pages on a walnut desk, Editorial Services)

Static site. No build step, no JavaScript framework.

- index.html, about.html, archive.html, books.html, submit.html, editorial.html — the six pages
- base.css — base tokens; texture.css — paper, desk, type, stamps, and seasonal ephemera (shared by every page)
- uploads/ — fonts, textures, covers, portraits
- favicon.png, og.png

## Deploying

Upload everything in this folder, folders included, to the repo root on main (GitHub web UI: "Add file → Upload files", drag the folder's contents in, commit). The pages expect `uploads/`, `base.css`, and `texture.css` to sit beside them.

## Each issue

- Seasonal ephemera: replace the six files in `uploads/texture/season/` (ephemera-1.png … ephemera-6.png). Same names, every page picks them up.
- Contents and contributors live in the page HTML (archive.html, index.html "In this issue", about.html credits).

## Credits

- Desk texture: "Wood 060" from ambientCG (ambientcg.com), CC0 public domain.
