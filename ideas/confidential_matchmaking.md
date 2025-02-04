# Confidential Matchmaking

## Why
Matchmaking is a critical component of many online services, from dating apps to multiplayer games. However, the current state of matchmaking is often centralized and lacks privacy. This can lead to issues such as data leaks and biased matchmaking.

## High-level Technical Design
User profiles can be encrypted and stored on-chain as is or as part of NFT metadata. Arcium can be used to execute secure set intersection & matching, without revealing the underlying data.

## Why is it only possible with Arcium
Arcium allows to have confidential computing on top of shared private state, which is a necessity for privacy in such applications. Traditional matchmaking systems are prone to data leaks, and unauthorized selling of your data, which might be sensitive information, for eg, data of dating profile. 
