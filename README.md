# Copy-trade experiment ($52 paper)

PAPER ONLY: pretend money. No real trades, wallets or exchanges are involved.

A static view of a month-long (24 Oct to 25 Nov 2026) paper copy-trading simulation that follows the top weekly trader on Kolscan (Solana memecoins) at 0.25x size, starting from a pretend $52.
`data.json` is computed on a separate machine from public data (Solana RPC, Kolscan, Jupiter and DexScreener prices) and pushed here at most every 5 minutes; `index.html` renders it.

From 25 Oct 2026 every new paper fill includes modelled costs: a 1% swap fee per side plus slippage (1% base + a liquidity tier from DexScreener pool liquidity + 2 x trade size / liquidity, capped at 15%).
