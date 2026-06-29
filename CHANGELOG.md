# Changelog — Modal Fretboard

## v1.2 — Build 26062803 (2026-06-28)

### Changes
- Fret numbers pushed further below neck — no longer overlaps note dots
- Triads view: interval labels are now chord-relative (Dm shows R, b3, 5 — not 2, 4, 6)
- Added **7ths view** — diatonic 7th chord arpeggios (Cmaj7, Dm7, Em7, Fmaj7, G7, Am7, Bø7) with chord-relative labels (R, b3, b5, b7 etc.)
- Legend: "Triad" → "Chord tone" (applies to both triads and 7th arpeggios)
- Control row label dynamically switches between "Triad" and "7th" based on view

---

## v1.1 — Build 26062802 (2026-06-28)

### Changes
- Triads view: non-triad scale notes now appear as faded ghost dots (context without clutter)
- View button "Box" renamed to "3NPS" (3 notes per string)
- #/b notation toggle now updates Key button labels and the info title
- Legend: "Scale note" → "Scale tone"

---

## v1.0 — Build 26062801 (2026-06-28)

Initial public release.

### Features
- SVG fretboard visualizer for all 7 modes of the major scale
- All 12 keys supported
- Three views: Box position (5-fret window), 15 frets, 24 frets
- Label toggle: interval names (R, b3, 6…) or note names (D, F, B…)
- Dot color hierarchy: Root (orange) · Butter Notes (yellow) · Scale notes (blue)
- String orientation matches guitarist's perspective — low E at bottom, high e at top
- String thickness scales with gauge (low E thickest)
- Fret position dots and double dots at 12/24

### Music theory
- Butter notes: the 3rd of every scale is always highlighted, plus the interval(s) that uniquely define each mode vs its neighbors

### Design
- Light is Beauty brand: Syne 800 title, DM Mono labels, Proximity Blue (#3EB8F0) accents
- Neutral grey fretboard on dark navy background
- Deployed as GitHub Pages at https://lightisbeauty.github.io/Modal/
