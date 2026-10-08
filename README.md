# Montreal Lions

Final approved version 3. Use this folder as the Git repository root and static deployment directory. No build or installation step is required.

- `index.html`: complete bilingual website, styles and interactions.
- `img/`: the original logo and unmodified copies of photos from `../_ai_context/images/`, used by the page.
- `image-sources.json`: original source paths for every photo used on the site.
- `gallery-sources.json`: original source paths for the gallery photos.

Open `index.html` in a browser, or run `python -m http.server 8000` here for a local preview. Google Fonts uses the internet, with fallback fonts available.

Scroll-driven motion is built in with a small dependency-free script at the end of `index.html` (no external libraries):

- Hero: giant outlined words slide behind the crest as you scroll and the team photo settles.
- Honours: the 6–0 record counts up like a scoreboard; the trophy photo zooms out.
- Schedule: a red route line draws down the season; each event stamps in.
- Roster ("The lineup."): on wide screens the section pins and shows one Lion at a time; signature tips open over the photo.
- Owner: the photo assembles from particles.
- Gallery: on wide screens it becomes a horizontal film strip with parallax.
- Everywhere: heading wipes, red curtain photo reveals, a gold scroll-progress line, film grain, and a hover tilt on mouse devices.

Headlines in the loud moments use the Anton display font (Google Fonts). With reduced motion, or if the script fails, the page falls back to the plain static layout, and phones get a simpler version without pinned sections.

The logo welcome plays on every page load or reload, including direct section links, and respects reduced-motion settings. Escape or the Enter button skips the introduction. Language preference is saved locally.

Only photos supplied in `../_ai_context/images/` are used. Deployment copies are kept in `img/`, so the site works when deployed independently. Source paths are relative to this folder. The original standalone logo is retained. Team photos replace unavailable portraits and the trophy photo.
