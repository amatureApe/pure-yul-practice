## PureYul instructions
1) solc --strict-assembly src/PureYul.sol
2) anvil
3) cast send --rpc-url http://localhost:8545 --private-key 0xac0974bec39a17e36ba4a6b4d238ff944bacb478cbed5efcae784d7bf4f2ff80 --create 0x6026600b5f3960265ff3fe6005601b565b637eed0172146012575f80fd5b60045f5260205ff35b600160e01b5f35049056
    - This should give you the following response:
    blockHash               0xee726704036edbd213abd5d478825079d1811431439ac51ec5f0e5658882ebe3
    blockNumber             1
    contractAddress         0x5FbDB2315678afecb367f032d93F642f64180aa3
    cumulativeGasUsed       61416
    effectiveGasPrice       4000000000
    gasUsed                 61416
    logs                    []
    logsBloom               0x00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
    root                    
    status                  1
    transactionHash         0xe391232f16b7000888fb4666dfd3b40339d3747b14662973fd13a06a7fc5ee24
    transactionIndex        0
    type                    2
4) cast call --rpc-url http://localhost:8545 0x5FbDB2315678afecb367f032d93F642f64180aa3 0x7eed0172
    - This should give you the following response:
    0x0000000000000000000000000000000000000000000000000000000000000004

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
