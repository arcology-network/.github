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
You need the followings for the test.

- Presigned transactions

- [An Ammolite container image](./ammolite-client.md)

### 2.1. Transactions

[DownloadedThe transaction data](https://github.com/arcology-network/presigned-transactions) first. These files contain all pre-generated transactions for the benchmarking. 

### 2.2. Download the Ammolite Container Image

Download and start [Ammolite docker container image](../mode/ammolite-client.md). Mount the transactions files to the right directory.

### 2.3. Check the Testnet Status

Make sure the [testnet](../mode/troubleshooting/check-testnet-status.md) is up and running. [Deploy a new testnet](../mode/deployment-comparison.md) if you need to.

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

<!-- ## 3. Deployment Contracts

By now, you should have been logged in to Ammolite docker container image. This first step is to deploy the smart contracts used in the tests.

### 3.1. deploy parallel_kitties

```sh
>cd parallel_kitties
>./deploy.sh http://192.168.1.106:8080
```

### 3.2. deploy ds_token

```sh
>cd ../ds_token
>./deploy.sh http://192.168.1.106:8080
```

### 3.3. Deploy uniswap_v2

```sh
>cd ../data/uniswap
>python deploy.py http://192.168.1.106:8080 134aea740081ac7e0e892ff8e5d0a763ec400fcd34bae70bcfe6dae3aceeb7f0
```

## 4. Start Benchmarking
Once the deployment is completed, it is time to start benchmarking.

### 4.1. Send 500k coin_transfer  

```sh
>cd
>python sendtxs.py http://192.168.1.106:8080 data/simple_transfer/simple_transfer_1m_01.dat
```

### 4.2. Send 1M parallel_kitties

```sh
>python sendtxs.py http://192.168.1.106:8080 data/pk_init_gen0/pk_init_gen0_2m_01.out
>python sendtxs.py http://192.168.1.106:8080 data/pk_kitty_transfer/pk_kitty_transfer_1m_01.dat
```

### 4.3. Send 1M ds_token

```sh
>python sendtxs.py http://192.168.1.106:8080 data/ds_token_mint/ds_token_mint_5m_1m.out

>python sendtxs.py http://192.168.1.106:8080 data/ds_token_transfer/ds_token_transfer_1m_01.out
```

### 4.4. Send 600K uniswap_v2

```sh
>cd data/uniswap
>python sendtxs.py http://192.168.1.106:8080 token1_mint_100k.out
>python sendtxs.py http://192.168.1.106:8080 token2_mint_100k.out
>python sendtxs.py http://192.168.1.106:8080 token1_approve_100k.out
>python sendtxs.py http://192.168.1.106:8080 token2_approve_100k.out
>python sendtxs.py http://192.168.1.106:8080 add_liquidity_100k.out
>python sendtxs.py http://192.168.1.106:8080 swap_100k.out
``` -->
