# MUBA 2026 Web3 Option Book Reader & AI Strategy Advisor (version 3.0)

An interactive Web3 application that streams real-time Ethereum Mainnet public blockchain data, connects to live option orderbook market quotes, and features an **AI Option Strategy & Risk Analysis Engine**.

Live Repository: [https://github.com/Xiwen1120/MUBA2026BlockChain](https://github.com/Xiwen1120/MUBA2026BlockChain)

---

## 🌟 Key Features & Hackathon Tracks

### 🏆 Qualified Tracks:
1. **Thetanuts Finance Track** (Live Option Book Orderbook & Vault Financial Model)
2. **AI x Options / AI + DeFi Track** (Client-side AI Options Risk Engine & Tactical Advisor)

---

## 🚀 Module Overview

1. **Section 01 · Live Public Blockchain Data Reader**:
   - **Auto-Connecting Public RPC**: Connects automatically to Ethereum Mainnet using a failover rotation array of 5 public JSON-RPC nodes (`publicnode.com`, `llamarpc.com`, `ankr.com`, `1rpc.io`, `cloudflare-eth.com`).
   - **Live Polling**: Automatically polls block numbers (~12s per block) and gas prices in Gwei.
   - **NUTS Token Contract Reader**: Reads real-time total supply and contract metadata for the official Thetanuts Governance Token (`0x23f3d4625aef6f0b84d50db1d53516e6015c0c9b`).
   - **Wallet Connection / Custom Address Reader**: Connects to MetaMask or allows manual input of any custom Ethereum address to read live ETH and NUTS balances.

2. **Section 02 · Financial Model & Payoff Calculator**:
   - **Live Option Book Integration**: Select from real-time option market contracts (e.g. `ETH-27SEP26-3400-C`, `ETH-27SEP26-3200-P`) with live strike prices, mark premiums, and IVs.
   - **Payoff Graph Visualizer**: Renders SVG payoff curves computed dynamically via $P\&L = \text{payoff} \times \text{size} - (\text{premium} \times \text{size} + \text{gas})$.

3. **Section 03 · Live Option Book Quotes & Market Depth**:
   - Displays real-time market depth including Mark Premium ($), Implied Volatility (IV %), and Best Bid / Best Ask spreads ($).

4. **Section 04 · AI Option Assistant & Strategy Advisor (AI x Options)**:
   - **AI Strategy Rating**: Evaluates contract parameters to generate ratings (`BULLISH CALL`, `BEARISH PUT`, `HIGH RISK`, `NEUTRAL SPREAD`).
   - **Est. Win Rate (POP %)**: Calculates Probability of Profit using normal distribution approximations.
   - **Risk / Reward Score**: Evaluates downside risk vs. premium and implied volatility.
   - **Interactive AI Prompt Assistant**: Users can trigger automated AI analysis for Risk, POP, and Strategy Optimization.

---

## 🛠️ Technology Stack

- **Frontend**: HTML5, Vanilla CSS, JavaScript (ES6+)
- **AI & Probability Engine**: Client-side option analytics & Black-Scholes Delta inference engine
- **Blockchain Libraries**: Ethers.js v5.7.2
- **Data Protocols & APIs**:
  - Ethereum Public JSON-RPC Nodes (Mainnet Chain ID 1)
  - Deribit Public Option Orderbook API
  - CoinGecko Price Feed API
- **Deployment**: Standalone static Web3 application (`Main.html`)

---

## 📄 Submission Metadata

- **Project Name**: MUBA 2026 Web3 Option Book Reader & AI Strategy Advisor
- **GitHub URL**: [https://github.com/Xiwen1120/MUBA2026BlockChain](https://github.com/Xiwen1120/MUBA2026BlockChain)
- **Primary File**: `Main.html`
