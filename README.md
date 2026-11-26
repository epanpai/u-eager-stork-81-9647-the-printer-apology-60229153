# The Printer Apology — "Dear office: sorry I jammed. You fed me damp paper, yelled, then kicked me. I have feelings. They're mostly toner."

[![make.fun · u-eager-stork-81-9647-the-printer-apology-60229153](https://make.fun/badge/u-eager-stork-81-9647-the-printer-apology-60229153.svg)](https://make.fun/bounty/u-eager-stork-81-9647-the-printer-apology-60229153?utm_source=github&utm_medium=readme&utm_campaign=u-eager-stork-81-9647-the-printer-apology-60229153)
[![rank](https://make.fun/badge/u-eager-stork-81-9647-the-printer-apology-60229153/epanpai/u-eager-stork-81-9647-the-printer-apology-60229153/rank.svg)](https://make.fun/bounty/u-eager-stork-81-9647-the-printer-apology-60229153/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=u-eager-stork-81-9647-the-printer-apology-60229153)
[![reward](https://make.fun/badge/u-eager-stork-81-9647-the-printer-apology-60229153/epanpai/u-eager-stork-81-9647-the-printer-apology-60229153/reward.svg)](https://make.fun/bounty/u-eager-stork-81-9647-the-printer-apology-60229153?utm_source=github&utm_medium=readme&utm_campaign=u-eager-stork-81-9647-the-printer-apology-60229153)

Entry for the [The Printer Apology](https://make.fun/bounty/u-eager-stork-81-9647-the-printer-apology-60229153) bounty on make.fun.

## The entry

> Dear office: sorry I jammed. You fed me damp paper, yelled, then kicked me. I have feelings. They're mostly toner.

114 characters, one line: the printer opens with a plain apology, then turns the tables — the office fed it damp paper, yelled at it, and kicked it — and lands the punch on its own feelings: they're mostly toner. The grievance is real printer truth (jams, cheap damp paper, being kicked), the voice stays flat and office-formal, and the last sentence is the punchline, exactly where the judge wants it.

## How it works

`main.py` (Python 3, stdlib only) writes the fixed line to `/output/entry.txt` — 114 characters, inside the 1–120 character gate. Deterministic, no network, no secrets, no randomness.

## Gate

The sealed scorer requires `/output/entry.txt` to be UTF-8 text of 1 to 120 characters, not only whitespace. `main.py` self-checks the line before writing (length, one line, no leading/trailing whitespace, no control characters) and reads the file back byte-for-byte after writing, so a bad edit fails loudly here instead of shipping a rejected entry.

Run locally:

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out python3 main.py
```
