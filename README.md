# ETCswap V2 Core

Core smart contracts for the ETCswap V2 AMM protocol on Ethereum Classic.

Forked from [Uniswap V2 Core](https://github.com/Uniswap/v2-core). The contracts are unmodified — ETCswap V2 uses the same constant-product AMM logic as Uniswap V2.

## Status: Reference Only

These contracts are deployed and immutable. This repo exists as a reference for the deployed bytecode. No further development is expected.

## Deployed Contracts

### Ethereum Classic (Chain ID: 61)

| Contract | Address |
|----------|---------|
| Factory | [`0x0307cd3D7DA98A29e6Ed0D2137be386Ec1e4Bc9C`](https://etc.blockscout.com/address/0x0307cd3D7DA98A29e6Ed0D2137be386Ec1e4Bc9C) |
| INIT_CODE_HASH | `0xb5e58237f3a44220ffc3dfb989e53735df8fcd9df82c94b13105be8380344e52` |

### Mordor Testnet (Chain ID: 63)

| Contract | Address |
|----------|---------|
| Factory | [`0x212eE1B5c8C26ff5B2c4c14CD1C54486Fe23ce70`](https://etc-mordor.blockscout.com/address/0x212eE1B5c8C26ff5B2c4c14CD1C54486Fe23ce70) |
| INIT_CODE_HASH | `0x4d8a51f257ed377a6ac3f829cd4226c892edbbbcb87622bcc232807b885b1303` |

## Key Contracts

- **UniswapV2Factory.sol** — Creates and tracks trading pairs
- **UniswapV2Pair.sol** — Constant-product AMM pair with flash swap support
- **UniswapV2ERC20.sol** — LP token implementation with permit (EIP-2612)

## Related Repos

- [v2-periphery](https://github.com/etcswap/v2-periphery) — Router and library contracts
- [v2-interface](https://github.com/etcswap/v2-interface) — Trading frontend
- [sdks](https://github.com/etcswap/sdks) — TypeScript SDK monorepo

## Local Development

```bash
yarn install
yarn compile
yarn test
```

Solidity 0.5.16. Requires Node.js 10+.
