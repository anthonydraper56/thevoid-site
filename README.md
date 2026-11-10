# The Void — website (textured edition, 10 Nov 2026)

Static site. No build step, no JavaScript framework.

- index.html, about.html, archive.html, books.html, submit.html — the five pages
- base.css — base tokens; texture.css — paper, type, stamps, and seasonal ephemera (shared by every page)
- uploads/ — fonts, textures, covers, portraits
- favicon.png, og.png

## Deploying

Upload everything in this folder, folders included, to the repo root (GitHub web UI: "Add file → Upload files", drag the whole folder contents in, commit). The pages expect `uploads/`, `base.css`, and `texture.css` to sit beside them.

## Each issue

- Seasonal ephemera: replace the six files in `uploads/texture/season/` (ephemera-1.png … ephemera-6.png). Same names, every page picks them up.
- Contents and contributors live in the page HTML (archive.html, index.html "In this issue", about.html credits).
