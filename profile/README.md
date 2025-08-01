# Arcology Network 
<!-- <picture> -->
  <!-- <img alt="." src="./img/github-theme.gif"> -->
  <!-- ![](/img/github-theme.gif) -->
<!-- </picture> -->

## What is Arcology :bell:
Welcome to Arcology, the world's first parallel Ethereum L2 blockchain infrastructure, specifically designed as an Ethereum Layer 2 rollup solution. If you are looking for a platform capable of processing tens of thousands complex smart contract calls in full parallel without losing composability, Arcology is your only choice.


## Parallel Execution :rocket:

Arcology is capable of processing multiple transactions, including arbitrarily complex smart contract calls in full parallel. The state consistency is always strictly protected by the concurrency framework. Arcology effortlessly handles tens of thousands of transactions per second.

![](/img/system.png)

## EVM Equivalent

It maintains full EVM equivalence. You can deploy your smart contracts to Arcology without modification and vice versa as long as you **don't** use any Arcology concurrent API in the source code.

## Concurrent API in Solidty

Arcology features a concurrent API in native Solidty, making it easy for smart contract developers to parallelize their contracts with minimal effort.

![](/img/coin-contract.gif)


## Nettedswap

[Nettedswap](https://github.com/arcology-network/nettedswap) is a high-performance AMM DEX built on the Uniswap v3 codebase. It adds an **on-chain netting layer** that batches and offsets trades before they reach liquidity pools, significantly reducing slippage, mitigating MEV, and enabling massive parallel execution.


## Other Example APPs

Here is a list of applications parallelized with the Concurrent API. Let us know if you'd like to add yours to the list.

 - [CryptoKitties](https://github.com/arcology-network/parallel-kitties)
 - [DSToken](https://github.com/arcology-network/parallel-dstoken)
 - [Coin transfers](https://github.com/arcology-network/parallel-coin-transfer)

## Architecture :desktop_computer: +...+ :desktop_computer:

On Arcology, a node is no longer a single machine but can be a group of interconnected computers with functional modules deployed. All the machines can work collaboratively to share the workload (execution/storage/bandwidth) just like one. The overall throughput is proportional to amount of the resources available.


## [Arcology Docs](https://doc.arcology.network/product-docs/overview/welcome-to-arcology-network) :book:

<!-- ## Get in Touch :loudspeaker:

[<code><img height="40" src="icons/arcology-a.png"></code>](https://www.arcology.network)
[<code><img height="40" src="icons/twitter.svg"></code>](https://twitter.com/ArcologyN)
<!-- [<code><img height="40" src="icons/telegram.svg"></code>]()
[<code><img height="40" src="icons/discord.svg"></code>](https://discord.gg/SkkCtZuAnm) 
[<code><img height="40" src="icons/medium.svg"></code>](https://medium.com/arcology-network) -->
[<code><img height="40" src="icons/email.png"></code>](mailto:info@arcology.network) -->

