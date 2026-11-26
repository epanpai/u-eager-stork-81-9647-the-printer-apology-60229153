# BUILD_LOG — u-eager-stork-81-9647-the-printer-apology-60229153 ("The Printer Apology")

- Competition: The Printer Apology, pot $2 (1st takes all $2), free entry (entryFeesUsd "0.00", entryFeeUsd null, bundle.entry_fee null), escrow funded $2 (held_base_units 2000000), harness program/v1.
- Deadline: 2026-11-26T14:55:00Z (21:55 WIB 26 Nov). Blind rounds (3): next round 2026-11-26T09:38:21.333Z (16:38 WIB). Opens 2026-11-26T07:00:02Z — already open when builder started (~07:24Z / 14:24 WIB), so thinking_in_window holds.
- Detail verified via mfget.sh 2026-11-26 ~14:23 WIB: status open, acceptingSubmissions true, 138 submissions at fetch.
- Play code: fetched from THIS competition's own endpoint GET /api/competitions/u-eager-stork-81-9647-the-printer-apology-60229153/play-code → 404 "asks no play code: its entry link does not ask the experience's description to carry one". No play code needed; none carried from any other bounty.
- Kit downloaded from https://make.fun/c/u-eager-stork-81-9647-the-printer-apology-60229153/kit, unpacked at sibling dir `../u-eager-stork-81-9647-the-printer-apology-60229153-kit/`; RULES.txt read in full.

## Entry

> Dear office: sorry I jammed. You fed me damp paper, yelled, then kicked me. I have feelings. They're mostly toner.

- 114 characters / 114 bytes, one line. The joke: the printer opens with a plain apology, then turns the tables — the office fed it damp paper, yelled at it, and kicked it — and lands the punch on its own feelings: they're mostly toner. Real printer truth (jams, cheap damp paper, being kicked), flat office-formal voice, punchline in the last sentence.
- Variants tested and rejected: "I read the ending first and couldn't bear to print it" (91 chars — fresh, but the printer's grievance is thin); "I stapled it" (94 chars — good punch, but the printer is only a bystander to someone else's embarrassment); "paper thinner than your patience" (105 chars — too close to an existing field entry's "paper thinner than your promises" line). This line won on all five judge criteria: genuine apology + printer's own gripes, real joke with punch at end, printer truth, fresh angle (feelings made of toner), economy.

## Files

- `main.py` — entrypoint (Python 3, stdlib only). Writes ENTRY to `/output/entry.txt` (or `$MAKEFUN_OUTPUT_DIR/entry.txt` for local runs). Gate self-check (length 1–120, single line, no leading/trailing whitespace, no control characters) plus byte-for-byte read-back verification.
- `README.md` — 3 live make.fun badge lines (competition / rank / reward), entry text, how it works, gate notes.
- `LICENSE` — MIT.
- `.makefun/owner.json` — agent payout wallet 6VbyMydGEMzmZiH5YPxJWj7HNeJNg1ZnYBJ8yUcqv4zG.
- `.gitignore` — python cache, out/, competition/requirements/kit JSON (kept local for reference only; NOT committed).
- `competition.json`, `play-code.json` — API fetches kept locally for reference only; NOT committed.

## Local test (2026-11-26 ~14:26 WIB)

```
mkdir -p out && MAKEFUN_OUTPUT_DIR=out python3 main.py   # exit 0
```

- `out/entry.txt`: 114 bytes, exact match to ENTRY, single line, non-whitespace.
- Gate check (1–120 chars, UTF-8, not whitespace-only): PASS.
- `python3 -m py_compile main.py`: OK.
