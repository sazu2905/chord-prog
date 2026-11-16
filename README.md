# Changes — Chord Progression Builder

A single-page app for composing chord progressions: build a progression, loop it, rearrange it, and hear it in different keys and modes with a drum groove underneath.

Open `index.html` in a browser. Everything is in that one file (HTML, CSS, JavaScript and a Web Audio synth), with no build step and no dependencies apart from Google Fonts.

## Features

- **Chord palette:** 12 roots and 33 chord qualities (triads, sixths and sevenths, extensions, altered dominants), optional slash bass, chord lengths of 1–8 beats.
- **Key & mode:** 9 modes (the church modes plus harmonic and melodic minor), the mode's chords as triads or 7ths, Roman-numeral analysis, sharp/flat spelling.
- **Re-key / re-mode:** changing key or mode moves the whole progression by scale degree (e.g. G major ii–V–I becomes Aø7–Dm7–Gm7 in G minor), with undo/redo to compare.
- **Playback:** loop with play/pause/stop, tempo, 4/4 or 3/4, click, bass, three sounds (Keys, Pad, Organ), three rhythms (Held, Charleston, Quarters), smooth voice leading.
- **Arranging:** drag to reorder (mouse or touch), edit chords in place, duplicate, move, delete, transpose, undo/redo, copy as a text chord chart.
- **Multi-select:** box-select by dragging across empty space, Shift-click ranges, Ctrl/⌘-click to toggle (or the Multi-select toggle on touch). Copy, cut, paste and duplicate whole sections, including between saved progressions. Drag a selection to move it; hold Alt while dropping to copy it. Type and length edits apply to every selected chord.
- **Files:** New, Save, Save as… and Open, with an unsaved-changes indicator and a prompt before anything on screen would be replaced.
- **Import / export:** export any or all saved progressions as JSON (copy or download), including key, mode, tempo, meter, drum settings and a readable chord chart. Import from a `.json` file or pasted JSON; entries are validated, unreadable ones are skipped, and name clashes can be kept side by side or replaced.
- **Staff view:** a read-only grand staff showing the exact piano voicing and bass note played for every chord, highlighted during playback, with a First time / On repeat switch where voice leading voices the loop differently.
- **Drums:** 8 styles, presence sliders for kick, snare, hats, cymbals and toms, auto fills, swing, and an expandable 16-step sequencer with accents and ghost notes. The panel collapses to a single line so the beat can keep running out of the way.
- **Inspire me:** generates a random 8-bar progression in the current key in a chosen style (jazz standard, bossa nova, neo-soul, gospel, 8-bar blues, pop, modal vamp, or surprise me). Audition it, then start a new progression from it or insert it into the current one.

## Keyboard

`Space` play/pause · `Enter` add chord · `Ctrl/⌘` + `C` `X` `V` `D` `A` copy, cut, paste, duplicate, select all · `Ctrl/⌘+S` save (`Shift` for Save as) · `←` `→` select · `Shift`+`←` `→` extend selection · `Alt`+`←` `→` move · `Del` remove · `Esc` deselect · `Ctrl/⌘+Z` undo

## Storage

Progressions and settings are saved in the browser's `localStorage`. Nothing is uploaded, so saved progressions stay on the device and browser where they were made. Use Open → Export / Import to move them between browsers or devices.

## Roadmap

- Package as a progressive web app (manifest, service worker, offline support).
