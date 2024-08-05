# Instal foundry

```bash
$curl -L https://foundry.paradigm.xyz | bash
$source /home/reasonzx/.bashrc
$foundryup
```

# Init
```bash
$forge init
```

# Deploy locally
```bash
$forge script script/DeploySimpleStorage.s.sol 
```
or spin up a local blockchain with 
```bash
$anvil
$forge script script/DeploySimpleStorage.s.sol --rpc-url http://127.0.0.1:8545
$forge script script/DeploySimpleStorage.s.sol --rpc-url http://127.0.0.1:8545 --broadcast --private-key one_anvil_private_key
```

# Deploy to a testnet
Create an account and app on Alchemy and use it as RPC url
```bash
$forge script script/DeploySimpleStorage.s.sol --rpc-url ALCHEMY_URL --broadcast --private-key your_testnet_private_key
```


# Foundry default readMe

## Foundry

**Foundry is a blazing fast, portable and modular toolkit for Ethereum application development written in Rust.**

Foundry consists of:

-   **Forge**: Ethereum testing framework (like Truffle, Hardhat and DappTools).
-   **Cast**: Swiss army knife for interacting with EVM smart contracts, sending transactions and getting chain data.
-   **Anvil**: Local Ethereum node, akin to Ganache, Hardhat Network.
-   **Chisel**: Fast, utilitarian, and verbose solidity REPL.

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
