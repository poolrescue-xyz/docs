---
icon: scroll
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

# Changelog

## Changelog

Track the main releases and improvements of PoolRescue.<br>

***

#### **v1.4.1 — “Sharable Links & New Protocols”**

📅 December 2025

* Added direct shareable links for chains, protocols, and pools to make sharing and support easier.
* Removed an unnecessary API call related to USD value calculation
* Added support for the following protocols:
  *   **BSC:** FstSwap, EmpireDex, KaoyaSwap, BabySwap, GIBXSwap, Titano Swych, PinkSwap, BearnFi

      **Avalanche:** EmpireDex

      **Ethereum:** EmpireDex, Unicly v2, Unicly v1

      **Polygon:** EmpireDex

      **Base:** BaseSwap

      **opBNB:** LuigiSwap

***

#### **v1.4 — “Feedbacks & Analytic Dashboard”**

📅 December 2025

* Based on user feedback, we added USD value display for positions.
* After a user reported issues when scanning many pools, we added a recommendation to stay below 100 pools for optimal performance.
* Added a direct link to the Dune Analytics Dashboard.

#### **v1.3 — “Improvements & more Scroll Protocols”**

📅 November 2025

* Improved Search function
* Added support for the following Protocols:\
  **Scroll:** Asteria, BallExchange, ChiliSwap, ChimeraDex, IvySwap, LuigiSwap, PapyrusSwap, PixelSwap, QuillSwap, Sanctuary, ScrollSwap, Scrollswap Finance, VoltageSwap

***

#### **v1.2 — “Improvements & New Protocols”**

📅 November 2025

* Improved Calls and Search
* Improved Wallet Connection
* Removed Pools with 0 Supply / 0 Holders
* Added support for 63 new Protocols

***

#### **v1.1.1 — “Links & New Protocols”**

📅 October 2025

* Added links for Docs and X(Twitter)
* Added support for:
  * **Linea:** Secta
  * **Arbitrum:** Auragi
  * **Polgyon:** Pearl

***

#### **v1.1 — “Uniswap V2 Support”**

📅 October 2025

* Introduced updated adapter logic for Uniswap v2 protocols
* Unified contract version `PoolRescueV1` across all supported chains
* Improved mobile-friendly UI layout
* Added support for:
  * **Ethereum:** Hope, CCSwap
  * **BSC:** CCSwap
  * **opBNB:** Thena
  * **Arbitrum:** Ramses

***

#### **v1.0 — “Initial Alpha”**

📅 October 2025

* First public alpha release of PoolRescue
* Supported **Scroll (Tokan, Skydrome)** and **Mantle (Stratum)**
* Introduced adapter for Solidly-style protocols
* Implemented wallet scan, claim, and withdraw flow
* Integrated **2.5% infrastructure fee logic**
