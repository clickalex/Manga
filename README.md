# AURELION — The Nine Realms Saga

**An original multi-race fantasy IP — one world, nine realms, 49 races, 628 named characters — built from day one for manga, anime, movies, card games, and PC games.**

Theme: **unity without erasure.** No race is the monster.

> 📖 **Read the project on the web:** this repo is the site. Once deployed to GitHub Pages, open **`https://clickalex.github.io/Manga/`** — one index page for the manga, the story bible, the characters, the locations, and the future scope. (Setup below; or preview locally with `python3 -m http.server`.)

---

## Repository structure

```
Manga/
├── index.html                  ← THE INDEX PAGE (deployable on GitHub Pages — single file, no build step)
├── README.md                   ← this file
│
├── story/                      ← CANON (the story side)
│   ├── README.md               ← IP index: logline, franchise math, file index, status
│   ├── 01-the-story.md         ← the great story (premise, history, 3-act saga, arcs, ending, sequel hook)
│   ├── 02-races-and-realms.md  ← 49 races + 9 reserved Realm-10 slots; realm profiles
│   ├── 03-characters.md        ← cast book index (628 total) + Tier 1 (9) + Tier 2 (29) + villains
│   ├── 03a-principals.md       ← Tier 2 new principals (67)
│   ├── 03b-ensemble.md         ← Tier 3 named ensemble (283)
│   ├── 03c-roster.md           ← Tier 4 named population (240)
│   ├── 04-power-system.md      ← Sigils / Chords / the Unraveling / Nine Crowns (card-game ready)
│   ├── 05-future-scope.md      ← the canon spine + full franchise roadmap (anime/manga/movies/TCG/PC/10-yr)
│   └── manga/                  ← THE MANGA (main series)
│       ├── README.md           ← reading order + pilot canon quick-reference + writing rules
│       ├── chapter-01.md       ← Ch. 1 "The Bell in the Rain" (12-page panel script)
│       ├── chapter-02.md       ← Ch. 2 "The Name of the Scar" (12-page panel script)
│       ├── chapter-03.md       ← Ch. 3 "One Table" (12-page panel script)
│       ├── chapter-04.md       ← Ch. 4 "The Withered Court" (12-page panel script)
│       ├── chapter-05.md       ← Ch. 5 "The Name of the King" (12-page panel script)
│       ├── chapter-06.md       ← Ch. 6 "The First Crown" (12-page panel script — end of pilot)
│       ├── chapter-07.md       ← Ch. 7 "The Name of the Road" (12-page panel script — S1 continues)
│       ├── chapter-08.md       ← Ch. 8 "Open Doors" (12-page panel script — S1 continues)
│       ├── chapter-09.md       ← Ch. 9 "The Realm's Word" (12-page panel script — S1 continues)
│       ├── chapter-10.md       ← Ch. 10 "The Unnamed Road" (12-page panel script — S1 continues)
│       ├── chapter-11.md       ← Ch. 11 "The Held Door" (12-page panel script — S1 continues)
│       ├── chapter-12.md       ← Ch. 12 "Every Branch" (12-page panel script — S1, the call)
│       ├── chapter-13.md       ← Ch. 13 "Every Name" (12-page panel script — **Season 1 finale / end of Vol. 3**)
│       ├── chapter-14.md       ← Ch. 14 "Twelve Braids" (12-page panel script — **Season 2 opens / Vol. 4 "The Mountain-Ask"**)
│       ├── chapter-15.md       ← Ch. 15 "The Contract Braid" (12-page panel script — Vol. 4 continues)
│       ├── chapter-16.md       ← Ch. 16 "The Street Question" (12-page panel script — Vol. 4 continues)
│       └── chapter-17.md       ← Ch. 17 "The Eve" (12-page panel script — Vol. 4 continues)
│
├── character/                  ← DESIGN (the character side)
│   ├── README.md               ← cast system + tier audit + rules for new characters
│   └── mosaic-nine.md          ← the nine leads' design sheets (look, hex palettes, motifs, pilot lines)
│
├── location/                   ← WORLD (the location side)
│   ├── README.md
│   ├── ashenmere.md            ← the pilot town: map, design guide, the Festival of Open Doors
│   └── nine-realms.md          ← the nine realms: location guide + geography rule + Realm 10 (reserved)
│
└── other/                      ← SITE (the deployment side)
    ├── README.md               ← deploy guide (GitHub Pages steps) + house rules
    └── assets/
        ├── cover-vol1.png      ← Volume 1 cover, v2 (AI concept, no text; scar canon)
        ├── cover-vol1-v1-glow.png ← superseded v1 (nine-color chest glow — kept for reference only)
        └── cover-vol1-web.jpg  ← web copy used by index.html (JPEG q86, ~250 KB)
```

