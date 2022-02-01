# Hardhat Stream Blocks

This repo contains a script (`scripts/index.ts`) and a `hardhat.config.ts` to fetch blocks from an upstream provider and replay them against a local fork node. 

The script and config configured hardhat to mine transactions in blocks. 

## Usage

```
FORK_URL=https://eth-mainnet.alchemyapi.io/v2/AlchemyApiKey
FORK_BLOCK_NUMBER=14047500
npx hardhat node --fork $FORK_URL --fork-block-number $FORK_BLOCK_NUMBER
```

```
FORK_URL=https://eth-mainnet.alchemyapi.io/v2/AlchemyApiKey
FORK_BLOCK_NUMBER=14047500
npx hardhat run ./scripts/index.ts --network localhost
```