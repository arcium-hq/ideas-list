# Dark Pool (aka, onchain encrypted orderbook)

## Why
Dark pools are private exchanges primarily used by large institutional investors to trade securities without revealing their intentions to the broader market. They enable the execution of substantial trades with minimal market impact, reducing slippage and potentially lowering transaction costs. The significance of dark pools in modern financial markets is substantial; for instance, on NASDAQ, up to 40% of trades occur in dark pools.

## High-level Technical Design
Encrypt orderbook and store onchain. Run a cranker to constantly watch the state of the encrypted orderbook and execute matches if found. Trades can be settled using an in-app accounting system. 

## Why is it only possible with Arcium
Implementing dark pools on-chain presents unique challenges, particularly in maintaining the confidentiality of the order book. zk proofs can't enable shared private state which is a requirement for a dark pool. Arcium enables having an encrypted shared orderbook on-chain which can be computed on top of without revealing the orderbook at any point. 