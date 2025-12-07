# Qubic Quest 🔍

## AI-Powered Blockchain Analytics for the Qubic Network

---

![Main Interface](./main-interface.png)

## 🌟 Overview

Qubic Quest is an intelligent blockchain exploration platform that makes querying the Qubic blockchain as simple as having a conversation. Built with cutting-edge AI technology, Quest transforms complex blockchain data into accessible insights through natural language queries.

**Ask questions. Get answers. Explore the blockchain—naturally.**

---

## 📦 Projects

### [Quest App](https://github.com/qubic-quest/quest-app)

The main application—a Next.js-powered AI chat interface for exploring Qubic blockchain data.

**Features:**

- 🤖 ChatGPT-like conversational interface
- 🛠️ 17 specialized blockchain query tools
- 📊 Real-time price charts and market analytics
- 💼 Wallet portfolio tracking
- 🖼️ NFT marketplace visualization
- 🐋 Whale transaction monitoring
- 📈 DeFi protocol analytics (QX, QEARN, CCF, QBAY)

**Tech Stack:** Next.js 16, TypeScript, OpenAI GPT-4o-mini, Vercel AI SDK, Tailwind CSS

### [Quest Pipeline](https://github.com/qubic-quest/quest-pipeline)

The data infrastructure—a Python-based ETL pipeline that indexes and decodes Qubic blockchain data.

**Features:**

- 🔄 Automated data fetching every minute
- 🔍 Smart contract event decoding (QX, QEARN, CCF, QBAY)
- 💾 SQLite database with optimized schema
- 🚀 Production-ready with comprehensive error handling
- 📊 Data validation and quality checks

**Tech Stack:** Python 3.9+, better-sqlite3, Qubic RPC API

---

## 🎯 Why Quest?

Traditional blockchain explorers are complex, technical, and often overwhelming. Quest removes these barriers by:

✅ **Making blockchain data accessible** through natural language  
✅ **Providing instant insights** without SQL or technical knowledge  
✅ **Visualizing complex data** with beautiful, intuitive interfaces  
✅ **Combining historical and real-time data** for comprehensive analysis  
✅ **Supporting all major Qubic protocols** (QX, QEARN, CCF, QBAY)  

---

## 🚀 Quick Start

### 1. Set up the data pipeline

```bash
# Clone and set up the pipeline
git clone https://github.com/qubic-quest/quest-pipeline.git
cd quest-pipeline
pip install -r requirements.txt

# Run the pipeline
python pipeline.py
```

### 2. Launch the Quest app

```bash
# Clone and set up the app
git clone https://github.com/qubic-quest/quest-app.git
cd quest-app
npm install

# Configure environment
cp .env.example .env.local
# Add your OPENAI_API_KEY

# Start the app
npm run dev
```

