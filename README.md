# Creditcoin USC Networks

Network configuration map for Creditcoin USC environments.

## Structure

`networks.json` defines the following per network:

| Field | Description |
|---|---|
| `graphql_url` | GraphQL indexer endpoint |
| `proof_api_url` | Proof generation API endpoint |
| `creditcoin3_url` | WebSocket RPC connection |
| `blockscout_url` | Block explorer URL |
| `dashboard_url` | Dashboard URL |
| `supported_chains` | Supported chains keyed by chain ID |

Each entry in `supported_chains` contains:

| Field | Description |
|---|---|
| `name` | Chain name (e.g. sepolia, ethereum, bsc-testnet) |
| `archiver_url` | Archiver endpoint for the chain |
| `bootnodes` | Attestor bootnode addresses |

## Networks

- **usc-devnet** — USC development network (deprecated, use cc3-devnet)
- **cc3-devnet** — CC3 development network (primary dev network)
- **cc3-devnet-dryrun** — CC3 dryrun development network
- **usc-testnet** — USC test network
