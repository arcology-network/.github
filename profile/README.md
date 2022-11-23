# Arcology Network 

## What is Arcology :bell:
Arcology network A truly scalable L1 blockchain infrastructure. If you are looking for a platform capable of processing tens of thousands complex smart contract calls in full parallel without losing composability, Arcology is your only choice.

<picture>
  <img alt="." src="./img/theme4.png">
</picture>

## Architecture :gear:

Arcology adopted an event-driven microservice architecture. All the key models are provided as web services. Arcology uses Streamer to coordinate different threads in the same process. For inter-process communication (IPC), Arcology relays on Apache Kafka.

## Cluster Deployment :desktop_computer: +...+ :desktop_computer:

On Arcology, a node is no longer a single machine but can be a group of interconnected computers with functional modules deployed. All the machines can work collaboratively to share the workload (execution/storage/bandwidth) just like one. The overall throughput is proportional to amount of the resources available.

In case the workload outgrows the resources of a single machine, try the cluster mode.

## Parallel Execution :rocket:

Arcology is capable of processing multiple transactions, including arbitrarily complex smart contract calls in full parallel. The state consistency is always strictly protected by the concurrency framework. **Check out how some popular Dapps can benefit from the power of parallel execution.**  :fire:
 
 - [CryptoKitties](https://github.com/arcology-network/parallel-kitties)
 - [DSToken](https://github.com/arcology-network/parallel-dstoken)
 - [Coin transfers](https://github.com/arcology-network/parallel-coin-transfer)

## Concurrency Libraries :pencil:

The [concurrency library](https://docs.arcology.network/arcology-concurrent-programming-guide/) helps you write [contention](https://en.wikipedia.org/wiki/Resource_contention)-free smart contracts to take full advantage of Arcology's parallel transaction execution capabilities.

<img src="./img/ConcurrentSample3.gif" height="800"/> 


## Benchmarking Reports  :chart_with_upwards_trend: 

 - [x] [3rd party](https://arcology.network/docs/arcology-bt-report-final.pdf)
 - [x] [Internal](TBD)

## Quick Links :pushpin:

- [x] [Start a testnet](deployment/aio-docker.md)
- [x] [Connecting wallet](exploring/metamask.md)
- [x] [Writing concurrent smart contracts](https://docs.arcology.network/arcology-concurrent-programming-guide/)
- [x] [Reading the whitepaper](https://docs.arcology.network/arcology-technical-whitepaper/)
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
