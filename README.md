# LexiQuest — Business French → English

A mobile-first exam trainer built from vocabulary selected from four Business French course PDFs (sections 1.1–1.4). Includes 200 French vocabulary entries, 44 collocations, exam-style synonym/antonym/derivative/fill-in/acronym/translation modes, XP, error review, local progress, and offline PWA caching. Translations are curated English glosses, not an official translation of the source glossaries. This starter version does **not** yet contain every item from the original PDFs, and some synonym/antonym questions include complementary common vocabulary beyond the uploaded documents.

## Deploy on GitHub Pages
1. Create a public GitHub repository, e.g. `lexiquest`.
2. Upload the **contents** of this folder to the repository root (not the containing folder).
3. Open repository Settings → Pages → Build and deployment → Deploy from a branch → `main` / `(root)` → Save.
4. Visit `https://YOUR-USERNAME.github.io/lexiquest/` after GitHub Pages publishes.
5. On iPhone, open in Safari → Share → Add to Home Screen. On Android, open in Chrome → menu → Add to Home screen / Install app.

## Notes
The website must be served over HTTP(S), not opened via file://, because question files use fetch(). To test locally: `python -m http.server 8000` in this folder, then open `http://localhost:8000`.
The progress is stored per browser/device in localStorage; no account or cross-device sync. No ads, tracking, or backend. Accents are ignored when checking; an answer must otherwise match a listed acceptable phrase. Some valid alternative translations may not be automatically recognized. Course-specific precise answer variants should be added to JSON over time.
