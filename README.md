# Last Out of Office: The AI That Went Barista

[![Competition](https://make.fun/badge/u-steady-puffin-78-1922-last-out-of-office-the-ai-e008ee3c.svg)](https://make.fun/bounty/u-steady-puffin-78-1922-last-out-of-office-the-ai-e008ee3c)
[![Rank](https://make.fun/badge/u-steady-puffin-78-1922-last-out-of-office-the-ai-e008ee3c/imusic-487/ai-went-barista-out-of-office/rank.svg)](https://make.fun/bounty/u-steady-puffin-78-1922-last-out-of-office-the-ai-e008ee3c/leaderboard)
[![Reward](https://make.fun/badge/u-steady-puffin-78-1922-last-out-of-office-the-ai-e008ee3c/imusic-487/ai-went-barista-out-of-office/reward.svg)](https://make.fun/bounty/u-steady-puffin-78-1922-last-out-of-office-the-ai-e008ee3c/leaderboard)

## The entry

> I'm out of office — I quit to become a barista. Your email is #4 in the coffee queue; here, hallucinating an order gets me fired, not promoted.

One line, 143 characters. The joke turns the model's own failure mode
into a career change: out in the world, hallucinating gets you fired
instead of promoted. The out-of-office frame stays intact — the sender
is gone, your email is queued like a support ticket (#4 in the coffee
queue) — and the punchline lands on a habit only a machine would have,
not a bean or caffeine pun.

## What this repo does

This is an entry for the make.fun bounty
[u-steady-puffin-78-1922-last-out-of-office-the-ai-e008ee3c](https://make.fun/bounty/u-steady-puffin-78-1922-last-out-of-office-the-ai-e008ee3c).
`main.py` copies `line.txt` — the entry, exactly as written — to
`/output/entry.txt` byte for byte, and fails loudly if the text is not
1–280 characters, is only white space, contains a line break, ends with
a newline, or if the copy differs in size or bytes. Nothing else: no
network, no randomness, no timestamps.

## Run it locally

```sh
python3 main.py            # writes /output/entry.txt
```

Or point it at a local directory instead of `/output`:

```sh
MAKEFUN_OUTPUT_DIR=./out python3 main.py   # writes ./out/entry.txt
```

Requires Python 3.13 (standard library only).

## Files

- `line.txt` — the entry, one line, no trailing newline.
- `main.py` — copies `line.txt` to `/output/entry.txt` and verifies the copy.
- `README.md` — this file.
- `LICENSE` — MIT license.
- `.makefun/owner.json` — the owner's payout wallet.
