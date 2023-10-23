![](https://i.imgur.com/PX4WW56.jpg)

[![Chat on Discord][ico-discord]][link-discord] [![Website][ico-website]][link-website] [![Chat on Twitter][ico-twitter]][link-twitter]

[ico-discord]: https://img.shields.io/badge/-%20?style=social&logo=discord&logoColor=7B3FE4&label=polygonMiden
[ico-twitter]: https://img.shields.io/twitter/url?label=polygonMiden&style=social&url=https%3A%2F%2Ftwitter.com%2F0xpolygonmiden
[ico-website]: https://img.shields.io/static/v1?label=docs&message=PolygonMiden&color=7B3FE4

[link-discord]: https://discord.com/invite/0xpolygondevs
[link-twitter]: https://twitter.com/0xPolygonDevs
[link-website]: https://0xpolygonmiden.github.io/miden-base/introduction.html

# Polygon Miden
Polygon Miden is a zero-knowledge rollup running on the Miden VM. Polygon Miden prioritizes ZK-friendliness over EVM compatibility; that way it can offer features and benefits that are not available on Ethereum. It aims at builders that want to create high-throughput and private dApps. Miden is a general purpose rollup and builders can write and deploy arbitrary smart contracts.

## Project structure
This repository stores all the code for Polygon Miden. Everything is open source. 

| Repository              | Description |
| ----------------------- | ----------- |
| [AirScript](https://github.com/0xPolygonMiden/air-script)     | Domain-specific language for writing AIR constraints for Miden VM. |
| [Miden Base](https://github.com/0xPolygonMiden/miden-base)    | Core components of the Polygon Miden rollup. |
| [Miden Client](https://github.com/0xPolygonMiden/miden-client)| A reference Miden Client to be used by users. |
| [Miden Crypto](https://github.com/0xPolygonMiden/crypto)      | Cryptographic primitives used in Polygon Miden rollup. |
| [Miden IR](https://github.com/0xPolygonMiden/miden-ir)        | MidenIR for compiling to Miden Assembly from higher-level languages. |
| [Miden Node](https://github.com/0xPolygonMiden/miden-node)    | Miden Node to be used by the Miden operators. |
| [Miden VM](https://github.com/0xPolygonMiden/miden-vm)        | STARK-based virtual machine for Polygon Miden rollup. |
| [Examples](https://github.com/0xPolygonMiden/examples)        | Examples of using the Miden VM and Miden assembly. |

## Status
At the moment you can use the Miden VM v0.6 on our [playground](https://0xpolygonmiden.github.io/examples/) and locally. Check out the Miden VM repository or our [Miden VM docs](https://0xpolygonmiden.github.io/miden-vm/intro/main.html) for more detailed instructions.
    
As soon as we have the Miden Client or Miden Node, we will make it available. Follow us on Twitter to get the latest updates.
    
In case you want to use parts of Polygon Miden - like the Miden VM or AirScript - please reach out to [us](dschmid@polygon.technology).

## Design    

### Key features of Polygon Miden
1. **Client side proving** where users can locally execute transactions and create proofs thereof on their own. 
2. **Parallel transaction execution** where causally independent transactions can be processed in parallel.
3. **Privacy** which includes the ability to engage in private transactions as well as have privacy-preserving smart contracts.
4. **Support for composable smart contracts** via safe but Turing-complete language. This is needed to support safer wallets, DeFi, DAOs, and many other cool use cases.
5. **Native support for multiple assets** where the environment itself ensures asset safety allows fee payments in multiple assets etc.

    
## License
This project is [MIT licensed](https://github.com/0xPolygonMiden/.github/blob/main/LICENSE).
