# Connect to the AIO Container Image

- [Connect to the AIO Container Image](#connect-to-the-aio-container-image)
  - [1. Start the Testnet](#1-start-the-testnet)
    - [1.2. Minimum Requirements](#12-minimum-requirements)
    - [1.3. Install the Docker Engine](#13-install-the-docker-engine)
    - [1.4. Download the Image](#14-download-the-image)
    - [1.5. Start the Image](#15-start-the-image)
  - [2. Shut Down the Testnet](#2-shut-down-the-testnet)
    - [2.1. Stop the Container](#21-stop-the-container)
    - [2.2. Remove the Container](#22-remove-the-container)
  - [3. Troubleshooting](#3-troubleshooting)

## 1. Start the Testnet

Using the AIO docker container image is the easiest way to set up a fully functional testnet locally. Once the testnet is running you can start interacting with it through standard [Ethereum jason RPC API.](https://github.com/ethereum/execution-apis)

![alt text](./img/testnet-container.svg)

### 1.2. Minimum Requirements

- 2 Cores**
- **16G RAM**
- Docker Engine

### 1.3. Install the Docker Engine

Download and install the docker engine from [here](https://www.docker.com/)

### 1.4. Download the Image

```sh
docker pull arcologynetwork/cluster:1.17.0
```

### 1.5. Start the Image

Use the the command below to start the testnet container and map the port `8080` to the host machine. You will need the host IP to access the container image later. Remember, the host machine is the one on which your testnet docker is running. 

The port 7545 is for handling standard Ethereum json rpc calls, users can use the standard Ethereum tools like Truffle, Remix and MetaMask to connect.

```sh
docker run --name allinone-cluster -p 8080:8080 -p 7545:7545 -d arcologynetwork/cluster:1.17.0/root/dstart.sh chainID:16 rpcPort:7545
```

![alt txt](./img/docker-run.png)

```
docker ps -a
```

![alt txt](./img/docker-ps.png)

> It will take some time for the services to start. Please wait for some time before proceeding to the next steps.

## 2. Shut Down the Testnet

Use the command below the stop the testnet. Please don't try to start a testnet docker while another one is still running. Always stop the running instance first before starting the next one. Otherwise you might have to reinstall the testnet docker.

### 2.1. Stop the Container

```sh
sudo docker stop allinone-cluster 
```

### 2.2. Remove the Container

```sh
sudo docker rm allinone-cluster 
```

## 3. [Troubleshooting](./troubleshooting/questions.md)
