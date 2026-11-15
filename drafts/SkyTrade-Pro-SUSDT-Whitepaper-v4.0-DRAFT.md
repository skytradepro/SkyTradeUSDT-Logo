<p align="center">
  <img src="../Logo.png" alt="SkyTrade Pro" width="120" />
</p>

<h1 align="center">SkyTrade Pro Ecosystem Whitepaper</h1>

<p align="center"><strong>Version 4.0 — DRAFT FOR INTERNAL REVIEW</strong><br/>
<strong>Not for publication.</strong> Supersedes v3.1 (Final) upon official release only.</p>

<p align="center">
  <img src="https://img.shields.io/badge/SUSDT-BNB%20Chain-yellow" />
  <img src="https://img.shields.io/badge/SKYX-SkyX%20Mainnet-blue" />
  <img src="https://img.shields.io/badge/Bridge-LIVE-green" />
</p>

---

## Document Control

| Field | Value |
|---|---|
| Project | SkyTrade Pro |
| Primary utility token | SUSDT (BEP-20 on BNB Smart Chain) |
| Network native asset | SKYX (Cosmos SDK chain `skyxnew`) |
| BSC contract | `0x1f891D25A386e6F67ead37d9BFAf5C444213a134` |
| Website | https://pro.skytradepro.com |
| Repository | https://github.com/skytradepro/skyx-network |
| Contact | admin@skytradepro.com |

---

## 1. Executive Summary

SkyTrade Pro is a transparent digital-asset ecosystem combining a **utility token (SUSDT)** on **BNB Smart Chain (BEP-20)** with **SkyX Network**, an operational **Cosmos SDK proof-of-stake mainnet** that provides staking, governance, and cross-chain settlement for ecosystem assets.

The project’s mission is to deliver professional-grade trading infrastructure, on-chain verifiability, and sustainable growth without misleading market tactics. SkyTrade Pro emphasizes **organic liquidity**, **public audits**, **identified leadership**, and **long-horizon utility** over short-term speculation.

**Status snapshot (November 2026)**

| Capability | Status |
|---|---|
| SUSDT on BNB Smart Chain | **LIVE** |
| SkyX Network mainnet (`skyxnew`) | **LIVE** |
| SkyX v2-tokenomics upgrade (block 3,708,000) | **COMPLETED** |
| BSC ↔ SkyX SUSDT bridge | **LIVE** |
| Public explorer & open documentation | **LIVE** |
| SKYX staking & on-chain governance | **LIVE** |
| Fixed 7% SKYX annual inflation | **LIVE** |
| EVM execution environment on SkyX mainnet | **IN TESTING** (isolated environments only) |
| EVM on SkyX mainnet (production) | **PLANNED** (technical review + governance) |

SUSDT remains the canonical ecosystem utility token for platform access, trading benefits, rewards, and bridge portability. SKYX is the native gas, staking, and governance coin securing SkyX Network.

---

## 2. Legal Disclaimer

SkyTrade Pro (**SUSDT**) and **SKYX** are digital utility assets intended for use within the SkyTrade Pro and SkyX Network ecosystems. **They do not represent equity, ownership interests, debt, or securities** in any jurisdiction.

This whitepaper is provided for **informational purposes only** and does not constitute financial, legal, tax, or investment advice. Participation in blockchain networks involves substantial risk, including total loss of funds.

No statement herein guarantees returns, listings, partnerships, or future performance. Regulatory treatment of digital assets varies globally and may change without notice.

NFT products referenced by the project are **utility/access instruments**, not investment contracts, unless expressly stated otherwise in separate legal terms. Participation in NFT programs does not guarantee financial return.

**DRAFT NOTICE:** Version 4.0 is a workspace draft. It must not be published, linked from the production website, or presented to investors until SkyTrade Pro leadership approves all figures marked for verification.

---

## 3. Ecosystem Overview

### 3.1 Vision

SkyTrade Pro integrates decentralized trading tools with a dedicated application chain (SkyX) so users can:

- Hold and transfer **SUSDT** on BNB Smart Chain with public audit and KYC verification.
- Move **SUSDT** to SkyX through an official bridge for ecosystem applications.
- Stake **SKYX**, participate in **governance**, and benefit from transparent inflation parameters.
- Access trading dashboards, community channels, and planned mobile and DeFi extensions.

