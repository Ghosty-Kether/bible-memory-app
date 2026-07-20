# Bible Memory

A single self-contained HTML app for memorizing Bible verses.

Open `index.html` in any browser — no install, no server, no internet connection required after the initial download.

## Features

- The complete World English Bible (WEB) — 66 books, 1189 chapters, all 31,000+ verses — embedded directly in the file. WEB is a modern, public-domain translation, so the full text can be freely bundled and distributed.
- Browse by book, chapter, and verse.
- **Practice mode**: each word of a verse is masked. Type its first letter and the word fills itself in, revealing the verse one word at a time until you've typed the whole thing from memory.
- Tracks which verses you've memorized, with per-book and overall progress stats.
- Progress is saved automatically in your browser (`localStorage`) and persists between sessions.
- **Export / Import progress**: download your progress as a JSON file at any time, and load it back in later — useful as a backup, for moving between devices, or if your browser blocks local storage for files opened directly (`file://`).

## Usage

1. Download `index.html` (or clone this repo).
2. Open it in your browser by double-clicking, or via `File > Open`.
3. Pick a book, chapter, and verse from the dropdowns to read it.
4. Click **Practice this verse** to start the memorization exercise.
5. Check the **Progress** tab any time to see your stats, export a backup, or reset.

### Hosting it online (optional)

Since this is a single static HTML file, you can also enable **GitHub Pages** for this repo (Settings → Pages → deploy from the `main` branch) to get a shareable link, instead of only opening it locally.

## License

- App code: MIT — do whatever you like with it.
- Bible text: [World English Bible](https://worldenglish.bible/), public domain.
