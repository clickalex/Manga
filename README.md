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
│       ├── chapter-32.md       ← Ch. 32 "Then Come In" (12-page panel script — **the flood session; the deep answers the answer**)
│       ├── chapter-33.md       ← Ch. 33 "The Second Register" (12-page panel script — **the horn gets a door; the realm coins “an ear”**)
│       ├── chapter-34.md       ← Ch. 34 "Carried, Not Kept" (12-page panel script — **the Shell’s first suit; four findings and a released ledger**)
│       ├── chapter-35.md       ← Ch. 35 "The Chorus Counts Itself" (12-page panel script — **the Re-Oath called; a shift and a voice defined apart**)
│       ├── chapter-36.md       ← Ch. 36 "Sung True" (12-page panel script — **the Re-Oath sung; two chords, and a no with its own note**)
│       ├── chapter-37.md       ← Ch. 37 "The First Song" (12-page panel script — **VOLUME 6 COMPLETE: the answer, the ring, and the year closed**)
│       ├── chapter-38.md       ← Ch. 38 "The First Signature" (12-page panel script — **VOLUME 7 OPENS: promises hang in the air, and the Nine are asked to sign**)
│       ├── chapter-39.md       ← Ch. 39 "What a Promise Is Worth" (12-page panel script — **the void was a vacancy; the realm kept its word; the Court cuts a word for it**)
│       ├── chapter-40.md       ← Ch. 40 "One Who Keeps" (12-page panel script — **the office is kept, not filled; the realm's first stone law, and a stool facing the door**)
│       ├── chapter-41.md       ← Ch. 41 "The Door in the Page" (12-page panel script — **the Re-Oath signed; the clause read through, and the door no hand can close**)
│       ├── chapter-42.md       ← Ch. 42 "The Second Book" (12-page panel script — **the realm's first book that promises nothing, a lesson taught in the rain, and two chips nobody can file**)
│       └── chapter-43.md       ← Ch. 43 "The Reader Who Paid in Advance" (12-page panel script — **the realm's first publication: a copy that declares itself, and a price of nothing**)
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
- **The manga** — **Season 1 is complete (Ch. 1–13) and Season 2 is running: Ch. 14–43 scripted (516 pages)**. The pilot (Ch. 1–6) ends with the King's first line, the grove's Re-Oath, and the Hollow's first word; the Sylvaris arc (Ch. 7–13) names the roads, gives the realm's word, and closes with *Every Name* — the realm's answer in nine names, the Chord through the tree, the Crown loosed into the tree's own crown, Vaelthorn's reserved line spent to Kaelen alone, and the scar that beats: Aurelion's. **Volume 4 — *The Mountain-Ask***: *Twelve Braids* takes the Nine eleven days east to a realm that counts a person's word in their own hair, a mine that sells the binding and files the breaking, and a mountain that has stopped answering; *The Contract Braid* moves the realm's court into the mine and puts a braid in the last Khazdûrin's beard; *The Street Question* walks fifty-eight doors for a dead man's face and finds a realm with no archive; *The Eve* closes the year by lamp, carries eight chairs down a mountain, and asks the realm the one question it has ever been allowed to ask — and the answer does not get said; *The Reading* reads four thousand and nine entries out loud in a mine until the realm says, for the first time in four hundred years, the one word its own law has always had; **the arc's payoff, *The Naming***, calls the witness — the stone answers in a language of shapes nobody can read, and a mortal, six old women's memories and one pencil turn it into nine hundred names, a year judged *answered*, and a hundred-year-old forge-fire brought home; and ***The Price*** deals with what all of that cost, re-cutting the realm's oath in fire — a word in a bar, a thumb pressed into hot iron, and a signature nobody can forge; and the **coda, *The Anvil's Warm***, pays the volume's held things — a century of shifts ending without ceremony, the flame-clan carrying fire into the cold forge and adopting the boy, a grummpling's padded pocket finally filled, and a realm deciding to keep **one line blank, by law, with a year on the waiting**; and **Volume 5 opens with *War-Song*** — the Barrens, a border that makes every traveller read their worst debt aloud, a realm with the best procedure in the world and no way to use it, and a clause drafted that will cost **skin** before it costs anything else; **Ch. 23** takes that clause into a labyrinth whose walls *are* the realm's code, where a champion takes it off her mouth and hands it back with two holes in it, and then east to the oldest maps in the world, where the whole crime turns out to have been **lawful**; and **Ch. 24** is the vote itself — nine stones, a clause with two holes and a witness who pays, a no said with the face up, the throat changing hands in front of the realm, and an amendment that makes a released debt come home to the realm: **one throat, carrying**; and **Ch. 25** is the duel and the choice — a walk-for-the-holding decided by the words two minotaurs name at the gate, a loser who inherits a *school*, a captain who hands her stone back and keeps her brother's oath **unfinished**, and the realm's answer to a crime committed by courtesy: **readers**, posted at every door, one of them walking east with the Nine; and **Ch. 26** takes the law out of the realm altogether — a reading-post on a caravan road, a realm that keeps its law in ink instead of skin, a document that declares what it is and isn't, an angel's unwitnessed oath entered at his own asking, and the first map symbol in nine realms drawn for a *law*; and **Ch. 27** takes the law into a foreign court and out of its own realm's hands — a crossing bought out by a deed, a fee paid in grain, a ruling entered in ink, and, at the end of the shelf road, the **Rift** and the camp at its edge that keeps hours of business; and **Ch. 28** brings the volume's antagonist back off the grey — a founder who concedes a complaint, pays restitution out of the purse that pays his own samplers, and tells a captain the truth about her brother and then declines to be forgiven — while an old man with a lamp and a stick walks three hundred miles to say eight words to the student he raised, and the realm leaves the edge of the world with **a clerk's desk, one reader, and a rule rewritten to fit it**; and **Ch. 29** closes the volume the way its realm decides things — a reader's office made as a **collar** with a buckle, a war renamed into a **reading-road**, a school's first four honest refusals filed on a wall, and the volume's clock taking its first **rest** — nine days north of a boat on a wagon; and **Ch. 30** opens Volume 6 at the **sea-gate**, where a door opens for a song and shuts for everything else, a chorus-parliament adjourns when the water says so, and the sea's oldest law — *nothing that is heard is lost* — is given words for the only time in the saga, so that the realm of the collar and the horn can say the one sentence none of the nine realms has ever said: **the sea answered**; and **Ch. 31** takes the report home — a post opening its first door, nine crossings in a week, a war-chief refused at his own post and filing praise, the school framing its first *yes*, and a realm entering **the first office it did not invent** while a well rises one finger during the reading; and **Ch. 32** takes them to the flood, where the sea invents an ear (**the flood session**, a tenth notch cut square), the deep answers the answer with the first song's **second line** — four words, half of them in a key the water does not have — and the realm answers a law of the sea with a habit, not a statute: **the flood reading**, at the top of every water, at nine posts, a school and a camp; and **Ch. 33** brings the sentence home to a realm of bindings, where a welcome cannot be cut into skin — so the Barrens cuts it **a door instead**, a second register on the outside of the debt-horn, kept only by being read aloud every day (*if it is not read, it is not kept*), answers the company’s exploit in a day (*the reading opens nothing*), and coins the word its code never had: **an ear** — a person who is read to; and **Ch. 34** puts the whole volume on trial in the sea's own courtroom, where the company's case is real, the charter says *carriage*, and the court rules four things — **carriage may be priced and the water may not · an answer is not property · *person* means a person · the ledger is released** — while a realm contracts eleven clerks, pays nothing for words, and a clerk who sold the sea's answers for three years pays nine feathers to read them at the water himself; and **Ch. 35** calls the sea's Re-Oath and counts the Chorus-True — **nine hundred and forty-one**, fifty-nine short, and the missing are on a company payroll — until a definition (*a shift is work, a voice is a person*), a stand-off paid in wages, fifty-nine fares bought by the singers themselves, and **one old woman's no** bring the count to a thousand, with **the first sea-law ever adopted from dry land** written into the reef-roll: *a voice present by refusal is present.* And **Ch. 36** sings the Re-Oath itself: the Tidesong Crown asks the realm its one sentence (*…give me your part*), Thalassa fails it twice because the sea's parts have been secrets for four hundred years, the no is given its own note (*sung first, sung with, never sung over*), and the realm's parts are given in public by a thousand voices — **the Oathflame Choir** and then **the Chorus-True** — while a crown that is only a witness does nothing at all; and **Ch. 37** closes the volume: the deep answers **in water and in pressure and never as a character** (a line of current going the wrong way, seawater in a listening tube, a flood an hour early and flat, a bowl on a shelf with four hands on its rim), the reef **grows its ring**, the sea's year of unboundness is **read out and filed closed** on both sides of the world, a company's contract is spent into the water like its answers were, twelve hundred tide-guard case their tridents and sing bar one, the law-court's last duet ends in the first verdict its judge has ever sung that is not a cage, and the volume's final page has nobody in it at all; and **Ch. 38** opens Volume 7 in **Emberfall**, where a spoken promise hangs in the air as legible text and a broken one **burns the name** off everything it stood on — where the Nine are asked for **a signature**, the Court overrules four thousand years of its own statute to admit **plural forms**, eight sign in eight grammars and one reserves her name *until it is hers again*, and seven hellhounds sit at the ash gate wearing collars whose text died with an oath, fed by a bath-house because the realm's law has no word for them; and **Ch. 39** ends the trial of oaths and corrects the realm's oldest error — the void-clause is a **test**, the realm has been keeping its promises for eight years without anybody watching (**4,206** of them, made on a name chiselled out of an archive field), the collar answers **word by word** to a crier reading the day's entries at a gate, and Emberfall cuts the word it never had into its dictionary: ***kept*** — *an oath nobody holds is still held if somebody keeps it.* And **Ch. 40** writes the realm's first new form in four thousand years: the Court discovers it has no form for filling an office because **a blank produces no text** in a realm that reads its law in the air; the First Contract's eighth office turns out to have been a form all along (*the eighth is not appointed; the eighth is kept*); the realm rules that it will not **fill** the office but **keep** it — *filled by: the clause; held by: whoever keeps it; field for a name: none; kept by: reading* — cuts the form into **stone**, moves the eighth chair's lamp from the man to the office, and seats the guilty archduke at a reader's stool facing the door; a cook's objection (*you are filing the office so that the realm does not have to forgive him*) is entered unauthored, unanswered and standing; and the trial's findings are read back **where they were kept** — 4,206 of 4,206, every keeper standing — while the collar climbs to ***one who keeps*** and a realm whose rule is that nothing is withheld from a reader hands a man with no realm a measured drawing of the fourth page. And **Ch. 41** signs the Re-Oath: the realm's largest promise performed **by signature** at the same gate where it tells strangers their oaths are cheap, the ninth field read first, the parties witnessing and not signing, the calling read at noon and still unanswered — and the realm's oldest clause read **through** a leaf that has been cut clean through since the founding day, because the realm has spent four thousand years reading a wall; the collar's sentence finishes in the hour of the signing, the last oath signs last, and the realm files the finding in the same case as the leaf, having paid for its own honesty one morning early. And **Ch. 42** is the first ordinary morning: a realm that goes back to work and discovers it has no form for a sentence nobody can act on — so it cuts a second book (*read, not filed*), invents the first law it has that is made of air, shelves the book beside its own foundation, walks that foundation out to a way-marker at dusk on published hours, and answers its first roadside forgery by teaching the whole road to look: *how to tell a hole from a door*, free, in the rain, while a carter's one-chip copy sits in his pocket and two chips nobody can account for are entered unfiled. Then **Ch. 43** gets its first **paid paper**: a strip bought at a crossing for two chips, a woman two days off the east road, and a realm that rules it will not honor the paper and will not refuse the woman — takes down none of its hours, polices no door, and answers a price it cannot reach by **publishing itself**: a copy that declares itself, cut by the thousand, marked with two strokes, given away at the gate and sent west with the cart, the crossings and the boats, with a price of nothing and a place in the queue for anybody who walks up.
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
