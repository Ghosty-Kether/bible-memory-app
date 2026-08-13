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


## Windows .exe (built automatically)

This repo has a GitHub Actions workflow that builds a Windows installer on every push
to `main` — no need to install Node.js or run any commands yourself:

1. Go to the **Actions** tab on GitHub.
2. Open the latest **Build Windows App** run (or click **Run workflow** to trigger one manually).
3. Once it finishes (a few minutes), open it and download the **Bible-Memory-Windows**
   artifact from the bottom of the page — it contains the installer `.exe`.

Since the app isn't code-signed, Windows SmartScreen may warn it's from an unknown
publisher the first time you run the installer — click "More info" → "Run anyway".


## Android app (built automatically)

Like the Windows build, there's a GitHub Actions workflow that builds an installable
Android APK on every push to `main` — no Android Studio or SDK needed on your end:

1. Go to the **Actions** tab on GitHub.
2. Open the latest **Build Android App** run (or click **Run workflow** to trigger one manually).
3. Once it finishes, download the **Bible-Memory-Android** artifact — it contains
   `app-debug.apk`.
4. Copy the APK to your phone and open it to install. You'll need to allow "install
   from unknown sources" for whichever app you use to open it (Files, Chrome, etc.) —
   Android will prompt you for this the first time.

This is a debug-signed build, meant for installing on your own device. Publishing to the
Play Store would need a proper release signing key, which is a separate step if you ever want it.
