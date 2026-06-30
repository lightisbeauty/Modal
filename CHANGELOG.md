# Changelog — Modal Fretboard

## v1.5 — Build 26062908 (2026-06-29)

### Pad audio

- Added **♪ Pad button** — drones the I chord of the current key/mode as a sustained pad (slow attack, LPF warmth, convolution reverb)
- Button displays the live chord name in Syne 800 (e.g. "D", "Dm7") — updates with key and mode
- In **7ths view** the pad plays and labels the full 7th chord (Dmaj7, G7, Am7, etc.)
- Pad **persists across all navigation** — changing triads, view, or labels doesn't stop it
- Switching **key or mode crossfades** (~0.35s) to the new I chord in real-time
- Switching between Triads and 7ths views also triggers a crossfade to the correct voicing
- Button pulses with a slow blue glow at rest; turns solid magenta while playing
- Button positioned to the right of the chord strip with a matching vertical separator

### Chord mode colors

- **Butter notes stay yellow in chord mode** — chord tones that are also characteristic intervals (e.g. F# in Bm over D Lydian) now render yellow on the fretboard and in the chord strip, not magenta
- **Key center root fades** when a chord is selected and the key root is not the chord root — shown as a faint orange ghost circle (no label) to eliminate the competing-roots confusion

### Chord info strip

- Added **chord info panel** next to the key note strip — visible in Triads and 7ths view whenever a chord is selected
- Shows chord name (in magenta) + a row of tone badges with chord-relative interval labels (R, b3, 5 etc.) and note names
- Butter-note chord tones show in yellow within the strip

---

## v1.4 — Build 26062901 (2026-06-29)

### Changes

- **Key center root fades** in Triads/7ths view when it is not the chord root (initial implementation)
- **Chord info strip** added alongside the key note strip (initial implementation)
- **upper-extensions.html Lydian walkthrough fixed** — step order now shows butter notes in 15-fret view before entering Triads, so F# correctly appears yellow when switching to Lydian

---

## v1.3 — Build 26062804 (2026-06-28)

### Changes

- In Triads/7ths view, all visible dots are now magenta — the key-center orange root is suppressed to avoid competing roots
- **Chord root** distinguished by a white glow ring (3px halo) around the magenta dot
- Version/build tag added to bottom of page

---

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