### 3.2 Architecture (High Level)

```
                    ┌─────────────────────────────┐
                    │   SkyTrade Pro Platform     │
                    │   (Web / future mobile)     │
                    └─────────────┬───────────────┘
                                  │
          ┌───────────────────────┼───────────────────────┐
          │                       │                       │
          ▼                       ▼                       ▼
   ┌──────────────┐      ┌──────────────┐       ┌──────────────┐
   │ SUSDT BEP-20 │◄────►│  SkyX Bridge │◄─────►│  SUSDT on    │
   │  BNB Chain   │      │  (official)  │       │  SkyX        │
   └──────────────┘      └──────┬───────┘       └──────────────┘
                                │
                                ▼
                    ┌─────────────────────────────┐
                    │   SkyX Network (skyxnew)    │
                    │   SKYX gas · staking · gov  │
                    │   Cosmos SDK + CometBFT     │
                    └─────────────────────────────┘
```

Bridge UI: https://bridge.skytradepro.com/

---

## 4. SUSDT — BNB Smart Chain Utility Token

### 4.1 Token Profile

| Attribute | Value |
|---|---|
| Name | SkyTrade Pro |
| Symbol | SUSDT |
| Network | BNB Smart Chain (BEP-20) |
| Decimals | 18 |
| Contract | `0x1f891D25A386e6F67ead37d9BFAf5C444213a134` |
| Explorer | https://bscscan.com/token/0x1f891d25a386e6f67ead37d9bfaf5c444213a134 |

### 4.2 Supply and Distribution

**Design maximum supply (narrative, v3.x family):** **1,000,000,000 SUSDT**.

The v3.1 whitepaper described an initial allocation model:

| Bucket | % (design model) |
|---|---|
| Liquidity pool | 40% |
| Burned (permanent) | 30% |
| Ecosystem & rewards | 15% |
| Team & development (multisig) | 10% |
| Marketing & partnerships | 5% |

