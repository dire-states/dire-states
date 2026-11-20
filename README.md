Tools and open data for the Filecoin network. Website: [dire-states.github.io](https://dire-states.github.io/)

### sector-spiegel

How long do Filecoin sectors live? sector-spiegel tracks every live sector on mainnet and calibnet,
shows when each miner's sectors expire, and estimates when the network runs out of them if nobody
extends.

- **Site:** [mainnet](https://dire-states.github.io/filecoin-sector-spiegel/?net=mainnet) · [calibnet](https://dire-states.github.io/filecoin-sector-spiegel/)
- **Source:** [filecoin-sector-spiegel](https://github.com/dire-states/filecoin-sector-spiegel)
- **Data:** [mainnet](https://github.com/dire-states/filecoin-sector-spiegel-data-main) · [calibnet](https://github.com/dire-states/filecoin-sector-spiegel-data-calibration). These are snapshots of every miner's live sectors, updated several times a day.

### message-mix

What is the Filecoin chain doing? message-mix counts every message on mainnet and calibnet by the
receiving actor type and method (`miner.SubmitWindowedPoSt`, `evm.InvokeContract`, `account.Send`, …)
in hourly buckets, and shows the result as a time series you can browse.

- **Site:** [mainnet](https://dire-states.github.io/filecoin-message-mix/?net=mainnet) · [calibnet](https://dire-states.github.io/filecoin-message-mix/)
- **Source:** [filecoin-message-mix](https://github.com/dire-states/filecoin-message-mix)
- **Data:** [mainnet](https://github.com/dire-states/filecoin-message-mix-data-main) · [calibnet](https://github.com/dire-states/filecoin-message-mix-data-calibration). These are daily and hourly CSV files of message counts per method, updated several times a day.

### fil-release

When is locked FIL released? fil-release reads every miner's vesting block rewards and the initial
pledge of each live sector on mainnet and calibnet, and shows when they unlock: per miner, per day,
and for the whole network.

- **Site:** [mainnet](https://dire-states.github.io/filecoin-fil-release/) · [calibnet](https://dire-states.github.io/filecoin-fil-release/?net=calibnet)
- **Source:** [filecoin-fil-release](https://github.com/dire-states/filecoin-fil-release)
- **Data:** [mainnet](https://github.com/dire-states/filecoin-fil-release-data-main) · [calibnet](https://github.com/dire-states/filecoin-fil-release-data-calibration). These are snapshots of every miner's vesting schedule and sector pledge release dates, updated 4 times a day.

### public-mpool

What's waiting to get on chain? public-mpool watches the Filecoin mainnet mempool through public RPC
nodes (Glif, Zondax, dRPC, Ankr) while the page is open. It lists pending messages with their fees,
age and full JSON, charts mempool size and premiums, measures how long messages wait before inclusion,
and shows how each node's mempool differs.

- **Site:** [mainnet](https://dire-states.github.io/filecoin-public-mpool/)
- **Source:** [filecoin-public-mpool](https://github.com/dire-states/filecoin-public-mpool)
- **Data:** none stored. The page polls the nodes from your browser and shows only what happened since you opened it.
