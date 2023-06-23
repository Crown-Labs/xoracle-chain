# xOracle Chain

The xOracle chain is a public Proof of Authority (POA) blockchain designed to store real-time price feed information. It allows anyone to join the node and verify the transparency of the information feeds.

## Installation

### Step 1: Initialize Genesis.json
To initialize the genesis.json file, perform the following command:

```bash
docker run --rm -it -v $PWD:/xor -w /xor ethereum/client-go:v1.12.0 --datadir /xor/datadir init genesis.json
```

### Step 2: Run the Node
To start the xOracle Full-Node with Docker compose, execute the following command:

```bash
docker compose up -d
```

Please note that additional configuration or setup steps may be required depending on your specific environment or
 requirements.

## Useful Links
- Block Explorer: [https://explorer.xoracle.io](https://explorer.xoracle.io/)
- RPC Endpoint: [https://rpc.xoracle.io](https://rpc.xoracle.io)