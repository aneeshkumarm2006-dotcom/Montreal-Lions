# Montreal Lions

Final approved version 3. Use this folder as the Git repository root and static deployment directory. No build or installation step is required.

- `index.html`: complete bilingual website, styles and interactions.
- `img/`: unmodified copies of photos from `../_ai_context/images/`, used by the page.
- `image-sources.json`: original source paths for every photo used on the site.
- `gallery-sources.json`: original source paths for the gallery photos.

Open `index.html` in a browser, or run `python -m http.server 8000` here for a local preview. Google Fonts uses the internet, with fallback fonts available.

The text-wordmark welcome plays once per tab session, skips direct section links, and respects reduced-motion settings. Escape or the Enter button skips the introduction. Language preference is saved locally.

Only photos supplied in `../_ai_context/images/` are used. Deployment copies are kept in `img/`, so the site works when deployed independently. Source paths are relative to this folder. Text branding replaces the previous standalone logo, and team photos replace unavailable portraits and the trophy photo.