Visit [http://localhost:3000](http://localhost:3000) and start exploring! 🎉

---

## 💡 Example Queries

Try asking Quest:

- "Show me recent transactions"
- "What's the current QUBIC price?"
- "Who are the top 10 holders?"
- "Show me CFB trading activity"
- "Compare QUTIL and GARTH performance"
- "What's in my wallet portfolio?"
- "Show me whale transactions over 10M QUBIC"
- "Show me recent QBAY NFT sales"
- "What are the latest CCF proposals?"

---

## 🏗️ Architecture

```txt
┌─────────────────────────────────────────────────┐
│                  Quest App                      │
│         (Next.js + AI Interface)                │
│  ┌──────────────────────────────────────────┐  │
│  │  Chat UI → AI Agent → Tool Selection     │  │
│  │         ↓                                 │  │
│  │  Database Queries + RPC Calls            │  │
│  │         ↓                                 │  │
│  │  Custom Visualizations                   │  │
│  └──────────────────────────────────────────┘  │
└───────────────────┬─────────────────────────────┘
                    │ Reads from
                    ↓
┌─────────────────────────────────────────────────┐
│              SQLite Database                    │
│         (Indexed Blockchain Data)               │
└───────────────────┬─────────────────────────────┘
                    │ Updated by
                    ↓
┌─────────────────────────────────────────────────┐
│             Quest Pipeline                      │
│      (Python ETL + Data Processing)             │
│  ┌──────────────────────────────────────────┐  │
│  │  Fetch → Decode → Transform → Load      │  │
│  │         ↓                                 │  │
│  │  Smart Contract Event Parsing           │  │
│  └──────────────────────────────────────────┘  │
└───────────────────┬─────────────────────────────┘
                    │ Fetches from
                    ↓
┌─────────────────────────────────────────────────┐
│           Qubic Blockchain                      │
│         (RPC + Archive Data)                    │
└─────────────────────────────────────────────────┘
```

---

## 🎨 Screenshots

**Main Interface:**
![Quest Interface](https://via.placeholder.com/800x450?text=Quest+Main+Interface)

**Asset Trading Analysis:**
![Trading Analysis](https://via.placeholder.com/800x450?text=Trading+Analysis)

**Wallet Portfolio:**
![Portfolio View](https://via.placeholder.com/800x450?text=Wallet+Portfolio)

**NFT Marketplace:**
![NFT Gallery](https://via.placeholder.com/800x450?text=NFT+Marketplace)

---

## 🛠️ Technology Stack

### Frontend (Quest App)

- **Framework:** Next.js 16 with App Router
- **Language:** TypeScript
- **AI:** OpenAI GPT-4o-mini + Vercel AI SDK
- **UI:** Tailwind CSS + shadcn/ui + Radix UI
- **Charts:** Recharts
- **Database Client:** better-sqlite3

### Backend (Quest Pipeline)

- **Language:** Python 3.9+
- **Database:** SQLite with optimized indexes
- **Data Source:** Qubic RPC API
- **Scheduling:** Built-in cron support

---

## 📊 Supported Protocols

### ✅ QX (Decentralized Exchange)

- Asset trading analytics
- Price discovery
- Volume tracking
- Portfolio management

### ✅ QEARN (Staking Protocol)

- Lock/unlock events
- Staking statistics
- Epoch tracking

### ✅ CCF (Community Fund)

- Governance proposals
- Voting activity
- Fund allocation tracking

### ✅ QBAY (NFT Marketplace)

- NFT minting and trading
- Collection analytics
- Trait breakdowns
- Ownership tracking

---

## 🌍 Use Cases

**For Investors:**

- Track wallet portfolios
- Monitor market trends
- Analyze whale movements
- View price charts and statistics

**For Traders:**

- Compare asset performance
- Monitor trading volumes
- Track buy/sell activity
- Get instant price quotes

**For NFT Collectors:**

- Browse marketplace activity
- View NFT metadata and traits
- Track collection values
- Discover new drops

**For Developers:**

- Query blockchain data without SQL
- Test wallet integrations
- Monitor smart contract activity
- Access comprehensive analytics

**For Researchers:**

- Analyze on-chain behavior
- Study protocol adoption
- Export data for analysis
- Track network metrics

---

## 🤝 Contributing

We welcome contributions from the community! Whether you're fixing bugs, adding features, or improving documentation, your help is appreciated.

### How to Contribute

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

---

## 📄 License

Both Quest App and Quest Pipeline are open source under the MIT License.

---

## 🔗 Links

- **Quest App:** [github.com/qubic-quest/quest-app](https://github.com/qubic-quest/quest-app)
- **Quest Pipeline:** [github.com/qubic-quest/quest-pipeline](https://github.com/qubic-quest/quest-pipeline)
- **Live Demo:** https://qubic-quest-xi.vercel.app/

---

## 💬 Community

Join the conversation and get support:

- **GitHub Discussions:** Share ideas and feedback
- **Issues:** Report bugs and request features

---

## 🙏 Acknowledgments

Built with ❤️ for the Qubic community.

Special thanks to:

- The Qubic core team for building an amazing blockchain
- The open-source community for incredible tools and libraries

---

Ready to explore? Start your Quest today! 🚀
