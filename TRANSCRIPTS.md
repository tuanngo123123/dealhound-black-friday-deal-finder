# Transcripts — what the submitter still has to do (NOT done in this prep)

This repo was prepared for submission to make.fun bounty
`black-friday-deal-finder-01` (DealHound). No entry was submitted from here.

## What submission needs (per kit RULES.txt, "Enter" step 3)

Every entry must upload the transcripts (session logs) of the AI coding-agent
sessions that built it, as a bundle made by the kit CLI:

  node <kit>/cli/makefun.mjs bundle --repo <this repo> --system-prompt <file> \
    --effort <level> --out transcripts.tar.gz --redact "<personal details>"

Then run the pre-submit check:

  node <kit>/cli/makefun.mjs check --kit <kit> --repo <this repo> \
    --transcripts transcripts.tar.gz

## Sessions that built this entry (upload all of them, whole)

1. The session that built `app/index.html` (DealHound site, 14 verified deals)
   — the build subagent's session, started after the competition opened
   (2026-11-27T00:42:00Z).
2. This packaging session (repo-ready assembly, screenshot retake, build run).

## Known transcript-gate notes

- `thinking_fresh`: this entry was NOT built from a repo created by the kit's
  `init` (no `makefun anchor ...` line was printed before building), so for a
  source-bundle entry this check skips as a note, not a rejection. For a GitHub
  repo entry it does not apply the same way — check `makefun check` output.
- `thinking_reproduces`: `main.ts` is the kit starter's file plus a 2-line
  authored header comment; the counted lines are the site's own source
  (`app/index.html`), which the build session wrote. Starter lines are
  excluded from the counted lines by the gate.
- Sessions must fall inside the competition window (opened 2026-11-27T00:42:00Z)
  up to the entry's receipt time. Any session that began before the opening
  cannot be entered — start a new session instead.
- The build used no MCP servers and no environment secrets.
- If the harness keeps no session record, hand over the sessions as
  self-exported files with `"handed_over"` (see RULES.txt) — but note
  `handed_over_places` is none: a handed-over entry is ranked but takes no
  paid place. Prefer a harness whose sessions `bundle` reads.

## Submission itself (parent's job, NOT done here)

- Needs: a Solana keypair wallet linked to the make.fun account
  (@tuan-ngo, payout wallet Trust DBWbvedPzfmGLHhtcZd2wR8yzRWbBXFSogbjeh2Qrvux),
  a public GitHub repo created after the opening (or a source bundle via
  kit `init`), README with the three make.fun badges + GitHub About
  (website on make.fun, topic `makefun`), and `.makefun/owner.json`
  naming the wallet if the GitHub owner is not the linked login.
- Deadline: Sun 2026-11-29 07:42 +07 (00:42 UTC).
