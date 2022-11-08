# Arcology Network

## What is Arcology
Arcology network A truly scalable L1 blockchain infrastructure. If you are looking for a platform capable of processing tens of thousands complex smart contract calls in full parallel without losing composability, Arcology is your only choice.


<picture>
  <img alt="." src="img/theme.png" width="800" height="400">
</picture>

## Architecture

Arcology adopted an event-driven microservice architecture. Arcology uses [Streamer]() to coordinate different threads in the same process. For inter-process communication (IPC), Arcology relays on Apache Kafka. The overall throughput is proportional to amount of the resources available.

In case the workload outgrows the resources of a single virtual machine, you can scale up using a machine cluster to run a single node. All you need to do is to change some settings.

## Parallel Execution

Arcology is capable of processing multiple transactions, including arbitrarily complex smart contract calls in pull parallel. The state consistency is strictly protected by the concurrency framework.

## Concurrency Libraries
The [concurrency library](https://github.com/arcology-network/concurrent-programing-guide) helps you write [contention](https://en.wikipedia.org/wiki/Resource_contention)-free smart contracts to can take full advantage of Arcology's parallel transaction execution capabilities.

<img src="img/ConcurrentSample.gif" width="800" height="350" />
<!-- ![alt text](..img/arcology-light.png) -->

## Showcases
Below are some parallelized smart contracts.

 - [x] [CryptoKitties](https://github.com/arcology-network/parallel-kitties)
 - [x] [DSToken](https://github.com/arcology-network/parallel-dstoken)
 - [x] [Coin transfers](https://github.com/arcology-network/parallel-coin-transfer)

## Benchmarking Reports
  1. [3rd party](https://arcology.network/docs/arcology-bt-report-final.pdf)
  2. [Full-scale]()

## Quick Links

- [x] [Connecting Wallet](exploring/metamask.md)
- [x] [Writing concurrent smart contracts](https://github.com/arcology-network/concurrent-programing-guide)
- [x] [Reading the whitepaper](https://github.com/arcology-network/whitepaper)
- [x] [Arcology Architecture](https://github.com/arcology-network/architecture)
- [x] [Benchmarking Arcology](benchmarking/benchmarking.md)

## Get in Touch
[<code><img height="40" src="../img/arcology-a.png"></code>](https://www.arcology.network)
[<code><img height="40" src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/twitter/twitter.png"></code>](https://twitter.com/ArcologyN)
[<code><img height="40" src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/telegram/telegram.png"></code>]()
[<code><img height="40" src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/discord/discord.png"></code>](https://discord.gg/SkkCtZuAnm)
[<code><img height="40" src="../img/medium.png"></code>](https://medium.com/arcology-network)
