---
icon: display-code
layout:
  width: default
  title:
    visible: true
  description:
    visible: true
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: true
  metadata:
    visible: true
---

# Technical Overview

## Technical Overview

PoolRescue is a lightweight, non-custodial tool that helps users locate and recover stranded or migrated liquidity positions (LPs) across multiple EVM chains.\
It runs entirely client-side — no backend, no indexing layer, and no stored user data.

***

#### ⚙️ System Architecture

```
User Wallet (MetaMask, Rabby, etc.)
          │
          ▼
Frontend App (poolrescue.xyz)
          │
          ├── Loads Protocol JSON Files (chain & protocol definitions)
          │
          ├── Runs Adapter Logic (JavaScript + Ethers.js)
          │
          ▼
PoolRescueV1 Contract (deployed per chain)
          │
          ▼
DEX & Gauge Contracts (e.g. Skydrome, Tokan, Stratum)
```

#### 🧱 Components

**Frontend (UI)**

* Fully client-side HTML + JavaScript application.
* Uses Ethers.js to communicate directly with each chain’s RPC endpoint.
* Handles wallet connection, scanning, and transaction execution.
* Hosted on the **official PoolRescue infrastructure** — no external hosting, no data collection.

**Protocol JSON Files**

Each supported protocol is defined in a JSON file containing:

* Protocol name
* Pair and gauge addresses
* Token0 / Token1 (address, symbol, decimals)
* Stability flag (`true` or `false`)

This modular structure allows rapid protocol onboarding without redeploying contracts or maintaining a backend.

**Adapter Logic**

* JavaScript modules interpret JSON definitions and execute RPC reads.
* Detect LP balances in both wallet and gauge contracts.
* Perform claim, withdraw, and remove-liquidity actions directly through the connected wallet.
* Unified logic for **Solidly-style** and **Uniswap v2** protocols.

**Smart Contract — PoolRescueV1**

* Minimal helper contract deployed per chain.
* Handles transaction routing and the **2.5% infrastructure fee**.
* No upgradeability, no admin control, no stored state.
* Verified on most supported explorers (see Contracts & Security).

***

#### 🔐 Security Model

* **Non-custodial:** PoolRescue never holds funds or private keys.
* **Transparent:** All addresses, ABIs, and logic are public on GitHub.
* **Direct execution:** Every transaction originates from the connected wallet.
* **Minimal surface:** No backend, database, or user tracking.
* **Verified contracts:** Published and verified on multiple chain explorers.

***

#### 🧭 Future Focus

* Support for **Concentrated Liquidity (v3)** pools.
* Integration of more protocols
* Optimized RPC batching&#x20;
* Extended analytics view for LP holders
