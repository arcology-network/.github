# Check Network Status

- [Check Network Status](#check-network-status)
  - [1. Connect](#1-connect)

## 1. Connect

To check if the network is reachable, paste the following line into your browser.

```sh
http://localhost:8080/blocks/latest?access_token=access_token&transactions=false
```

You should see something like the blow.

```json
{
  "block": {
      "height":41285,
      "hash":"b2858fbefc496e844e1a7e8a0d2ee23afb8c18492f1ce694b70160fe96db7c47",
      "coinbase":"0x971Df33B1EFe022ec4173E61f1113C3887c08b8E",
      "number":0,
      "transactions":null,
      "gasUsed":0,
      "elapsedTime":173000,
      "timestamp":1632962218
  }
}
```

>Replace the `localhost` with the node IP

If the network isn't responding, please refer for [troubleshooting.](./questions.md)
