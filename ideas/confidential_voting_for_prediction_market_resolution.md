# Confidential Voting for Permissionless Prediction Markets

## Why
Prediction markets are a way to predict the outcome of events. They are used to predict the outcome of elections, sports games, and other events. Polymarket gained a lot of traction due to the 2024 US elections market. Some of their other markets have revealed underlying issues with the current state of prediction markets. Prediction markets are centralized in the sense that the markets can only be spun up by a single entity. You or I cannot go and spin up our own market, simply because how do we build a system to resolve the outcome of the market in an unbiased way? Most prediction markets use optimistic oracles to resolve the outcome of the market. But these oracles have been shown to be manipulated in the past. 

## High-level Technical Design
Honest majority confidential voting for resolution combined with staking for game theoretic incentive alignment. 

## Why is it only possible with Arcium
Confidential voting through Arcium's MPC infrastructure solves a critical game theoretic flaw in traditional prediction market resolution systems. In a transparent voting system with staking, voters can see previous votes and are incentivized to vote with the majority to avoid being slashed, regardless of the true outcome. This creates a "cascade effect" where early votes disproportionately influence the final result. By making votes private, Arcium ensures that each resolver must vote based on their genuine assessment of the outcome, as they cannot observe other votes. This aligns incentives properly: assuming an honest majority, the optimal strategy becomes voting truthfully since voters must bet that others are doing the same to avoid stake slashing.
