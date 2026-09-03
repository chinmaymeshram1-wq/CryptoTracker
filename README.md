# VASP Attribution Intelligence Engine (VASP-AIE)
> **Automated Blockchain Intelligence & Virtual Asset Service Provider Attribution Platform**

Designed for **Law Enforcement Agencies (LEAs)**, Financial Intelligence Units (FIUs), and Cyber Crime Investigation Units to investigate unknown cryptocurrency wallets, trace fund layering flows, and automatically identify the nearest likely Virtual Asset Service Provider (VASP), centralized exchange, custodial wallet provider, or deposit wallet cluster.

---

## 🏛️ System Overview

The **VASP Attribution Intelligence Engine** is a specialized cyber forensics platform structured specifically for investigative rigor. Unlike retail cryptocurrency explorers or trading dashboards, VASP-AIE enforces strict segregation between:
- **FACT** (Confirmed on-chain transactions, timestamped ledger entries)
- **INFERENCE** (Graph proximity, clustering heuristics, temporal velocity)
- **AUTOMATED ATTRIBUTION** (Algorithmic probabilistic matching)
- **INVESTIGATOR VERIFICATION** (Manual validation required before judicial filing)

---

## 🚀 Key Features

1. **Law Enforcement Intelligence Dashboard**
   - Live KPI overview (Active Investigations, Wallets Analyzed, VASPs Identified, High-Risk Wallets, Cross-Chain Movements, Pending Disclosure Requests)
   - Real-time incident alert stream and blockchain activity distribution

2. **Automated New Investigation Workflow**
   - 9-stage forensics pipeline simulation:
     1. Validating wallet address format
     2. Identifying blockchain network
     3. Fetching transaction history
     4. Building transaction graph
     5. Detecting intermediary layering wallets
     6. Identifying exchange clusters
     7. Querying VASP intelligence database
     8. Calculating attribution confidence score
     9. Generating forensic investigation dossier

3. **Automated VASP Attribution Engine**
   - 5-factor mathematical confidence scoring model:
     $$\text{Confidence} = (\text{Cluster Match} \times 30\%) + (\text{Deposit Rel.} \times 25\%) + (\text{Graph Prox.} \times 20\%) + (\text{Tx Pattern} \times 15\%) + (\text{Temporal Corr.} \times 10\%)$$
   - Ranked VASP identification with confidence classifications:
     - **90% – 100%**: Very High Match
     - **75% – 89%**: High Match
     - **50% – 74%**: Medium Match
     - **< 50%**: Low Match / Requires Further Tracing

4. **Interactive Transaction Graph**
   - Full interactive React Flow node & edge graph
   - Visualizes: `Suspect Wallet → Intermediary Wallets → Exchange Deposit Addresses → Exchange Cluster → VASP Hot Wallets`
   - Node-level intelligence drawer with transaction metrics, risk ratings, and address labels
   - Risk-weighted animated edges for high-risk flows

5. **Multi-Chain & Cross-Chain Intelligence**
   - Multi-chain monitoring: **Bitcoin, Ethereum, TRON, BNB Chain, Solana, Polygon**
   - Visual Cross-Chain flow tracker (`Source Chain → Bridge Protocol → DEX → Destination Chain → Centralized Exchange`)

6. **Comprehensive Risk Intelligence**
   - 0–100 weighted risk score with breakdown across:
     - Fraud Exposure (20%)
     - Ransomware Exposure (20%)
     - Darknet Exposure (15%)
     - Sanctions Exposure (15%)
     - High-Risk VASP Exposure (10%)
     - Mixer / Tumbler Exposure (10%)
     - Rapid Fund Movement / Velocity (5%)
     - Cross-Chain Layering Activity (5%)

7. **Lawful VASP Disclosure Request Generator**
   - Complete workflow to generate formal statutory disclosure requests under legal authorities (e.g. *Section 91 CrPC*, *PMLA 2002*, *18 U.S.C. § 2703*)
   - Supports request types: KYC Records, Account Details, Transaction Records, Wallet Ownership Verification, Asset Freeze Orders, Preservation Notices

8. **Investigation Report Generation**
   - One-click formal intelligence report compiler
   - Export options: PDF, JSON, CSV, and Print view with mandatory judicial disclaimers

9. **Live Global Search & RBAC Access Control**
   - Universal search across Case IDs, Wallets, Hashes, and VASPs
   - Role-Based Access Control matrix (*Administrator, Senior Investigator, Investigator, Analyst, Viewer*)
   - Immutable audit logging tracking all query and export actions

---

## 🛠️ Architecture & Tech Stack

```
vasp-intelligence/
├── src/
│   ├── app/
│   │   ├── (dashboard)/
│   │   │   ├── dashboard/          # Intelligence Dashboard
│   │   │   ├── investigations/     # Case workspace & details ([id])
│   │   │   ├── wallet/             # Deep wallet analysis
│   │   │   ├── graph/              # Interactive transaction graph
│   │   │   ├── vasp/               # Automated VASP attribution
│   │   │   ├── cross-chain/        # Cross-chain bridging intelligence
│   │   │   ├── risk/               # Risk scoring & gauge breakdown
│   │   │   ├── alerts/             # Automated alert monitoring
│   │   │   ├── reports/            # Forensic report generator
│   │   │   ├── api-integrations/   # Data feed health & API status
│   │   │   └── settings/           # RBAC & system audit logs
│   │   ├── api/                    # Modular API route handlers
│   │   ├── login/                  # Secure LEA authentication portal
│   │   ├── globals.css             # Government enterprise design tokens
│   │   └── layout.tsx
│   ├── components/
│   │   ├── layout/                 # Sidebar, Topbar with live global search
│   │   ├── ui/                     # Cards, Badges, Tabs, Modals, Gauges
│   │   ├── investigations/         # New investigation wizard
│   │   └── disclosure/             # Disclosure request modal
│   ├── services/                   # Typed Service Layer (Blockchain, VASP, Risk, etc.)
│   ├── data/                       # Synthetic LEA case data
│   ├── types/                      # Comprehensive TypeScript definitions
│   └── lib/                        # Formatting, risk, confidence helpers
```

---

## 💻 Running the Application

### 1. Install Dependencies
```bash
npm install
```

### 2. Run Development Server
```bash
npm run dev
```
Open [http://localhost:3000](http://localhost:3000) in your browser.

### 3. Sign In
Enter any Official ID (e.g. `LEA-IN-2024-7821`) and password to access the platform.

---

## ⚖️ Legal & Compliance Notice

> **DEMO / SYNTHETIC DATA ENVIRONMENT**
> All wallet addresses, transaction hashes, case identifiers, and incident descriptions in this software are synthetic simulations for investigative workflow demonstration and educational evaluation. Automated attribution scores are probabilistic intelligence indicators and must be verified by a qualified forensic analyst prior to judicial submission.
