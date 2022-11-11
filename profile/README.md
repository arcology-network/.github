# Arcology Network 

## What is Arcology :bell:
Arcology network A truly scalable L1 blockchain infrastructure. If you are looking for a platform capable of processing tens of thousands complex smart contract calls in full parallel without losing composability, Arcology is your only choice.

<picture>
  <img alt="." src="./img/theme2.png">
</picture>

## Architecture :sunny:

Arcology adopted an event-driven microservice architecture. Arcology uses [Streamer]() to coordinate different threads in the same process. For inter-process communication (IPC), Arcology relays on Apache Kafka. The overall throughput is proportional to amount of the resources available.

In case the workload outgrows the resources of a single virtual machine, you can scale up using a machine cluster to run a single node. All you need to do is to change some settings.

## Parallel Execution :rocket:

Arcology is capable of processing multiple transactions, including arbitrarily complex smart contract calls in pull parallel. The state consistency is strictly protected by the concurrency framework. **Check out how some popular Dapps can benefit from the power of parallel execution.**  :fire:
 
 
 abcd
 - [CryptoKitties](https://github.com/arcology-network/parallel-kitties)
 - [DSToken](https://github.com/arcology-network/parallel-dstoken)
 - [Coin transfers](https://github.com/arcology-network/parallel-coin-transfer)

## Concurrency Libraries :pencil:

The [concurrency library](https://docs.arcology.network/arcology-concurrent-programming-guide/) helps you write [contention](https://en.wikipedia.org/wiki/Resource_contention)-free smart contracts to can take full advantage of Arcology's parallel transaction execution capabilities.

<img src="./img/caption3.png" width="190"/> <img src="./img/ConcurrentSample.gif" height="300"/> 


## Benchmarking Reports  :chart_with_upwards_trend: 

 - [x] [3rd party](https://arcology.network/docs/arcology-bt-report-final.pdf)
 - [x] [Internal](TBD)

## Quick Links :pushpin:

- [x] [Connecting Wallet](exploring/metamask.md)
- [x] [Writing concurrent smart contracts](https://docs.arcology.network/arcology-concurrent-programming-guide/)
- [x] [Reading the whitepaper](https://arcology-network.gitbook.io/arcology-technical-whitepaper/)
- [x] [Arcology Architecture](https://github.com/arcology-network/architecture)
- [x] [Benchmarking Arcology](benchmarking/benchmarking.md)

## Get in Touch :loudspeaker:

[<code><img height="40" src="icons/arcology-a.png"></code>](https://www.arcology.network)
[<code><img height="40" src="icons/twitter.svg"></code>](https://twitter.com/ArcologyN)
[<code><img height="40" src="icons/telegram.svg"></code>]()
[<code><img height="40" src="icons/discord.svg"></code>](https://discord.gg/SkkCtZuAnm)
[<code><img height="40" src="icons/medium.svg"></code>](https://medium.com/arcology-network)
[<code><img height="40" src="icons/email.png"></code>](mailto:info@arcology.network)
![](https://visitor-badge.glitch.me/badge?page_id=arcology-network)
