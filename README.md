# BNB Chain MCP

<p align="center">
  <a href="https://www.npmjs.com/package/@nirholas/bnbchain-mcp"><img src="https://img.shields.io/npm/v/@nirholas/bnbchain-mcp.svg?style=for-the-badge&logo=npm&color=cb3837" alt="npm version"></a>
  <a href="https://www.npmjs.com/package/@nirholas/bnbchain-mcp"><img src="https://img.shields.io/npm/dm/@nirholas/bnbchain-mcp.svg?style=for-the-badge&logo=npm&color=cb3837" alt="npm downloads"></a>
  <a href="LICENSE"><img src="https://img.shields.io/badge/License-Apache%202.0-blue.svg?style=for-the-badge" alt="License: Apache 2.0"></a>
</p>

<p align="center">
  <a href="https://modelcontextprotocol.io"><img src="https://img.shields.io/badge/MCP-Compatible-6366f1?style=for-the-badge" alt="MCP Compatible"></a>
  <a href="https://www.bnbchain.org/"><img src="https://img.shields.io/badge/BNB%20Chain-F0B90B?style=for-the-badge&logo=binance&logoColor=white" alt="BNB Chain"></a>
  <a href="https://sperax.io/"><img src="https://img.shields.io/badge/Sperax-USDs-purple?style=for-the-badge" alt="Sperax"></a>
</p>

> A comprehensive Model Context Protocol (MCP) server for **BNB Chain** ecosystem - BSC EVM, BNB Greenfield storage, and Sperax Protocol (USDs stablecoin).

## Features

### 🔗 BNB Smart Chain (BSC EVM)
- **Blocks** - Query block data, latest blocks, block by number/hash
- **Tokens** - ERC20/BEP20 token operations, balances, transfers
- **NFTs** - NFT minting, transfers, metadata queries
- **Transactions** - Send transactions, get receipts, estimate gas
- **Contracts** - Deploy and interact with smart contracts
- **Wallet** - Wallet management and balance queries

### 💾 BNB Greenfield (Decentralized Storage)
- **Storage** - Create buckets, upload/download objects
- **Payment** - Manage storage payments and billing
- **Account** - Account management and permissions
- **Storage Providers** - Query and select SPs

### 💰 Sperax Protocol (USDs Stablecoin)
- **USDs** - Auto-yield stablecoin operations, mint/redeem
- **SPA** - SPA token staking, veSPA governance
- **Vault** - Vault operations, collateral management
- **Demeter** - Yield farming on Demeter DEX
- **Oracle** - Price feeds and oracle data
- **Governance** - Protocol governance and voting
- **Analytics** - Protocol metrics and analytics
- **Portfolio** - Track holdings and yields
- **Swap** - Token swaps via Sperax DEX

## Quick Start

### Claude Desktop

Add to your `claude_desktop_config.json`:

```json
{
  "mcpServers": {
    "bnbchain-mcp": {
      "command": "npx",
      "args": ["-y", "@nirholas/bnbchain-mcp@latest"],
      "env": {
        "PRIVATE_KEY": "your_private_key_here"
      }
    }
  }
}
```

### Cursor / VS Code

Add to your MCP settings:

```json
{
  "mcpServers": {
    "bnbchain-mcp": {
      "command": "npx",
      "args": ["-y", "@nirholas/bnbchain-mcp@latest"],
      "env": {
        "PRIVATE_KEY": "your_private_key_here"
      }
    }
  }
}
```

## Server Modes

| Mode | Command | Use Case |
|------|---------|----------|
| stdio | `npx @nirholas/bnbchain-mcp` | Claude Desktop, Cursor |
| HTTP | `npx @nirholas/bnbchain-mcp --http` | ChatGPT Developer Mode |
| SSE | `npx @nirholas/bnbchain-mcp --sse` | Legacy HTTP clients |

## Example Prompts

### BSC EVM Operations

```
Get my BNB balance on BSC mainnet
```

```
Transfer 0.1 BNB to 0x742d35Cc6634C0532925a3b844Bc9e7595f5eB1
```

### Greenfield Storage

```
Create a new bucket called "my-ai-data" on Greenfield
```

```
Upload this file to my Greenfield bucket
```

### Sperax Protocol

```
What is the current USDs APY?
```

```
Mint 100 USDs using USDC as collateral
```

```
Show my SPA staking rewards
```

```
What's the TVL in the Sperax vault?
```

```
Stake my SPA tokens for veSPA
```

## Supported Networks

- **BSC Mainnet** (Chain ID: 56)
- **BSC Testnet** (Chain ID: 97)
- **opBNB Mainnet** (Chain ID: 204)
- **opBNB Testnet** (Chain ID: 5611)
- **Greenfield Mainnet**
- **Greenfield Testnet**
- **Arbitrum One** (Chain ID: 42161) - Sperax
- **Arbitrum Sepolia** (Chain ID: 421614) - Sperax Testnet

## Development

```bash
# Clone the repo
git clone https://github.com/nirholas/bnbchain-mcp
cd bnbchain-mcp

# Install dependencies
npm install

# Run in development mode
npm run dev

# Build
npm run build

# Run tests
npm test
```

## Related Projects

- [universal-crypto-mcp](https://github.com/nirholas/universal-crypto-mcp) - Universal MCP for all blockchains
- [Binance-MCP](https://github.com/nirholas/Binance-MCP) - Binance.com exchange API
- [Binance-US-MCP](https://github.com/nirholas/Binance-US-MCP) - Binance.US exchange API
- [sperax-crypto-mcp](https://github.com/nirholas/sperax-crypto-mcp) - Sperax Protocol MCP

## License

Apache 2.0 - see [LICENSE](LICENSE)

## Author

[nirholas](https://github.com/nirholas)
