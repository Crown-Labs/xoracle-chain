# xOracle Chain

The xOracle chain is a public blockchain with consensus `Proof of Stake with Authority (PoSA)`. Designed to store real-time data for xOracle functionalities like the xOracle Pricefeed and xOracle Message. It allows anyone to join the node and verify the transparency of the information feeds.

![xOracle's Architecture](https://github.com/Crown-Labs/xoracle-chain/blob/main/docs/xOracle-POSA.jpg)

## Installation

### Step 1: Initialize Genesis.json
To initialize the genesis.json file, perform the following command:

```bash
docker run --rm -it -v $PWD:/xor -v $PWD/config/genesis.json:/config/genesis.json -w /xor ethereum/client-go:latest --datadir datadir init /config/genesis.json
```

### Step 2: Create the jwt secret
Random the jwt secret as file, execute the following command:
```bash
openssl rand -hex 32 | tr -d "\n" > config/jwtsecret
```

### Step 3: Run the EL and CL node
To start the xOracle node with Docker compose, execute the following command:

```bash
docker compose up -d
```

Please note that additional configuration or setup steps may be required depending on your specific environment or
 requirements.

## Useful Links
- Block Explorer: [https://explorer.xoracle.io](https://explorer.xoracle.io/)
- Beacon chain Explorer: [https://beacon.xoracle.io](https://beacon.xoracle.io/)
- RPC Endpoint: [https://rpc.xoracle.io](https://rpc.xoracle.io)