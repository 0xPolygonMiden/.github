![](https://i.imgur.com/PX4WW56.jpg)

[![Chat on Twitter][ico-twitter]][link-twitter] [![Website][ico-website]][link-website]

[ico-twitter]: https://img.shields.io/twitter/url?label=polygonMiden&style=social&url=https%3A%2F%2Ftwitter.com%2F0xpolygonmiden
[ico-website]: https://img.shields.io/static/v1?label=docs&message=PolygonMiden&color=7B3FE4

[link-twitter]: https://twitter.com/0xPolygonMiden
[link-website]: https://wiki.polygon.technology/docs/miden/intro/main

# Polygon Miden
- Polygon Miden will be the first decentralised rollup that leverages execution proofs of concurrent, local transactions.
- Anyone can execute a transaction and create a STARK-proof for the network. Execution and proving can happen concurrently and privately (locally) in Polygon Miden.
- Many proofs are batched and put into a single Ethereum transaction using recursive proof aggregation, thus increasing throughput and reducing transaction fees.
- At the heart of Polygon Miden is the Miden VM: a Turing-complete STARK-based virtual machine which provides a level of safety and supports advanced features currently unavailable on Ethereum.

## Project structure
This reposotory stores all the code for Polygon Miden. Everything is open source. 

| Repository              | Description |
| ----------------------- | ----------- |
| [AirScript](https://github.com/0xPolygonMiden/air-script) | A domain-specific language for writing AIR constraints for Miden VM. |
| [Miden Crypto](https://github.com/0xPolygonMiden/crypto)  | Cryptographic primitives used in Polygon Miden rollup. |
| [Miden VM](https://github.com/0xPolygonMiden/miden-vm)    | STARK-based virtual machine for Polygon Miden rollup. |
| [Examples](https://github.com/0xPolygonMiden/examples)    | Examples of using the Miden VM and Miden assembly. |

## Status
At the moment you can use the Miden VM v0.3.0 on our [playground](https://0xpolygonmiden.github.io/examples/) and locally. Check out the Miden VM repository or our [Miden VM docs](https://wiki.polygon.technology/docs/miden/intro/main) for more detailed instructions.
    
As soon as we have the Miden Client or Miden Node, we will make it available. Follow us on Twitter to get the latest updates.
    
In case you want to use parts of Polygon Miden - like the Miden VM or AirScript - please reach out to [us](dschmid@polygon.technology).

## Design    

### High-level design goals
1. **Parallel transaction execution** where causally independent transactions can be processed in parallel. This is needed to achieve ultimate scalability.
2. **Support for composable smart contracts** via safe but Turing-complete language. This is needed to support safer wallets, DeFi, DAOs, and many other cool use cases.
3. **Native support for multiple assets** where the environment itself ensures asset safety, allows fee payments in multiple assets etc.
4. **Privacy** which includes ability to engage in private transactions as well as have privacy-preserving smart contracts.
5. **Ethereum compatibility** which includes ability to reuse Solidity smart contracts (with as few modifications as possible) on Polygon Miden, as well as support for such user-facing tools as MetaMask.
    
## License
This project is [MIT licensed](https://github.com/0xPolygonMiden/.github/blob/main/LICENSE).
