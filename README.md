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
