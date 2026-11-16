# Changes — Chord Progression Builder

A single-page app for composing chord progressions: build a progression, loop it, rearrange it, and hear it in different keys and modes with a drum groove underneath.

Open `index.html` in a browser. Everything is in that one file (HTML, CSS, JavaScript and a Web Audio synth), with no build step and no dependencies apart from Google Fonts.

## Features

- **Chord palette:** 12 roots and 33 chord qualities (triads, sixths and sevenths, extensions, altered dominants), optional slash bass, chord lengths of 1–8 beats.
- **Key & mode:** 9 modes (the church modes plus harmonic and melodic minor), the mode's chords as triads or 7ths, Roman-numeral analysis, sharp/flat spelling.
- **Re-key / re-mode:** changing key or mode moves the whole progression by scale degree (e.g. G major ii–V–I becomes Aø7–Dm7–Gm7 in G minor), with undo/redo to compare.
- **Playback:** loop with play/pause/stop, tempo, 4/4 or 3/4, click, bass, three sounds (Keys, Pad, Organ), three rhythms (Held, Charleston, Quarters), smooth voice leading.
- **Arranging:** drag to reorder (mouse or touch), edit chords in place, duplicate, move, delete, transpose, undo/redo, copy as a text chord chart, save/load named progressions.
- **Drums:** 8 styles, presence sliders for kick, snare, hats, cymbals and toms, auto fills, swing, and an expandable 16-step sequencer with accents and ghost notes.

## Keyboard

`Space` play/pause · `Enter` add chord · `←` `→` select · `Shift`+`←` `→` move · `Del` remove · `Esc` deselect · `Ctrl/⌘+Z` undo

## Storage

Progressions and settings are saved in the browser's `localStorage`.

## Roadmap

- Package as a progressive web app (manifest, service worker, offline support).
