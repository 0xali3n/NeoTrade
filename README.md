# 🚀 Neo Trade - Next-Gen Aptos Copy Trading Platform

<div align="center">
  <img src="img/1.png" alt="Neo Trade Project Overview" width="800"/>
  
  [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
  [![Aptos](https://img.shields.io/badge/Built%20on-Aptos-blue)](https://aptoslabs.com/)
  [![Telegram](https://img.shields.io/badge/Telegram-Bot-blue)](https://telegram.org/)
  [![React](https://img.shields.io/badge/Frontend-React-blue)](https://reactjs.org/)
</div>

## 📋 Table of Contents

- [Overview](#overview)
- [The Problem](#the-problem)
- [How It Works](#how-it-works)
- [Key Features](#key-features)
- [Architecture](#architecture)
- [Demo](#demo)
- [Installation](#installation)
- [Usage](#usage)
- [API Documentation](#api-documentation)
- [Contributing](#contributing)
- [License](#license)

## 🎯 Overview

**Neo Trade** is a revolutionary copy trading platform built on the Aptos blockchain that simplifies cryptocurrency trading for both beginners and experienced traders. Our platform combines a modern web interface with an intelligent Telegram bot to provide seamless copy trading experiences.

<div align="center">
  <img src="img/1.png" alt="Project Overview" width="600"/>
</div>

### 🎯 Mission
**Copy Trading Simplified on Aptos** - Making profitable trading accessible to everyone through AI-powered automation and real-time portfolio analytics.

## ❌ The Problem

Traditional copy trading comes with significant challenges:

<div align="center">
  <img src="img/2.png" alt="Copy Trading Challenges" width="600"/>
</div>

- **High Barriers to Entry**: Requires time, skills, and experience
- **Financial Risk**: Inexperienced users often lose money or miss opportunities
- **Complex Solutions**: Existing copy trading platforms have complicated setup and expensive fees
- **Manual Process**: Users need to manually approve every trade
- **Limited Analytics**: Lack of comprehensive portfolio insights

## ⚙️ How It Works

Our platform operates through a three-step process that makes copy trading effortless:

<div align="center">
  <img src="img/3.png" alt="How Neo Trade Works" width="600"/>
</div>

### 1. **Top Wallets on UI**
- Get the top traders/wallet addresses listed on our web interface
- Easy reference for users to pick whom to copy for trading
- Real-time performance metrics and PnL tracking

### 2. **Copy Trading on Telegram**
- Once users pick the best wallet, they're redirected to our Telegram bot
- Simple activation process through an intuitive chat interface
- No additional app downloads required

### 3. **The BOT's Magic**
- Continuous monitoring of swaps/trades from the master wallet
- Automatic trade replication without user approval
- AI-powered risk management and execution

## ✨ Key Features

<div align="center">
  <img src="img/4.png" alt="Key Features" width="600"/>
</div>

### 🔄 **Copy Trading**
- Mirror master trades in real-time
- Automated execution with your wallet
- No manual approval required

### 📱 **Telegram Integration**
- Easy to use, no extra app needed
- Intuitive chat-based interface
- Instant notifications for all activities

### 📊 **Portfolio Insights**
- Comprehensive holdings overview
- Real-time profit/loss tracking
- Detailed trade volume analytics

### 🏆 **Top Traders Leaderboard**
- Discover the best performing traders
- Performance metrics and rankings
- Easy trader selection process

### ⚡ **Aptos-Powered**
- Fast, low fees, secure blockchain
- Optimized for Aptos ecosystem
- Lightning-fast transactions

### 🤖 **AI-Powered Features**
- Intelligent trade replication
- Risk management protocols
- Automated execution optimization

## 🏗️ Architecture

### System Overview

```
┌─────────────────┐    ┌─────────────────┐    ┌─────────────────┐
│   Frontend      │    │   Telegram Bot  │    │   Aptos Chain   │
│   (React)       │    │   (Node.js)     │    │   (Blockchain)  │
├─────────────────┤    ├─────────────────┤    ├─────────────────┤
│ • Leaderboard   │    │ • User Mgmt     │    │ • Transactions  │
│ • Analytics     │◄──►│ • Copy Trading  │◄──►│ • Smart Contracts│
│ • Trader Search │    │ • Notifications │    │ • Token Swaps   │
└─────────────────┘    └─────────────────┘    └─────────────────┘
         │                       │                       │
         └───────────────────────┼───────────────────────┘
                                 │
                    ┌─────────────────┐
                    │   Database      │
                    │   (PostgreSQL)  │
                    ├─────────────────┤
                    │ • User Data     │
                    │ • Wallet Info   │
                    │ • Trade History │
                    └─────────────────┘
```

### Technology Stack

#### Frontend
- **React 18** with TypeScript
- **Tailwind CSS** for styling
- **Vite** for build tooling
- **Axios** for API calls

#### Backend
- **Node.js** with ES modules
- **Telegraf** for Telegram bot
- **PostgreSQL** for data persistence
- **Aptos SDK** for blockchain interaction

#### Blockchain
- **Aptos** blockchain
- **Pontem LiquidSwap** for DEX integration
- **Smart contract** interactions

## 🎮 Demo

### Web Interface Demo

<div align="center">
  <img src="img/5.png" alt="Web Interface Demo" width="800"/>
</div>

Our web interface provides:
- **Aptos Trading Leaderboard**: Top performing traders ranked by PnL
- **Single Address Analysis**: Analyze any Aptos wallet for trading insights
- **Real-time Data**: Live updates on trader performance
- **Interactive Charts**: PnL trends and trade analytics

### Telegram Bot Demo

<div align="center">
  <img src="img/6.png" alt="Telegram Bot Interface" width="800"/>
</div>

The Telegram bot offers:
- **Wallet Management**: Create and manage multiple wallets
- **Portfolio Overview**: Comprehensive token holdings and balances
- **AI Copy Trading Setup**: Easy configuration of copy trading

### Copy Trading Flow

<div align="center">
  <img src="img/7.png" alt="Copy Trading Setup Flow" width="800"/>
</div>

The copy trading process:
1. **Setup**: Enter master trader's wallet address
2. **Confirmation**: Review trading information and risks
3. **Activation**: Start AI-powered copy trading

### Live Trading Demo

<div align="center">
  <img src="img/8.png" alt="Live Trading Demo" width="600"/>
</div>

Real-time copy trading features:
- **Active Monitoring**: AI continuously scans for new trades
- **Instant Execution**: Automatic trade replication
- **Trade Notifications**: Real-time updates on all activities
- **Risk Management**: Built-in safety protocols

## 🚀 Installation

### Prerequisites

- Node.js (v18 or higher)
- PostgreSQL database
- Telegram Bot Token
- Aptos wallet with testnet/mainnet access

### Frontend Setup

```bash
# Navigate to frontend directory
cd Frontend/start

# Install dependencies
npm install
# or
pnpm install

# Start development server
npm run dev
# or
pnpm dev
```

### Backend Setup

```bash
# Navigate to backend directory
cd TelegramBackend/copytrade

# Install dependencies
npm install
# or
pnpm install

# Create environment file
cp .env.example .env

# Configure environment variables
# TELEGRAM_BOT_TOKEN=your_bot_token
# DATABASE_URL=your_postgresql_url
# APTOS_NODE_URL=your_aptos_node_url

# Start the bot
npm start
# or
pnpm start
```

### Environment Variables

Create a `.env` file in the backend directory:

```env
# Telegram Bot Configuration
TELEGRAM_BOT_TOKEN=your_telegram_bot_token

# Database Configuration
DATABASE_URL=postgresql://username:password@localhost:5432/neotrade

# Aptos Configuration
APTOS_NODE_URL=https://fullnode.mainnet.aptoslabs.com
APTOS_FAUCET_URL=https://faucet.mainnet.aptoslabs.com

# Optional: For development
NODE_ENV=development
```

## 📖 Usage

### Web Interface

1. **Access the Leaderboard**
   - Visit the web interface
   - View top-performing Aptos traders
   - Click on any trader for detailed analysis

2. **Analyze Single Address**
   - Enter any Aptos wallet address
   - Get comprehensive trading insights
   - View PnL trends and trade history

3. **Copy Trading Setup**
   - Click "Copy Trade" on any trader
   - Get redirected to Telegram bot
   - Follow the setup process

### Telegram Bot

1. **Start the Bot**
   ```
   /start
   ```

2. **Manage Wallets**
   ```
   /wallets
   ```

3. **Setup Copy Trading**
   - Navigate to "AI Copy Trading"
   - Enter master trader's wallet address
   - Confirm and activate

4. **Monitor Portfolio**
   - View real-time portfolio updates
   - Track PnL and trade history
   - Manage multiple wallets

## 📚 API Documentation

### Frontend API

The frontend uses the Aptos API to fetch trading data:

```typescript
// Fetch trader statistics
const stats = await calculateTraderStats(address, transactions);

// Get multiple traders
const traders = await fetchMultipleTraders(addresses);

// Analyze trader performance
const analysis = await getTraderAnalysis(address);
```

### Backend API

The Telegram bot provides these key functions:

```javascript
// Wallet management
await createNewWallet(telegramId);
await getPortfolioSummary(telegramId);

// Copy trading
await addCopyTrading(telegramId, masterWallet);
await startCopyTradingForUser(masterWallet, userPrivateKey, telegramId);
```

## 🤝 Contributing

We welcome contributions! Please follow these steps:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

### Development Guidelines

- Follow TypeScript best practices
- Write comprehensive tests
- Update documentation for new features
- Follow the existing code style

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🔗 Links

- **Website**: [Coming Soon]
- **Telegram Bot**: [@NeoTradeBot](https://t.me/NeoTradeBot)
- **Documentation**: [Coming Soon]
- **Discord**: [Coming Soon]

## 🙏 Acknowledgments

- Aptos Labs for the amazing blockchain infrastructure
- Pontem for LiquidSwap DEX integration
- The open-source community for various libraries and tools

---

<div align="center">
  <p>Built with ❤️ for the Aptos ecosystem</p>
  <p>© 2024 Neo Trade. All rights reserved.</p>
</div>
