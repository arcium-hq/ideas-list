# Sealed Bid Auctions

## Why
Sealed-bid auctions provide a secure and discreet environment for buyers all over the world to bid on high-end vehicles, luxury products, fine art, and offshore oil leases as well.

## High-level Technical Design
Bidders submit encrypted bids which are compiled on-chain. Track highest bid at any point (for first-price sealed bid auctions). 

## Why is it only possible with Arcium
Arcium's use of MPC allows for the secure submission and evaluation of bids without revealing them to other participants or even the auctioneer. Building sealed bid auction systems on-chain are better than offchain systems because it is verifiable, hence more secure. 