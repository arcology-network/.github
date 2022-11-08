# Deployment Comparison

- [Deployment Comparison](#deployment-comparison)
  - [1. Introduction](#1-introduction)
    - [1.1 Configurable](#11-configurable)
    - [1.2. Flexibility](#12-flexibility)
  - [2. Comparison](#2-comparison)
  - [3. Using the Container Image](#3-using-the-container-image)
  - [4. Performance Modes](#4-performance-modes)
    - [4.1. Single Machine Deployment](#41-single-machine-deployment)
    - [4.2. Cluster Deployment](#42-cluster-deployment)

## 1. Introduction

Arcology is a very powerful and sophisticated system. For other blockchain networks, everything has to run on the same machine. Arcology supports intra-node horizontal scaling, you can horizontally scale the modules like transaction execution and data storage onto multiple machines. These machines will work just like one.

### 1.1 Configurable

This design makes Arcology highly configurable. For example, you may have 12 machines in total and you config 6 of them to run transaction processing, 4 others for storage and 2 for other services. You could also have only 2 machines running transaction processing, 8 machine running storage and 2 for other services.

### 1.2. Flexibility

Flexibility usually comes with complexity, Arcology isn't an exception. This document explains different deployment options and pros and cons associated with them. The goal is to help Arcology users set up they Arcology testnets more effortlessly and smoothly. Users can find detailed guides below.

## 2. Comparison

Below are the deployment options users can choose from:

| Complexity   | Testnet Docker|Single machine on premise| Multiple Machines on Premise| Single Machine on Cloud|Multiple Machines on Cloud|
|---|---|---|---|---|---|
| Need to Configure the Cluster            |&cross; |&cross; |&check;| &cross;  |&check;  |
| Need to Configure the Services           |&cross; |&cross; |&check;| &cross;  |&check;  |
| Deal with Dynamic IPs                    |&cross; |&cross; |&cross;| &check;  |&check;  |
| Flexibility                              |High |Low     |Medium | Low      |Very High|
| Scalability                              |Very Low|Low     |High   | Low      |Very High|
| Deployment Complexity                  |Very Low|Low     |High   | Low      |Very High|
|

## 3. Using the Container Image

Using the docker container image comes with Arcology releases is probably the easiest way to start with. So if you are new to Arcology, we strongly suggest you to try the [docker container image.](./aio-docker.md) first before moving to the full-scale setups.

## 4. Performance Modes

There are some deployment modes that will give you better performance but they are more complex to work with.

### 4.1. Single Machine Deployment

You may prefer to use their own physical / virtual machine to host an Arcology testnet instead of using the docker container image.

[This deployment mode is more complex than using a out-of-the-box docker container image but it is still easier then setting up a machines cluster.](./single-machine.md) 

### 4.2. Cluster Deployment

If you happen to have a bunch of spare machines and necessary network equipments then it is possible to set up an Arcology node cluster.

First, you need the IP and login credential of each machine. Then you need to update IPs in the deployment configuration file. The file tells the installer scripts what services will be installed on which machines and how many instances you would like to have.

* [On-premises](https://github.com/arcology-network/deployment)
* [AWS](https://github.com/arcology-network/aws-ansible)