**Important:** Live on-chain holder distribution evolves with trading, liquidity, burns, and treasury movements. Public analytics (including [Cyberscope](https://www.cyberscope.io/audits/susdt?slug=susdt) and BscScan holder charts) have reported a **very large proportion of supply** associated with the standard burn address `0x000000000000000000000000000000000000dead`, which **may not match** the historical “30% burned” figure in v3.0/v3.1 documents.

**`[NEEDS USER VERIFICATION]`** — SkyTrade must confirm the authoritative burn percentage, transaction references, and whether v4.0 should publish the design table, a current snapshot, or narrative-only supply disclosure.

**On-chain transparency links**

- Token balances: https://bscscan.com/token/0x1f891d25a386e6f67ead37d9bfaf5c444213a134#balances  
- Holder distribution: https://bscscan.com/token/tokenholderchart/0x1f891d25a386e6f67ead37d9bfaf5c444213a134  
- Burn address view: https://bscscan.com/token/0x1f891d25a386e6f67ead37d9bfaf5c444213a134?a=0x000000000000000000000000000000000000dead  

### 4.3 Liquidity and Market Integrity

| Item | Status |
|---|---|
| PancakeSwap V2 liquidity | **LIVE** |
| Official pool (GeckoTerminal) | https://www.geckoterminal.com/bsc/pools/0xfd18da0e5d05dae2ddb3e711e7e77ef2d553367c |
| Swap link | https://pancakeswap.finance/swap?outputCurrency=0x1f891D25A386e6F67ead37d9BFAf5C444213a134 |
| Liquidity lock (DxLock) | **LIVE** — certificate referenced in project README |

**Primary liquidity locker (workspace + v3.1 PDF):**

- Certificate: https://www.dx.app/certificates/locker/v2-liquidity?address=0xA116A1325bf888E79ECFcB832c9C91655233a18a&chain=56  
- Locker view: https://www.dx.app/dxlock/view/liquidity-locker?address=0xA116A1325bf888E79ECFcB832c9C91655233a18a&chain=56  

v3.1 states lock duration **until 2027**. **`[NEEDS USER VERIFICATION]`** — confirm locked amount and exact unlock timestamp for investor-facing text.

**Note:** The older web whitepaper v3.0 cited a different locker address (`0xA7391aAe496F8D99e09C0941EDf038DF9a3E4978`). v4.0 follows v3.1/README unless leadership confirms migration details.

### 4.4 Security, Audit, and KYC

| Control | Status |
|---|---|
| Cyberscope smart contract audit | **COMPLETED** — https://www.cyberscope.io/audits/susdt?slug=susdt |
| Cyberscope KYC | **COMPLETED** |
| Contract verification on BscScan | **LIVE** |
| Ownership renounced (per audit vendor data) | Reported on Cyberscope — **`[NEEDS USER VERIFICATION]`** for legal wording |
| Multisig treasury | Claimed in v3.1 — **`[NEEDS USER VERIFICATION]`** (address, threshold, policy) |

The project does **not** rely on undisclosed security vendors. Names appearing only in web v3.0 (“CertSecure,” “EUROK Security Ltd.”) are **excluded** from v4.0 pending evidence.

### 4.5 SUSDT Utility (Use Cases)

SUSDT is a **utility token**, not a security.

| Use case | Status |
|---|---|
| Platform access and trading tools | **LIVE** / expanding |
| Fee benefits within SkyTrade Pro | **PLANNED** / partial — feature-dependent |
| Ecosystem incentives | **IN PROGRESS** |
| Bridge portability BSC ↔ SkyX | **LIVE** |
| SUSDT staking on BSC | **PLANNED** |
| Community governance tied to SUSDT | **PLANNED** |
| NFT-based membership (OpenSea collection) | **LIVE** collection; utility depth **PLANNED** |

NFT collection: https://opensea.io/collection/skytrade-pro-access-nft

---

## 5. SkyX Network

### 5.1 Network Profile

SkyX Network (`skyxnew`) is a **Cosmos SDK** blockchain using **CometBFT** consensus, standard Cosmos modules (bank, staking, distribution, mint, gov, upgrade, IBC), and public infrastructure operated for the SkyTrade Pro ecosystem.

| Field | Value |
|---|---|
| Chain ID | `skyxnew` |
| Network type | Mainnet |
| Genesis | 2026-03-21T20:16:58Z |
| Address prefix | `cosmos` |
| SKYX decimals (SkyX) | 6 |
| SUSDT decimals (SkyX) | 6 (18 on BSC; bridge normalizes units) |

**Public endpoints**

| Service | URL |
|---|---|
| RPC | https://skyxnew-rpc.skytradepro.com |
| REST / LCD | https://skyxnew-api.skytradepro.com |
| Explorer | https://skyxnew-explorer.skytradepro.com/skyxnew |
| Bridge | https://bridge.skytradepro.com/ |

Full parameters: [docs/NETWORK.md](https://github.com/skytradepro/skyx-network/blob/main/docs/NETWORK.md)

### 5.2 SKYX — Native Asset

SKYX (`skyx` base denom) is used for:

- Transaction fees (**LIVE**)
- Validator staking and delegations (**LIVE**)
- On-chain governance voting (**LIVE**)
- Inflation participation for stakers (**LIVE**)

### 5.3 v2-Tokenomics Upgrade — **COMPLETED**

At block height **3,708,000** (14 November 2026), governance proposal **#1** (`v2-tokenomics`, expedited) executed an on-chain upgrade that:

1. Minted **1,000,000 SKYX** to five designated ecosystem wallets (amounts at upgrade height).
2. Minted **100,000 SUSDT** to **SkyX-Reserve** as **bridge inventory** (not current operational balance).
3. Reduced maximum inflation to **7%** and aligned min/max inflation to a **fixed 7% annual rate**.
4. Registered denom metadata for SKYX and SUSDT on-chain.

Source: [UPGRADE-LOG.md](https://github.com/skytradepro/skyx-network/blob/main/docs/upgrades/UPGRADE-LOG.md)

#### SKYX allocation at upgrade height (public)

| Wallet role | Address | SKYX (display) |
|---|---|---:|
| SkyX-Staking | `cosmos12rymnv2g466pq80jqs4rq3tsyn62y8mt0rm7pw` | 400,000 |
| SkyX-Treasury | `cosmos1lv0h9n4u87gchjs8y82gtunkzeuhgdz3sr4498` | 250,000 |
| SkyX-Reserve | `cosmos13rprrdyegfwx7lhuwv2d58dlk62356ffd2cmre` | 150,000 |
| SkyX-Team | `cosmos1589s6m6edem5zyughf2xcrajkzznl07v0rtftn` | 100,000 |
| SkyX-Risk | `cosmos1ek3twjhw9pkgu4s3s0h2rglpjcnqd7td695qul` | 100,000 |
| **Total** | | **1,000,000** |

Current wallet balances may differ due to transfers, staking delegations, and fees. Verify via explorer — **do not treat this table as a live balance sheet**.

#### Inflation — **LIVE**

| Parameter | Value (verified via public API, Nov 2026) |
|---|---|
| `inflation` | 0.07 (7%) |
| `inflation_min` | 0.07 |
| `inflation_max` | 0.07 |

New SKYX from inflation is distributed per Cosmos SDK `mint` and `distribution` modules to validators and delegators.

### 5.4 Staking and Governance — **LIVE**

| Parameter | Value |
|---|---|
| Bond denom | `skyx` |
| Unbonding period | 21 days |
| Governance | On-chain proposals (e.g. proposal #1 passed for v2-tokenomics) |

Staking allocations at upgrade were documented in [docs/TOKENOMICS.md](https://github.com/skytradepro/skyx-network/blob/main/docs/TOKENOMICS.md). Validator set and delegation figures change over time.

### 5.5 SUSDT on SkyX

SUSDT on SkyX is the same economic asset as BEP-20 SUSDT with bridge-controlled supply on SkyX. The upgrade minted **100,000 SUSDT** to SkyX-Reserve as **initial bridge inventory**; user deliveries are handled by the bridge relayer when SUSDT is locked on BSC.

| Item | Value |
|---|---|
| BSC SUSDT contract | `0x1f891D25A386e6F67ead37d9BFAf5C444213a134` |
| BSC bridge contract | `0x15d803E9c7A660F3972f279a63cD4e897bD410AF` |
| Bridge app | https://bridge.skytradepro.com/ |

**Security note:** This document intentionally omits **live reserve balances**, relayer balances, and internal operational limits.

---

## 6. Cross-Chain Bridge — **LIVE**

The SkyX Bridge enables users to move **SUSDT** between BNB Smart Chain and SkyX through the official web interface. The bridge converts decimal representations (18 on BSC, 6 on SkyX) while preserving 1:1 economic intent.

Users must verify recipient addresses, chain selection, and transaction confirmations on both BscScan and the SkyX explorer.

---

## 7. EVM Integration — **IN TESTING**

SkyTrade Pro is pursuing **broad EVM compatibility** to expand developer tooling and wallet support on SkyX Network.

| Scope | Status |
|---|---|
| EVM execution in isolated test environments | **IN TESTING** — reported successful |
| EVM on SkyX mainnet | **PLANNED** — requires further testing, technical review, and governance approval |
| Individual wallet compatibility claims on mainnet | **Not stated** — no mainnet wallet certification claimed in v4.0 |

---

## 8. Platform and Market Approach

### 8.1 Trading Platform

SkyTrade Pro provides a web trading dashboard and supporting documentation:

- Platform: https://pro.skytradepro.com/trading

### 8.2 Market Listings and Tracking

| Resource | Status |
|---|---|
| CoinMarketCap | **LIVE** — https://coinmarketcap.com/currencies/skytrade-pro/ |
| CoinGecko | Listed (see official links in GitHub README) |
| Azbit IEO (historical) | **COMPLETED** per project materials |
| Tier-1 CEX listings | **PLANNED** |

### 8.3 Market Conduct Principles

SkyTrade Pro states a policy of **no wash trading**, **no artificial volume**, and **no price manipulation**. Trading activity is intended to be organic and verifiable on-chain.

---

## 9. Roadmap

Roadmap items use explicit status labels: **LIVE**, **COMPLETED**, **IN TESTING**, **PLANNED**.

### Phase A — Foundation (**COMPLETED**)

- BEP-20 deployment and BscScan verification  
- Initial branding, website, PancakeSwap liquidity  
- Cyberscope audit and KYC  
- Public GitHub and documentation  

### Phase B — Visibility (**LIVE** / **IN PROGRESS**)

- CoinMarketCap listing — **LIVE**  
- Community growth — **IN PROGRESS**  
- Metadata and explorer consistency — **IN PROGRESS**  

### Phase C — SkyX Mainnet (**COMPLETED** / **LIVE**)

- Cosmos SDK mainnet launch — **LIVE**  
- Public RPC, LCD, explorer — **LIVE**  
- v2-tokenomics upgrade @ 3,708,000 — **COMPLETED**  
- SKYX staking & governance — **LIVE**  
- 7% fixed inflation — **LIVE**  

### Phase D — Interoperability (**LIVE** / **IN TESTING**)

- BSC ↔ SkyX SUSDT bridge — **LIVE**  
- SkyX-Reserve SUSDT inventory mint (100,000 at upgrade) — **COMPLETED**  
- EVM integration testing — **IN TESTING**  
- EVM on mainnet — **PLANNED**  

### Phase E — Product Expansion (**PLANNED** / **IN PROGRESS**)

- Mobile dApp — **PLANNED** **[NEEDS USER VERIFICATION]**  
- SUSDT staking on BSC — **PLANNED**  
- Expanded DeFi and copy-trading modules — **PLANNED**  
- Wallet compatibility program — **PLANNED**  
- Developer tools & ecosystem integrations — **PLANNED**  
- Tier-1 exchange preparation — **PLANNED**  
- NFT utility depth — **IN PROGRESS**  

### Phase F — Adoption (**PLANNED**)

- SUSDT adoption in platform payments and partner integrations  
- Governance-driven parameter and feature upgrades  
- Global community and compliance alignment  

---

## 10. Team and Governance

### 10.1 Leadership and Core Team

SkyTrade Pro is led by a publicly identified team. Extended bios are available on the official about page: https://pro.skytradepro.com/about

| Name | Role |
|---|---|
| Ramzi Sahbani | Founder & Project Lead |
| Selim Uzun | Business Development & Partnerships Lead |
| Hafeth Malaoui | Blockchain Development Lead |
| Hajar Hammam | Marketing & Community Director |
| Aziz Annabi | Product, Digital & PR Lead |
| Hamdi Ghaleb | Marketing & Community Director |
| Lina Valova | Legal & Compliance Advisor |

**Founder profile (v3.x):** https://www.linkedin.com/in/ramzi-sahbani-8a8ba8268/

### 10.2 Network Governance

SkyX Network protocol changes require **on-chain governance** by SKYX stakers. Material upgrades (including tokenomics) follow Cosmos SDK upgrade mechanics, as demonstrated by **v2-tokenomics**.

---

## 11. Risk Factors

Participants should consider risks including but not limited to:

- **Market volatility** and illiquidity in early-stage tokens  
- **Smart contract and bridge** vulnerabilities despite audits  
- **Validator and slashing** risk when staking SKYX  
- **Regulatory change** affecting digital assets, staking, or bridges  
- **Cross-chain** transaction failure, delays, or user error  
- **Governance outcomes** that may alter inflation, fees, or upgrades  
- **Technology immaturity** of EVM integration while **IN TESTING**  
- **Operational dependency** on public infrastructure endpoints  

Conduct independent research before acquiring, staking, bridging, or using ecosystem tokens.

---

## 12. Official Resources

| Resource | URL |
|---|---|
| Website | https://pro.skytradepro.com |
| SkyX GitHub | https://github.com/skytradepro/skyx-network |
| Bridge | https://bridge.skytradepro.com/ |
| SkyX Explorer | https://skyxnew-explorer.skytradepro.com/skyxnew |
| Telegram | https://t.me/skytradeproteam |
| X | https://x.com/SkytradeproSKYX |
| Support | https://skytradepro-help.freshdesk.com/ |
| Cyberscope Audit | https://www.cyberscope.io/audits/susdt?slug=susdt |

---

## 13. Document History

| Version | Notes |
|---|---|
| v3.0 | Web Google Doc (superseded) |
| v3.1 Final | 4-page PDF — BSC-centric narrative |
| **v4.0 DRAFT** | Adds SkyX mainnet, bridge, SKYX tokenomics, EVM testing status; flags unverified SUSDT supply figures |

Major updates will be announced through official channels after leadership approval.

---

**SkyTrade Pro Team**  
*Draft prepared November 2026 — for review only.*