# ERC4626 Tokenized Vaults

ERC4626 is a standard for tokenized Vault implementations. This repository contains a minimal, gas-efficient implementation of the ERC4626 standard.

## Key Features

- Fully compliant with the ERC4626 standard
- Gas optimized implementation using Solmate's libraries
- Built with Foundry for robust testing and development
- Includes deposit/withdrawal functionality with share calculations
- Handles decimals conversion between vault shares and underlying assets

## Architecture

The vault implementation consists of:

- `ERC4626.sol`: Main vault contract implementing the ERC4626 interface
- `ERC20.sol`: Base ERC20 implementation that the vault inherits from
- SafeTransferLib: Library for safe ERC20 transfers
- FixedPointMathLib: Library for fixed point math calculations

## Security

This is a minimal implementation meant for learning and building upon. Before using in production:

- Thoroughly test all functionality
- Add necessary access controls
- Consider adding emergency procedures
- Get a security audit

## Foundry

**Foundry is a blazing fast, portable and modular toolkit for Ethereum application development written in Rust.**

Foundry consists of:

- **Forge**: Ethereum testing framework (like Truffle, Hardhat and DappTools).
- **Cast**: Swiss army knife for interacting with EVM smart contracts, sending transactions and getting chain data.
- **Anvil**: Local Ethereum node, akin to Ganache, Hardhat Network.
- **Chisel**: Fast, utilitarian, and verbose solidity REPL.

## Documentation

https://book.getfoundry.sh/

## Usage

### Build

```shell
$ forge build
```

### Test

```shell
$ forge test
```

### Format

```shell
$ forge fmt
```

### Gas Snapshots

```shell
$ forge snapshot
```

### Anvil

```shell
$ anvil
```

### Deploy

```shell
$ forge script script/Counter.s.sol:CounterScript --rpc-url <your_rpc_url> --private-key <your_private_key>
```

### Cast

```shell
$ cast <subcommand>
```

### Help

```shell
$ forge --help
$ anvil --help
$ cast --help
```
