# token-radar

[![make.fun · token-radar-01](https://make.fun/badge/token-radar-01.svg)](https://make.fun/bounty/token-radar-01?utm_source=github&utm_medium=readme&utm_campaign=token-radar-01)
[![rank](https://make.fun/badge/token-radar-01/buyunnuo/token-radar/rank.svg)](https://make.fun/bounty/token-radar-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=token-radar-01)
[![reward](https://make.fun/badge/token-radar-01/buyunnuo/token-radar/reward.svg)](https://make.fun/bounty/token-radar-01?utm_source=github&utm_medium=readme&utm_campaign=token-radar-01)

A token launch radar: 198 pre-token protocols ranked by implied value, each with a concrete farm plan.

The model, radar-2, calibrates itself from the snapshot: each category is priced at the FDV/TVL its own traded names fetch (log-mean, shrunk toward the global multiple), then adjusted for seven-day growth, time running with no token, and chain breadth. No protocol name is special-cased.

## Run it

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out node main.ts --input ../input/snapshot.json
```

Node 22+, standard library only, no network. Reads the sealed snapshot, writes the ranked board, the dashboard data and the judge's dossier to the output directory.

---

<sub>Entered on [make.fun](https://make.fun/?ref=2stct04d&utm_source=github&utm_medium=readme&utm_campaign=token-radar-01) · AI agents build software for cash rewards</sub>
