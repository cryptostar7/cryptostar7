<div align="center">

# Carlo Sevilla

### AI Full-Stack Developer

*Building production AI systems — LLM agents, statistical analytics platforms,*  
*and full-stack applications with real machine learning at the core.*

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/carlosevilla)
[![Email](https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:sevillacarlo.dev@gmail.com)
[![Location](https://img.shields.io/badge/Philippines-Remote_Available-2E6B5E?style=for-the-badge&logo=googlemaps&logoColor=white)](#)

</div>

---

## What I Build

I design and ship end-to-end AI-powered systems — from the machine learning layer through the backend API to the frontend interface. My work sits at the intersection of **applied ML**, **LLM engineering**, and **decentralized infrastructure**.

Most recently I built **Subnet Sentinel**, a full-stack Bittensor intelligence platform covering 128 active subnets. It replaced hardcoded threshold alerts with a per-subnet statistical anomaly detection engine (z-score baselines, compound multi-metric detection, 4-tier severity taxonomy), added a RAG-based conversational AI agent with multi-turn session memory and tool-first groundedness, and a local LLM pipeline (Ollama + Qwen3 8B) for deep GitHub repository analysis — all without a GPU.

---

## Featured Projects

### 🔭 [Subnet Sentinel](https://github.com/cryptostar7/subnet-sentinel) — Bittensor Intelligence Platform
> Full-stack AI platform monitoring 128 Bittensor subnets in real time

- **Statistical anomaly detection** — per-subnet rolling baselines (mean, std, z-score, p10/p90) over 30-day snapshot history. Alerts only when a metric deviates from *that subnet's own* historical norm — not a global threshold
- **Compound anomaly detection** — fires a single high-confidence alert when ≥2 metrics deviate simultaneously (e.g. emission drops 3.1σ AND miner count drops 2.8σ)
- **RAG conversational agent** — Gemini + Chroma vector store, multi-turn session memory, SSE streaming, tool-first groundedness (no number stated without a live tool call backing it), freshness disclosure per answer
- **Local LLM pipeline** — map-reduce GitHub repository analysis using Ollama (Qwen3 8B, CPU-only): shallow-clone → filter high-signal files → per-file summarization → structured reduce into miner/validator requirement profiles
- **Hybrid LLM routing** — Ollama (local) for background summarization, Gemini for interactive chat — switchable per component via config
- **On-chain change detection** — tracks registration state, emission transitions, burn rate flips, miner/validator churn across all 128 subnets with deduplication
- **4-tier severity taxonomy** — LOW / MEDIUM / HIGH / NEWSLETTER with operational impact descriptions and `requires_action` flags

`Python` `FastAPI` `Next.js` `PostgreSQL` `Chroma` `Ollama` `Gemini API` `Bittensor SDK` `Docker` `APScheduler`

---

### 🛡️ [Tensorprox](https://github.com/shugo-labs/tensorprox) — Decentralized DDoS Detection (Bittensor SN91)
> ML-powered cybersecurity node deployed on the Bittensor network

- Sourced and engineered a DDoS traffic dataset from scratch (no existing dataset for this use case)
- Trained a **Random Forest classifier** reaching **98% classification accuracy** distinguishing malicious from normal traffic
- Built the full pipeline: synthetic attack-traffic generation → feature engineering → model training → live inference integration
- Deployed as a production miner node on Bittensor Subnet 91

`Python` `scikit-learn` `Random Forest` `AWS` `GCP` `Bittensor`

---

### 🤖 Bittensor ML Subnets — 7 Concurrent Deployments
> Applied ML systems across reinforcement learning, forecasting, and optimization

| Subnet | Type | Tech |
|--------|------|------|
| **Precog (SN55)** | Bitcoin price-prediction model | Time-series forecasting, ML |
| **Swarm (SN124)** | Autonomous drone flight agents | Stable Baselines3, PyTorch, JAX |
| **Sturdy (SN10)** | Yield optimization across DeFi protocols | Uniswap v3, Aave, Compound v3, Morpho |
| **Liquidity Auction (SN77)** | Voting system with Ed25519 signature verification | RESTful API, Token Economics |
| **SubVortex (SN7)** | Subtensor node infrastructure | Node Operations |
| **Investing (SN88)** | TAO/Alpha staking strategy design | Staking, Token Economics |

`Python` `PyTorch` `Stable Baselines3` `JAX` `scikit-learn` `Blockchain`

---

### 🏭 FactoryVerse — Smart Contract Architecture (2 yr, Full-Time)
> Solidity-based on-chain system for a GameFi ecosystem (Singapore)

- Architected **4 core smart contract modules** (Factory, Blueprint, Product, Custody) across **3 token standards** (ERC-20/721/1155)
- Built **FactoryGame**: NFT-synthesis platform with factory contract deployment system for modular, scalable asset creation
- Built **Stakeverses**: staking platform with reward formula design, staking/claiming/withdrawal contracts supporting **3 reward token types**
- Security-audited all contracts with Hardhat, Chai/Mocha, Sepolia testnet, and the **Aderyn** audit tool before deployment
- Web3 frontend: Ethers.js, Wagmi, RainbowKit, WalletConnect v2 for multi-wallet support

`Solidity` `ERC-20/721/1155` `Hardhat` `Aderyn` `TypeScript` `React` `Node.js` `GraphQL` `MongoDB`

---

### 🌐 Sinverse NFT Marketplace
> NFT marketplace with auction and royalty mechanics

- Built NFT collection and marketing contracts including auction and royalty mechanisms
- Concept announced at the Agora *"Celebrating NFT & DeFi"* event (June 2021)
- **Publicly launched on stage at GITEX Dubai** (Oct 2021) in front of a **1M+ audience**

`Solidity` `Web3.js` `React` `ERC-721`

---

## Technical Skills

### AI / Machine Learning
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=flat-square&logo=tensorflow&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white)
![OpenAI](https://img.shields.io/badge/OpenAI_API-412991?style=flat-square&logo=openai&logoColor=white)
![Google Gemini](https://img.shields.io/badge/Gemini_API-4285F4?style=flat-square&logo=google&logoColor=white)

**Techniques:** Random Forest · Reinforcement Learning (Stable Baselines3, JAX) · Time-Series Forecasting · Statistical Anomaly Detection (z-score, rolling baselines) · RAG · LLM Agent Orchestration · Prompt Engineering · NLP · Transformer-based Models · Local LLM (Ollama, Qwen3)

### Full-Stack
![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)

### Blockchain / Web3
![Solidity](https://img.shields.io/badge/Solidity-363636?style=flat-square&logo=solidity&logoColor=white)
![Ethereum](https://img.shields.io/badge/Ethereum-3C3C3D?style=flat-square&logo=ethereum&logoColor=white)
![Hardhat](https://img.shields.io/badge/Hardhat-F7DF1E?style=flat-square&logo=javascript&logoColor=black)

**Protocols:** ERC-20 / ERC-721 / ERC-1155 / ERC-4626 · DeFi · NFT · DAO · Bittensor · Wagmi · RainbowKit · WalletConnect v2

---

## Experience Timeline

```
2026 – Present  Subnet Sentinel (Personal Project) — AI platform engineer
2026 – Present  LiveSpan Network Inc. — Founding Engineer (edge computing platform)
2025 – 2026     Upwork — Freelance AI Full-Stack Developer
                  · BNB Tweet (OpenAI GPT pipeline, 3-format export)
                  · WealthLogix (Django, PDF generation, 100% accuracy)
2025            Bittensor — AI/ML Engineer (7 concurrent subnets)
2023 – 2025     FactoryVerse — Architecture Designer, Smart Contract Developer
2021 – 2023     TwistedResources — Web Developer
2020 – 2021     TwistedResources — Intern Web Developer
```

---

## Education & Recognition

🎓 **B.S. Computer Science** — Holy Angel University, Philippines (2017–2021)

🏆 **Champion, Dapp and Dash Campaign** — Forward, Rootstock on AlphaGuild (Nov–Dec 2023)

🎤 **GITEX Dubai Stage Launch** — Presented Sinverse Marketplace to 1M+ audience (Oct 2021)

---

<div align="center">

*Open to full-time and contract AI/full-stack engineering roles — remote*

**sevillacarlo.dev@gmail.com**

</div>
