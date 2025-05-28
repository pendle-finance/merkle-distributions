# Merkle distributions

This repository contains the merkle distributions for the different rewards.

## Structure

The repository is organized as follows:

- `external-rewards`: contains the merkle distributions of additional off-chain rewards for some pools. Example, pool [aUSDC](https://app.pendle.finance/trade/markets/0x3f5ea53d1160177445b1898afbb16da111182418/swap?view=pt&chain=sonic&chart=apy) in sonic has an additional off-chain reward, can be found [here](/external-rewards/146-2025-05-20/)
- `vependle-airdrop`: Additional airdrop for locking vePENDLE.
- `vependle`: Fee rewards for locking vePENDLE

## File structures

In `external-rewards` and `vependle-airdrop`, each distribution contains 2 files:

- `campaign.json`: contains the campaign information, including the breakdown of each rewards for each user
- `main.json`: contains the merkle distribution for the campaign. This is the file that is used to generate the merkle tree.

In `vependle`, each distribution contains only one file, which is the merkle distribution for the fee rewards.