**The four-folder rule:** canon goes in `story/`, character design in `character/`, world/location docs in `location/`, site assets & deploy notes in `other/`. No loose files at the root except `index.html` and this README.

---

## Deploying the index page (GitHub Pages)

The index page is a **single self-contained file** (`index.html`). It fetches the markdown files from the repo and renders them in the browser (marked.js via CDN) — **no build step, no server code; the repo is the site.**

1. **Merge this branch into `main`** (the PR is open: `clickalex/Manga#1`).
2. GitHub → repo → **Settings → Pages** → *Build and deployment → Source*: **Deploy from a branch** → branch **`main`**, folder **`/ (root)`** → Save.
3. ~1 minute later the site is live at **`https://clickalex.github.io/Manga/`**. Every later push to `main` re-deploys automatically.

**Adding a chapter later:** drop `story/manga/chapter-10.md` (etc.) in the repo and add one entry to the `MANGA_CHAPTERS` list near the top of `index.html`'s script. That's all the site needs to know.

**Local preview** (before pushing):

```bash
cd Manga
python3 -m http.server 8000
# → http://localhost:8000
```

(the page uses `fetch()`, so it must be served over HTTP, not opened from disk)

---

## What's in the project (one paragraph each)

- **The story** — Aurelion, the First Dreaming, shattered itself into nine realms; its negative image (Vaelthorn, the Hollow Sovereign) hungers to reforge every race into one painless unity. A scarred human boy — a Mosaic, a fragment of the First Being — walks the seams with one warrior of every realm, answering the Unraveling the only way it can be answered: **by saying names back**.
- **The cast** — 628 named characters in four tiers (9 core · 96 principals · 283 ensemble · 240 population), each lead the emotional face of a realm & race, so any medium can re-center on a different lead and the world holds.
- **The power system** — Sigils (realm soul-marks that spend *identity*, not mana), Chords (two sigils of different realms, by *choice* — the card game's combo system, the theme as a mechanic), the Unraveling (the cost that is the story), and the Nine Crowns (artifacts of consent).
- **The manga** — **Season 1 is complete (Ch. 1–13) and Season 2 is running: Ch. 14–17 scripted (204 pages)**. The pilot (Ch. 1–6) ends with the King's first line, the grove's Re-Oath, and the Hollow's first word; the Sylvaris arc (Ch. 7–13) names the roads, gives the realm's word, and closes with *Every Name* — the realm's answer in nine names, the Chord through the tree, the Crown loosed into the tree's own crown, Vaelthorn's reserved line spent to Kaelen alone, and the scar that beats: Aurelion's. **Volume 4 — *The Mountain-Ask***: *Twelve Braids* takes the Nine eleven days east to a realm that counts a person's word in their own hair, a mine that sells the binding and files the breaking, and a mountain that has stopped answering; *The Contract Braid* moves the realm's court into the mine and puts a braid in the last Khazdûrin's beard; *The Street Question* walks fifty-eight doors for a dead man's face and finds a realm with no archive; and *The Eve* closes the year by lamp, carries eight chairs down a mountain, and asks the realm the one question it has ever been allowed to ask — and the answer does not get said.
- **The future scope** — the canon spine (the 8 fixed facts), a 12-volume manga roadmap, 4 anime seasons, movies, a TCG whose *system is the game*, four PC games, novels & audio, a 10-year IP timeline, and the sequel door (Realm 10 — the stars).

---

## Quick facts

| | |
|---|---|
| Working title | **AURELION: The Nine Realms Saga** |
| Realms / races | 9 (+ 1 reserved) / 49 (+ 9 reserved slots) |
| Named characters | **628** (9 + 96 + 283 + 240) |
| Pilot status | **Ch. 1–6 scripted — pilot complete** · **Ch. 7–13 scripted — Season 1 complete** (Vol. 3 closes on Ch. 13, *Every Name*) · **Ch. 14–17 scripted — Season 2 running** (Vol. 4, *The Mountain-Ask*) |
| IP rule #1 | **No race is the monster.** The monster is the hunger. |
