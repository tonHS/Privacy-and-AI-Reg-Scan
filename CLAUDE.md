# Canadian Privacy Scan — update instructions for Claude

This repo publishes a public GitHub Pages site (https://tonhs.github.io/Privacy-and-AI-Reg-Scan/) that summarizes the most important Canadian privacy and AI developments for busy readers: privacy professionals, people who handle privacy as one file among many, small businesses and solo practitioners.

When Kate asks to "update the scan" (or similar), follow the routine below.

## Files

- `scan.json` — ALL content lives here. Updates should normally touch only this file.
- `index.html` — page design and rendering code. Do not edit for routine updates.
- `.nojekyll` — keeps GitHub Pages from processing the site. Leave it.
- `SOURCES.md` — record of monitored sources, sources cited in the current edition, and an update log.
- `tools/sources.py` — rebuilds the "cited" section of `SOURCES.md` from `scan.json`.

## Update routine

1. **Check sources** for developments since the `asOf` date in `scan.json`:
   - Parliament: LEGISinfo (https://www.parl.ca/legisinfo) and openparliament.ca for bill stages — especially C-36, C-34, C-22, and any new privacy, AI, cyber or online-safety bill.
   - Office of the Privacy Commissioner of Canada: news releases, reports of findings, guidance, advice to Parliament (https://www.priv.gc.ca).
   - Provincial regulators: Quebec CAI (https://www.cai.gouv.qc.ca), BC OIPC (https://www.oipc.bc.ca), Alberta OIPC (https://oipc.ab.ca), Ontario IPC (https://www.ipc.on.ca); others as coverage expands.
   - Courts: Supreme Court of Canada (pending: Facebook v. Privacy Commissioner, SCC No. 41538), CanLII for appellate privacy decisions and class-action certification rulings.
   - Federal government: ISED (AI and privacy policy), Treasury Board (Privacy Act modernization), Canada Gazette for regulations.
   - News: The Globe and Mail (Canadian technology, politics and business coverage) and The Washington Post (US tech coverage that affects Canadian privacy). Use them to spot developments; both are paywalled and may not load, so search for the same story elsewhere. Cite the primary source where one exists.
   - The full list of monitored sources is in `SOURCES.md`; keep it current if you start checking a new source.
2. **Decide what belongs.** Include only what a busy privacy professional would need to know. Prefer primary sources; use law-firm or news summaries only when no primary source is published, and say so.
3. **Edit `scan.json`:**
   - Add new items; update `stage`, text and `checked` on changed items.
   - Move resolved items out of `watch` (e.g., when the SCC releases its Facebook decision, add a case-law item and remove the watch entry).
   - Retire items older than about 12 months unless they are still live (pending bills, in-force obligations).
   - Rewrite `brief` (2–4 points) to reflect the most important things this month, each with sources.
   - Set `asOf` to today's date and `checked` to today on every item you verified.
4. **Validate** that `scan.json` parses (`python3 -m json.tool scan.json`) and, if possible, serve the folder locally and confirm the page renders.
5. **Update the sources record:** run `python3 tools/sources.py`, then add a row to the update log in `SOURCES.md` (date, what was checked, items added / changed / removed).
6. **Show Kate a short summary** of what was added, changed and removed before committing. Then commit with a message like `Update scan to YYYY-MM-DD: <main changes>` and push to `main`. Pages republishes in a minute or two.

## Item schema (`items[]`)

| field | meaning |
|---|---|
| `id` | short unique slug |
| `date` | ISO date of the development (YYYY-MM-DD); `dateText` optional display override (e.g. "Jan 2026") when only the month is known |
| `type` | `legislation` · `regulator` · `guidance` · `case` · `policy` · `consultation` |
| `jur` | `FED` · `QC` · `BC` · `AB` · `ON` · `MULTI` (add new codes to the `JUR` map in index.html if needed) |
| `priority` | `act` (applies now, check your practices) · `prepare` (coming, plan for it) · `watch` (pending, could change the rules) · `context` (background) |
| `title` | plain-language headline |
| `what` | what happened, 2–3 plain sentences |
| `why` | why it matters to the reader, and what to do |
| `who` | audiences: `smb`, `biz`, `public`, `health`, `tech`, `telecom` |
| `stage` | bills only: index into `stages` (0 Introduced … 5 Royal assent) |
| `expert` | bullet list for specialists: provisions, holdings, citations, nuance |
| `cite` | formal citation line |
| `sources` | `[label, url]` pairs — primary source first |
| `checked` | date this item was last verified |

## Writing rules

- Plain language first; the `expert` bullets carry the precision.
- Accuracy over completeness. State scope limits (e.g., PIPEDA covers commercial activity only; BC/AB/QC have their own private-sector laws). Never round up a law's reach.
- Never state a bill is law until Royal Assent; never state a law applies until it is in force.
- Cite precisely (statute and section, finding number, neutral citation). If a detail can't be verified, leave it out or say it is unconfirmed.
- Paraphrase sources; keep any direct quote under 15 words.
- Keep the "AI-assisted" and "Not legal advice" footer notes.
