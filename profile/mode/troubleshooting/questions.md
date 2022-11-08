# Troubleshooting

- [Troubleshooting](#troubleshooting)
  - [1.1. The Network Isn't Responding](#11-the-network-isnt-responding)
    - [1.1.1. Check You Network Configurations](#111-check-you-network-configurations)
    - [1.1.2. Check Your System](#112-check-your-system)
    - [1.1.3. Check Your AIO](#113-check-your-aio)
  - [1.2. The Localhost Doesn't Work](#12-the-localhost-doesnt-work)
  - [1.3. Why Am I Receiving {"sysdbg":"block is nil"}](#13-why-am-i-receiving-sysdbgblock-is-nil)

## 1.1. The Network Isn't Responding

The whole starting process may take a few minutes. If you only see some of the services running, that is usually because other services haven't been started yet, just can check back later. If the problem persists after a few minutes, checking the followings.

### 1.1.1. Check You Network Configurations

If the network isn't responding, please refer to the section below.

- Your firewall must allow inbound connections to the designated port.
- Check port forwarding settings on your hardware router.
- The port 8080 of the docker container image must be mapped to a corresponding port on your host machine.
  
### 1.1.2. Check Your System

 make sure your system meets the [minimum requirements.](../aio-docker####12minimum-requirements)

### 1.1.3. Check Your AIO

In case you are using the AIO container image, the container image rarely has any issues, but it is still possible to [see if all the services are running properly](./aio-login.md).

## 1.2. The Localhost Doesn't Work

Don't use the localhost 127.0.0.1 when you try to connect to a testnet from the client docker, even if the testnet container is running on the same host machine with you client container.

## 1.3. Why Am I Receiving {"sysdbg":"block is nil"}

If you are receiving {"sysdbg":"block is nil"} in the browser window, while checking the connectivity, remove the testnet docker first and then start the testnet again.

