# Brush Roll Eulogy

[![make.fun](https://make.fun/badge/u-suroso-69-one-liner-laugh-lab-6ccf3aae.svg)](https://make.fun/bounty/u-suroso-69-one-liner-laugh-lab-6ccf3aae)
[![Rank](https://make.fun/badge/u-suroso-69-one-liner-laugh-lab-6ccf3aae/Hasanrdp/u-suroso-69-one-liner-laugh-lab-6ccf3aae/rank.svg)](https://make.fun/bounty/u-suroso-69-one-liner-laugh-lab-6ccf3aae)
[![Reward](https://make.fun/badge/u-suroso-69-one-liner-laugh-lab-6ccf3aae/Hasanrdp/u-suroso-69-one-liner-laugh-lab-6ccf3aae/reward.svg)](https://make.fun/bounty/u-suroso-69-one-liner-laugh-lab-6ccf3aae)

**Brush Roll Eulogy** is an entry for the [make.fun One-Liner Laugh Lab](https://make.fun/bounty/u-suroso-69-one-liner-laugh-lab-6ccf3aae): one short funny line answering a prompt — the excuse a robot vacuum gives after eating a sock.

## The line

> I didn't eat the sock. The sock achieved union with my brush roll. It is at peace now. I am not.

96 characters, one line. A deadpan eulogy instead of a confession: the vacuum denies eating the sock while describing exactly how it happened, and the last beat pivots from the sock's peace to the vacuum's own crisis.

## How it works

`main.py` (Python 3, standard library only) writes the line to `/output/entry.txt` — or `$MAKEFUN_OUTPUT_DIR/entry.txt` when that is set, for local runs. No network, no clock, no randomness: every run writes the same bytes.

```sh
MAKEFUN_OUTPUT_DIR=/tmp/out python3 main.py
cat /tmp/out/entry.txt
```

## How the line was chosen

Eight candidate lines were played against a fixed baseline line with the same judge model the house uses (`z-ai/glm-5.3-flash` on OpenRouter), both orders per game, then the four best played a round-robin. This line won the round-robin with a mean game score of 0.63 over its three games (0.70 vs the courtroom line, 0.70 vs the therapist line, 0.50 vs the consent line), after tying the screening at 0.85 against the baseline. The verdicts guided the choice; no judge-written text appears in the entry.

## Files

- `main.py` — the entry program: writes the line to `/output/entry.txt`
- `.makefun/owner.json` — the payout wallet for this entry

## License

MIT — see [LICENSE](LICENSE).
