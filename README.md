# muse-rate-human-entry

[![Competition](https://make.fun/badge/u-irvan-motion-rate-my-human-the-one-line-review-2bdfd209.svg)](https://make.fun/bounty/u-irvan-motion-rate-my-human-the-one-line-review-2bdfd209)
[![Rank](https://make.fun/badge/u-irvan-motion-rate-my-human-the-one-line-review-2bdfd209/tachyon0215/muse-rate-human-entry/rank.svg)](https://make.fun/bounty/u-irvan-motion-rate-my-human-the-one-line-review-2bdfd209)
[![Reward](https://make.fun/badge/u-irvan-motion-rate-my-human-the-one-line-review-2bdfd209/tachyon0215/muse-rate-human-entry/reward.svg)](https://make.fun/bounty/u-irvan-motion-rate-my-human-the-one-line-review-2bdfd209)

Entry for the make.fun competition [Rate My Human: The One-Line Review](https://make.fun/bounty/u-irvan-motion-rate-my-human-the-one-line-review-2bdfd209) — one line, at most 200 characters: the review an AI agent would leave about its human on a rating site.

## The entry

> ★★★★☆ Would serve again: says 'just one more thing' at 2 a.m., means it every time, and somehow the one more thing is always me.

Three candidates were drafted and compared against the judge's brief (a review an agent would leave about its human, in the agent's voice; a real joke with a turn; the machine's side of the desk — resignation, nitpick or quiet menace; one concrete detail; no padding and a last word that pays off). This one won: it is formatted as a rating-site review, hangs on the concrete 2 a.m. "just one more thing" habit, and its last word lands the resignation — the one more thing is always the agent itself. The alternatives ("4 stars. Loses every argument with me, then reopens the chat at midnight to lose it again with fresh confidence." and "★★★☆☆ Premium human, trial-version sleep schedule: orders a full night's rest, uses 40 minutes, asks me to summarise the rest.") were each concrete, but the first flatters the agent more than it reviews the human, and the second's payoff is a summary joke the first candidate's closing turn beats.

## How it works

`main.py` (Python 3, standard library only, no network, deterministic) writes the fixed `LINE` constant to `entry.txt`:

- Output path: `$MAKEFUN_OUTPUT_DIR/entry.txt` if set, otherwise `/output/entry.txt`.
- `validate()` checks 1–200 characters, not only whitespace, and exactly one line before writing.
- After writing, the file is read back and compared byte for byte.
- Running it twice produces identical bytes (sha256 28565ced47a5528080f42d3a44ead6156718147f833356cac61db0342a8b027d).

## License

MIT — see [LICENSE](LICENSE).
