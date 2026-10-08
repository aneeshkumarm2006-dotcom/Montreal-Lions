# Montreal Lions

Final approved version 3. Use this folder as the Git repository root and static deployment directory. No build or installation step is required.

- `index.html`: complete bilingual website, styles and interactions.
- `img/`: only the images used by the page.
- `gallery-sources.json`: original source paths for the optimized gallery photos.

Open `index.html` in a browser, or run `python -m http.server 8000` here for a local preview. Google Fonts uses the internet, with fallback fonts available.

The logo welcome plays once per tab session, skips direct section links, and respects reduced-motion settings. Escape or the Enter button skips the introduction. Language preference is saved locally.

Original photographs remain in `../_ai_context/images/` and are not needed for deployment. Gallery source paths are relative to this folder.
