<div align="center">
  <br>
  <h1>Kafka with Node.js </h1>
  <p>Live Bitcoin/ETH Wallet Tracker</p>
</div>

# Features

- Through Node.js interact with Kafka
- Produce/consume events to/from topics
- Use Kafka as a queue and as a publish/subscribe system
- Kafka with Zookeeper and without Zookeeper using Redpanda
- Make use of Kafka's partitioning ability

# Usage

**Requirements**: Node.js, Docker, Docker Compose

**Setup**

- `npm install` (Install NPM dependencies)
# Open four command / Terminal windows
- `docker-compose -f docker-compose.yaml up --build` (Start services)
- Optionally set environment variables in [`.env`](.env):
  - `BLOCKCYPHER_TOKEN` (https://accounts.blockcypher.com/tokens)

**Run**

- Rest of two terminal windows run commands like  `npx ts-node cli.ts <WALLET_ADDRESS>` (Watch a BTC or ETH wallet)
  - `npx ts-node cli.ts <BTC_WALLET_ADDRESS>`
  - `npx ts-node cli.ts <ETH_WALLET_ADDRESS>`

**Monitoring**

- http://localhost:8080 (Redpanda Console)

**Cleanup**

- `docker-compose -f docker-compose.yaml rm -s -f -v`
