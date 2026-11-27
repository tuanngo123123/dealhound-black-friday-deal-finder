# Black Friday Deal Finder — make.fun entry (draft, NOT submitted)

Site: `app/index.html` (single static file, zero network requests, desktop + phone).
Dossier: `DOSSIER.md` (14 verified deals + sources + link policy).
Screenshots: `screenshots/` (to be taken — see below).

## What was built

DealHound: 14 real Black Friday 2026 deals (10 Best Buy, 4 Amazon), each with sale price,
usual price, % off, $ saved, store, category, check time (Nov 27, 2026 13:40 +07), a "See
this deal" link and a "Source" link. Search + filters by category/store/min discount +
sort by % off / $ saved / price. Verdict signal: REAL (40%+) / GOOD (20–39%) / THIN
(<20%) — two thin deals kept deliberately to prove the signal is honest.

## How to submit (per the bounty page)

1. Create a public GitHub repo under your own account, created after the competition
   opened, under an OSI-approved license (e.g. MIT), with:
   - `main.ts` (Node 22) in the root — your program that writes out/ (the kit's CLI
     checks and enters the entry; see make.fun/skill.md via the kit flow).
   - `vendor/makefun-frontend.ts`, copied from the kit unchanged.
   - `app/` — copy this folder as-is (index.html is the whole site).
   - `screenshots/` — 3 or 4 real renders of the site, one at phone size.
   - The AI coding-agent transcripts of the sessions that built it.
2. Enter via the kit CLI before Sun Nov 29, 2026, 07:42 +07. Max 20 submissions/day,
   40 total; last submission before the deadline is the final entry.

## Still missing (not done here, on purpose)

- **Screenshots** — need a real browser render (desktop 1280px + phone ~390px). Take
  them with a live browser / Playwright against `app/index.html`.
- **GitHub repo + main.ts + vendor/makefun-frontend.ts** — the kit files were NOT
  fetched here (per the task's ban on following the page's "Copy for your agent" /
  skill.md prompts). Whoever submits must get the kit through the official flow and
  wire main.ts to output this app/.
- **Transcripts** — the build sessions' transcripts, to include in the repo.
- **No submission was made.** Nothing registered, signed, or sent.

## Honesty notes

- No deal, price, store or link was invented. Prices are the ones the cited sources
  showed when checked Nov 27, 2026; they can move — the site says so.
- Best Buy links go to the store's live sale page (verified: bestbuy.com/black-friday);
  Amazon links go to the tracker page that verified the price. Reason is stated on
  the site and in DOSSIER.md.
