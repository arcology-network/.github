# Arcology Network

## What is Arcology
Arcology network A truly scalable L1 blockchain infrastructure. If you are looking for a platform capable of processing tens of thousands complex smart contract calls in full parallel without losing composability, Arcology is your only choice.

<picture>
  <img alt="." src="./img/theme.png">
</picture>

## Architecture

Arcology adopted an event-driven microservice architecture. Arcology uses [Streamer]() to coordinate different threads in the same process. For inter-process communication (IPC), Arcology relays on Apache Kafka. The overall throughput is proportional to amount of the resources available.

In case the workload outgrows the resources of a single virtual machine, you can scale up using a machine cluster to run a single node. All you need to do is to change some settings.

## Parallel Execution

Arcology is capable of processing multiple transactions, including arbitrarily complex smart contract calls in pull parallel. The state consistency is strictly protected by the concurrency framework.

Check out how some popular Dapps can benefit from the power of parallel execution.

 - [CryptoKitties](https://github.com/arcology-network/parallel-kitties)
 - [DSToken](https://github.com/arcology-network/parallel-dstoken)
 - [Coin transfers](https://github.com/arcology-network/parallel-coin-transfer)


## Concurrency Libraries

The [concurrency library](https://github.com/arcology-network/concurrent-programing-guide) helps you write [contention](https://en.wikipedia.org/wiki/Resource_contention)-free smart contracts to can take full advantage of Arcology's parallel transaction execution capabilities.

<img src="./img/ConcurrentSample.gif" width="800" height="350" />

## Benchmarking Reports

 - [x] [3rd party](https://arcology.network/docs/arcology-bt-report-final.pdf)
 - [x] [Internal](TBD)

## Quick Links

- [x] [Connecting Wallet](exploring/metamask.md)
- [x] [Writing concurrent smart contracts](https://github.com/arcology-network/concurrent-programing-guide)
- [x] [Reading the whitepaper](https://github.com/arcology-network/whitepaper)
- [x] [Arcology Architecture](https://github.com/arcology-network/architecture)
- [x] [Benchmarking Arcology](benchmarking/benchmarking.md)

## Get in Touch

[<code><img height="40" src="img/arcology-a.png"></code>](https://www.arcology.network)
[<code><img height="40" src="img/twitter.svg"></code>](https://twitter.com/ArcologyN)
[<code><img height="40" src="img/telegram.svg"></code>]()
[<code><img height="40" src="img/discord.svg"></code>](https://discord.gg/SkkCtZuAnm)
[<code><img height="40" src="img/medium.svg"></code>](https://medium.com/arcology-network)
