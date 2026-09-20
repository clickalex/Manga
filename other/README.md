# Other — Assets & Deployment

> The repo's catch-all for *non-story* files: generated artwork, build/deploy notes, and anything that serves the site but isn't canon. Story canon lives in [../story/](../story/README.md); design specs in [../character/](../character/README.md) and [../location/](../location/README.md).

## Files here

| Path | What it is |
|---|---|
| [assets/cover-vol1.png](assets/cover-vol1.png) | **Volume 1 cover — v2** (AI-generated, no text — the reader adds the title in lettering): the rift, the nine-spired crown-citadel with one lantern per color, and Kaelen in his father's too-big work coat with an ordinary smith's hammer. **The chest is canon:** a small, faint gray-green mark with its first white thread and *no glow* — per [../character/mosaic-nine.md](../character/mosaic-nine.md) (“no eye-glow, no power aura; the power is the scar and the white threads, both small”) and Ch. 1 P2.2 (“a faint scar … like a smudge of un-ink”). Used by the index page's Home tab. |
| [assets/cover-vol1-v1-glow.png](assets/cover-vol1-v1-glow.png) | **v1 (superseded, kept for reference)** — stronger composition-identical art, but its chest scar was drawn as a full nine-color radial mandala with a power aura: an early misread of the Mosaic (the nine colors belong to the *scarf* and the *record*; on Kaelen’s skin the scar is one small mark and the **white threads** are the cost). Do not use for print or web. |
| [assets/cover-vol1-web.jpg](assets/cover-vol1-web.jpg) | **Web copy of the cover** (same 848×1264 image as the v2 master, JPEG q86, ~250 KB vs the 2.5 MB PNG) — this is what `index.html` shows on the Home tab. Regenerate from the PNG with `convert cover-vol1.png -strip -quality 86 cover-vol1-web.jpg`; keep the PNG as the master, and keep `index.html`’s hardcoded `width`/`height` in sync with the master’s pixel size. |

## Deploying to GitHub Pages (the index page)

The site is a **single index page** at the repo root: [`index.html`](../index.html). It fetches the `.md` files from this repo and renders them in the browser (marked.js from CDN) — so **the repo *is* the site**; no build step, no server code.

**Steps (one-time, ~2 minutes):**

1. Make sure the work is on **`main`** (merge the open PR into `main`).
2. On GitHub, open the repo → **Settings → Pages**.
3. Under **Build and deployment → Source**: choose **Deploy from a branch**.
4. Branch: **`main`**, folder: **`/ (root)`** → **Save**.
5. Wait ~1 minute. The site is live at **`https://clickalex.github.io/Manga/`**.

**After that:** every push to `main` re-deploys automatically. New chapters = drop a new `.md` in `story/manga/` and add one line to the chapter list in `index.html` (search for `MANGA_CHAPTERS`).

## Local preview (before pushing)

```bash
cd Manga
python3 -m http.server 8000
# open http://localhost:8000
```

(The index page uses `fetch()`, so it must be served over HTTP — opening `index.html` straight from disk won't load the markdown.)

## House rules for this folder

- **Artwork goes in `other/assets/`**, named `<thing>-<v<version> or vol<volume>>.png` (e.g. `cover-vol1.png`, `art-aelion-vaelthorn-v2.png`). **Superseded artwork stays in the folder with `-v<n>-<why>` in the name** (e.g. `cover-vol1-v1-glow.png`) — never overwrite or delete a master; the current one always carries the plain `<thing>-vol<n>` name.
- **Cover art obeys the design canon.** The Mosaic Nine’s sheets in [../character/mosaic-nine.md](../character/mosaic-nine.md) are canonical: no eye-glow, no aura, no nine-color bloom on anyone’s skin. A cover that breaks them gets re-rendered, not shipped — that is exactly why `-v1-glow` exists.
- **Generated/derived files never go in `story/`** — story/ is canon markdown only.
- If a file becomes canon (a design sheet, a location map used as a story reference), *move it* to `character/`, `location/`, or `story/` and update the READMEs — `other/` is for things that serve the site, not the story.
