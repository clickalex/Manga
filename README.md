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
│       ├── chapter-17.md       ← Ch. 17 "The Eve" (12-page panel script — Vol. 4 continues)
│       ├── chapter-18.md       ← Ch. 18 "The Reading" (12-page panel script — Vol. 4 continues)
│       ├── chapter-19.md       ← Ch. 19 "The Naming" (12-page panel script — the arc's payoff)
│       ├── chapter-20.md       ← Ch. 20 "The Price" (12-page panel script — the law re-cut in fire)
│       ├── chapter-21.md       ← Ch. 21 "The Anvil's Warm" (12-page panel script — the Volume 4 coda)
│       ├── chapter-22.md       ← Ch. 22 "War-Song" (12-page panel script — Vol. 5 opens / the Barrens)
│       ├── chapter-23.md       ← Ch. 23 "The Record of Losses" (12-page panel script — the maze, the maps)
│       ├── chapter-24.md       ← Ch. 24 "One Throat" (12-page panel script — the vote)
│       ├── chapter-25.md       ← Ch. 25 "The Walk for the Holding" (12-page panel script — the choice)
│       ├── chapter-26.md       ← Ch. 26 "The Road East" (12-page panel script — the law meets paper)
│       ├── chapter-27.md       ← Ch. 27 "The Shelf Road" (12-page panel script — the fee, the court, the Rift)
│       ├── chapter-28.md       ← Ch. 28 "The Founder" (12-page panel script — the table, the teacher, the reading-post)
│       ├── chapter-29.md       ← Ch. 29 "Four Beats and a Rest" (12-page panel script — the coda; the volume closes)
│       ├── chapter-30.md       ← Ch. 30 "The First Line" (12-page panel script — Volume 6 opens at the sea-gate)
│       ├── chapter-31.md       ← Ch. 31 "Nine Posts" (12-page panel script — **the realm enters a foreign office; the first door opens**)
│       └── chapter-32.md       ← Ch. 32 "Then Come In" (12-page panel script — **the flood session; the deep answers the answer**)
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
- **The manga** — **Season 1 is complete (Ch. 1–13) and Season 2 is running: Ch. 14–32 scripted (384 pages)**. The pilot (Ch. 1–6) ends with the King's first line, the grove's Re-Oath, and the Hollow's first word; the Sylvaris arc (Ch. 7–13) names the roads, gives the realm's word, and closes with *Every Name* — the realm's answer in nine names, the Chord through the tree, the Crown loosed into the tree's own crown, Vaelthorn's reserved line spent to Kaelen alone, and the scar that beats: Aurelion's. **Volume 4 — *The Mountain-Ask***: *Twelve Braids* takes the Nine eleven days east to a realm that counts a person's word in their own hair, a mine that sells the binding and files the breaking, and a mountain that has stopped answering; *The Contract Braid* moves the realm's court into the mine and puts a braid in the last Khazdûrin's beard; *The Street Question* walks fifty-eight doors for a dead man's face and finds a realm with no archive; *The Eve* closes the year by lamp, carries eight chairs down a mountain, and asks the realm the one question it has ever been allowed to ask — and the answer does not get said; *The Reading* reads four thousand and nine entries out loud in a mine until the realm says, for the first time in four hundred years, the one word its own law has always had; **the arc's payoff, *The Naming***, calls the witness — the stone answers in a language of shapes nobody can read, and a mortal, six old women's memories and one pencil turn it into nine hundred names, a year judged *answered*, and a hundred-year-old forge-fire brought home; and ***The Price*** deals with what all of that cost, re-cutting the realm's oath in fire — a word in a bar, a thumb pressed into hot iron, and a signature nobody can forge; and the **coda, *The Anvil's Warm***, pays the volume's held things — a century of shifts ending without ceremony, the flame-clan carrying fire into the cold forge and adopting the boy, a grummpling's padded pocket finally filled, and a realm deciding to keep **one line blank, by law, with a year on the waiting**; and **Volume 5 opens with *War-Song*** — the Barrens, a border that makes every traveller read their worst debt aloud, a realm with the best procedure in the world and no way to use it, and a clause drafted that will cost **skin** before it costs anything else; **Ch. 23** takes that clause into a labyrinth whose walls *are* the realm's code, where a champion takes it off her mouth and hands it back with two holes in it, and then east to the oldest maps in the world, where the whole crime turns out to have been **lawful**; and **Ch. 24** is the vote itself — nine stones, a clause with two holes and a witness who pays, a no said with the face up, the throat changing hands in front of the realm, and an amendment that makes a released debt come home to the realm: **one throat, carrying**; and **Ch. 25** is the duel and the choice — a walk-for-the-holding decided by the words two minotaurs name at the gate, a loser who inherits a *school*, a captain who hands her stone back and keeps her brother's oath **unfinished**, and the realm's answer to a crime committed by courtesy: **readers**, posted at every door, one of them walking east with the Nine; and **Ch. 26** takes the law out of the realm altogether — a reading-post on a caravan road, a realm that keeps its law in ink instead of skin, a document that declares what it is and isn't, an angel's unwitnessed oath entered at his own asking, and the first map symbol in nine realms drawn for a *law*; and **Ch. 27** takes the law into a foreign court and out of its own realm's hands — a crossing bought out by a deed, a fee paid in grain, a ruling entered in ink, and, at the end of the shelf road, the **Rift** and the camp at its edge that keeps hours of business; and **Ch. 28** brings the volume's antagonist back off the grey — a founder who concedes a complaint, pays restitution out of the purse that pays his own samplers, and tells a captain the truth about her brother and then declines to be forgiven — while an old man with a lamp and a stick walks three hundred miles to say eight words to the student he raised, and the realm leaves the edge of the world with **a clerk's desk, one reader, and a rule rewritten to fit it**; and **Ch. 29** closes the volume the way its realm decides things — a reader's office made as a **collar** with a buckle, a war renamed into a **reading-road**, a school's first four honest refusals filed on a wall, and the volume's clock taking its first **rest** — nine days north of a boat on a wagon; and **Ch. 30** opens Volume 6 at the **sea-gate**, where a door opens for a song and shuts for everything else, a chorus-parliament adjourns when the water says so, and the sea's oldest law — *nothing that is heard is lost* — is given words for the only time in the saga, so that the realm of the collar and the horn can say the one sentence none of the nine realms has ever said: **the sea answered**; and **Ch. 31** takes the report home — a post opening its first door, nine crossings in a week, a war-chief refused at his own post and filing praise, the school framing its first *yes*, and a realm entering **the first office it did not invent** while a well rises one finger during the reading; and **Ch. 32** takes them to the flood, where the sea invents an ear (**the flood session**, a tenth notch cut square), the deep answers the answer with the first song's **second line** — four words, half of them in a key the water does not have — and the realm answers a law of the sea with a habit, not a statute: **the flood reading**, at the top of every water, at nine posts, a school and a camp.
- **The future scope** — the canon spine (the 8 fixed facts), a 12-volume manga roadmap, 4 anime seasons, movies, a TCG whose *system is the game*, four PC games, novels & audio, a 10-year IP timeline, and the sequel door (Realm 10 — the stars).

---

## Quick facts

| | |
|---|---|
| Working title | **AURELION: The Nine Realms Saga** |
| Realms / races | 9 (+ 1 reserved) / 49 (+ 9 reserved slots) |
| Named characters | **628** (9 + 96 + 283 + 240) |
| Pilot status | **Ch. 1–6 scripted — pilot complete** · **Ch. 7–13 scripted — Season 1 complete** (Vol. 3 closes on Ch. 13, *Every Name*) · **Ch. 14–21 scripted — Vol. 4 complete** · **Vol. 5, *The One Throat* (Ch. 22–29) is COMPLETE; *Vol. 6, The First Song* (from Ch. 30) is running** (Season 2) |
| IP rule #1 | **No race is the monster.** The monster is the hunger. |
