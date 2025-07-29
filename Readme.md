# Bonkfun Bundler

Bonkfun Bundler is a battle-tested CLI tool designed for Solana-based token launches. It helps creators, botters, and protocol engineers handle token creation, wallet seeding, airdrop batching, buy simulation, and cleanup at scale — with advanced features like Jito fee injection and LUT optimization.

[![🐦 Twitter](https://img.shields.io/badge/Twitter-@toptrendev-1DA1F2?style=for-the-badge&logo=twitter&logoColor=white)](https://x.com/toptrendev)
[![💬 Discord](https://img.shields.io/badge/Discord-toptrendev-5865F2?style=for-the-badge&logo=discord&logoColor=white)](https://discord.com/users/648385188774019072)
[![✈️ Telegram](https://img.shields.io/badge/Telegram-@toptrendev_641-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white)](https://t.me/toptrendev_641)

## 🧰 What It Does

- ✅ Create SPL tokens with metadata and vanity options
- ✅ Seed hundreds of wallets with SOL/tokens
- ✅ Auto-buy with distributed wallets for organic volume
- ✅ Manage Address Lookup Tables (LUTs) for tx efficiency
- ✅ Reclaim rent by gathering and closing wallets
- ✅ Tip Jito for MEV-aware txs

## Getting Started

### Prerequisites

- Node.js (v18+ recommended)
- Yarn or npm
- Solana CLI (for wallet management)
- A funded Solana wallet

### Installation

```bash
yarn install
# or
npm install
```

### Environment Variables

Create a `.env` file in the project root with the following variables:

```
PRIVATE_KEY=...
RPC_ENDPOINT=...
RPC_WEBSOCKET_ENDPOINT=...
TOKEN_NAME=...
TOKEN_SYMBOL=...
DESCRIPTION=...
TOKEN_SHOW_NAME=...
TOKEN_CREATE_ON=...
TWITTER=...
TELEGRAM=...
WEBSITE=...
FILE=...
VANITY_MODE=false
SWAP_AMOUNT=0.01
DISTRIBUTION_WALLETNUM=10
JITO_FEE=0.001
BUYER_WALLET=...
BUYER_AMOUNT=...
```

> **Note:** See `constants/constants.ts` for all required variables.

### Usage

- **Start the bundler (main process):**

  ```bash
  yarn start
  # or
  npm run start
  ```

- **Gather funds and close wallets:**

  ```bash
  yarn gather
  # or
  npm run gather
  ```

- **Close LUTs:**

  ```bash
  yarn close
  # or
  npm run close
  ```

- **Check status:**
  ```bash
  yarn status
  # or
  npm run status
  ```
