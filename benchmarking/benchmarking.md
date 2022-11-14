# Benchmarking Arcology Network

- [Benchmarking Arcology Network](#benchmarking-arcology-network)
  - [1. Introduction](#1-introduction)
  - [2. Preparation](#2-preparation)
    - [2.1. Transactions](#21-transactions)
    - [2.2. Download the Ammolite Container Image](#22-download-the-ammolite-container-image)
    - [2.3. Check the Testnet Status](#23-check-the-testnet-status)
    - [2.4. Log in to the Ammolite Container Image](#24-log-in-to-the-ammolite-container-image)
  - [3. Start Benchmarking](#3-start-benchmarking)

## 1. Introduction

This document explains how to benchmark Arcology Network.

## 2. Preparation
You need the followings for the test:

- A live testnet
- Presigned transactions
- [An Ammolite container image](./ammolite-client.md)

### 2.1. Check the Testnet

Make sure the [testnet](../deployment/troubleshooting/check-testnet-status.md) is up and running. [Deploy a new testnet](../deployment/deployment-comparison.md) if you need to.

### 2.2. Transactions

[Downloaded the transactions](https://github.com/arcology-network/presigned-transactions) first. These files contain all pre-generated transactions for the benchmarking. 

### 2.3. Download the Ammolite Container Image

Download and start [Ammolite docker container image](../deployment/ammolite-client.md). Mount the transactions files to the right directory.

### 2.4. Log in to the Ammolite Container Image

SSH into the Ammolite container image with the command and credential below.

```sh
>ssh -p 32768 root@localhost
```

- **Username: root**
- **Password: frY6CvAy8c9E**

> If you are running the container image locally then `localhost` should work just fine. Replace `localhost` with the **host IP** of your Ammolite container if needed.

## 3. Start Benchmarking

- [Parallelized CryptoKitties](https://github.com/arcology-network/parallel-kitties)
- [Parallelized Dstoken](https://github.com/arcology-network/parallel-dstoken)
- [Parallel Coin Transfer](https://github.com/arcology-network/parallel-coin-transfer)
- [Uniswap v2](https://github.com/arcology-network/uniswap-testing)
