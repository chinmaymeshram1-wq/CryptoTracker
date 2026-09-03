# VASP Attribution Intelligence Engine (VASP-AIE)
## Comprehensive Technical & Implementation Documentation

**Subtitle:** Automated Blockchain Intelligence & Virtual Asset Service Provider Attribution Platform  
**Target Audience:** Law Enforcement Agencies (LEAs), Financial Intelligence Units (FIUs), Cyber Crime Investigation Units, Judicial Authorities  
**Classification:** DEMO / SYNTHETIC DATA ENVIRONMENT  

---

## 1. Executive Summary

The **VASP Attribution Intelligence Engine (VASP-AIE)** is an enterprise-grade cyber forensics and blockchain intelligence platform. It is engineered specifically for Law Enforcement Agencies to investigate unknown cryptocurrency wallets, de-anonymize complex fund-layering schemes, and automatically identify the nearest likely **Virtual Asset Service Provider (VASP)**, centralized exchange (CEX), custodial wallet service, or deposit cluster.

Unlike crypto-trading dashboards or retail block explorers, VASP-AIE is built with a **strict digital forensics design philosophy**:
- Clean, data-dense enterprise SOC/Forensics interface (no flashy crypto animations, price widgets, or trading charts).
- Strict legal segregation between **FACT** (on-chain confirmed transactions), **INFERENCE** (graph clustering & behavioral proximity), **AUTOMATED ATTRIBUTION** (probabilistic scoring), and **INVESTIGATOR VERIFICATION** (mandatory human validation before judicial filing).

---

## 2. Complete Features Implemented

### 🛡️ 1. Authentication & Security (LEA Portal)
- **Secure Access Control:** Government-style portal requiring Official LEA ID and password.
- **Session Security:** TLS 1.3 encrypted session simulation, activity monitoring, and automatic credential hashing.
- **RBAC Matrix:** Built-in Role-Based Access Control supporting 5 distinct tiers (*Administrator*, *Senior Investigator*, *Investigator*, *Analyst*, *Viewer*).
- **Immutable Audit Trail:** Automated logging of every wallet analysis, graph generation, VASP attribution, and report export with timestamps and investigator IDs.

### 📊 2. Executive Intelligence Dashboard (`/dashboard`)
- **Top-Level KPI Cards:**
  - *Active Investigations:* 128
  - *Wallets Analyzed:* 4,892
  - *VASPs Identified:* 1,276
  - *High-Risk Wallets:* 347
  - *Cross-Chain Transactions:* 8,421
  - *Pending Disclosure Requests:* 63
- **Forensic Data Visualizations:**
  - 7-Day Transaction Volume Area Chart (USD value under surveillance)
  - Blockchain Activity Distribution (Ethereum, TRON, Bitcoin, BNB Chain, Solana, Polygon)
  - VASP Attribution Distribution Bar Chart
  - Wallet Risk Distribution Progress Indicators
  - Investigation Case Status Distribution
- **Recent Case Table & Real-Time Alert Stream:** Direct drill-down into open cases and critical incident notifications.

### 🔍 3. Forensic Investigation Creation & 9-Step Pipeline
- Prominent **"+ New Investigation"** wizard with full metadata capture:
  - Case ID, Title, Investigator Name, Crime Category (*Cyber Fraud, Ransomware, Investment Scam, Darknet, Money Laundering, Terror Financing, Phishing, Other*).
  - Suspect Wallet Address, Target Blockchain Network, Incident Date, Priority Level, Evidence References, Case Narrative.
- **Simulated 9-Stage Forensic Processing Engine:**
  1. Validating wallet address format & checksum
  2. Identifying blockchain network & token standards
  3. Fetching raw transaction ledger history
  4. Building multi-hop transaction graph
  5. Detecting intermediary layering & pass-through wallets
  6. Identifying exchange deposit clusters
  7. Querying VASP intelligence database
  8. Calculating 5-factor attribution confidence score
  9. Generating digital investigation dossier
- **Instant Result Modal:** Direct summary of attribution results with one-click navigation into the case workspace.

### 💼 4. Deep Wallet Intelligence (`/wallet`)
- **Core Metrics:** Total Transactions, Incoming/Outgoing Volumes, Net Estimated Balance, Counterparty count, First Seen and Last Active timestamps.
- **Forensic Entity Classification Badges:** `UNHOSTED WALLET`, `ACTIVE`, `HIGH RISK`, `EXCHANGE DEPOSIT`, `SCAM CLUSTER`.
- **Directional Transaction Ledger:** Filterable by Incoming, Outgoing, and All transactions with risk badges, block numbers, gas fees, and behavioral flags (e.g. `ransomware_association`, `rapid_movement`, `structuring`).

### 🕸️ 5. Interactive Blockchain Transaction Graph (`/graph`)
- Built with **React Flow** with custom-styled nodes for:
  - Suspect Wallet (Red border, high-risk badge)
  - Intermediary Wallets (Layering hops)
  - Exchange Deposit Wallets (Blue cluster match)
  - VASP Hot Wallets / Entities (Green verified cluster)
  - Unhosted Feeder Wallets & Darknet Origins
- **Graph Controls:** Zoom, pan, minimap, animated flow edges for critical-risk transfers, and edge labels showing transaction count and token volume.
- **Node Intelligence Drawer:** Clicking any node opens a right-side forensic panel displaying address, entity type, risk score, transaction count, and associated VASP.

### 🏛️ 6. Automated VASP Attribution Engine (`/vasp`)
- **Ranked Attribution Results:**
  1. **Binance** (94% Confidence — Direct Deposit Match, 2 hops)
  2. **OKX** (72% Confidence — Related Wallet Cluster, 4 hops)
  3. **Bybit** (48% Confidence — Possible Intermediary, 6 hops)
- **5-Factor Mathematical Scoring Breakdown:**
  $$\text{Confidence} = (\text{Cluster Match} \times 30\%) + (\text{Deposit Rel.} \times 25\%) + (\text{Graph Prox.} \times 20\%) + (\text{Tx Pattern} \times 15\%) + (\text{Temporal Corr.} \times 10\%)$$
- **Visual Confidence Bars:** Interactive score meters reflecting each component of the algorithm.
- **Mandatory Disclaimers:** Visible notices that automated attribution is an intelligence indicator requiring investigator verification prior to judicial submission.

### 🌉 7. Cross-Chain Intelligence (`/cross-chain`)
- **Visual Cross-Chain Fund Flow:** Traces movement across bridging protocols and DEXs:
  $$\text{Ethereum} \longrightarrow \text{Stargate Bridge} \longrightarrow \text{BNB Chain} \longrightarrow \text{DEX} \longrightarrow \text{TRON} \longrightarrow \text{Centralized Exchange}$$
- **Multi-Chain Network Monitor:** Real-time health, indexing progress, latest block numbers, and API connectivity across **Bitcoin, Ethereum, TRON, BNB Chain, Solana, and Polygon**.

### ⚠️ 8. Risk Intelligence & Factor Breakdown (`/risk`)
- **Radial Risk Score Gauge:** 0–100 overall composite score (87 High Risk).
- **Weighted Factor Breakdown:**
  - *Fraud Exposure (20% weight)*
  - *Ransomware Exposure (20% weight)*
  - *Darknet Exposure (15% weight)*
  - *Sanctions Exposure (15% weight)*
  - *High-Risk VASP Exposure (10% weight)*
  - *Mixer / Tumbler Exposure (10% weight)*
  - *Rapid Fund Movement / Velocity (5% weight)*
  - *Cross-Chain Layering Activity (5% weight)*
- High-Risk vs. Low-Risk indicator analysis cards and methodology documentation.

### 📋 9. Lawful VASP Disclosure Request Workflow
- In-case workflow to create statutory information requests:
  - **Legal Authorities Supported:** *Section 91 CrPC*, *PMLA 2002*, *18 U.S.C. § 2703*, *Mutual Legal Assistance Treaties (MLAT)*.
  - **Request Categories:** KYC Information, Account Identification, Full Transaction Records, Wallet Ownership Verification, Asset Freeze Orders, Record Preservation Orders.
  - **Lifecycle States:** Draft $\rightarrow$ Ready for Review $\rightarrow$ Submitted $\rightarrow$ Acknowledged $\rightarrow$ Response Received.

### 📑 10. Comprehensive Investigation Report Generator (`/reports`)
- One-click dossier generation compiling Case Metadata, Suspect Wallet Intelligence, Ranked VASP Attribution, Key Transactions, and Judicial Disclaimers.
- Multi-format exports: **Generate PDF, Export JSON, Export CSV, and Print Dossier**.

### 🔌 11. API Integrations & Backend Abstraction (`/api-integrations`)
- Monitoring console for 9 external data feeds and node APIs with health percentages, latency in milliseconds, daily request counts, and rate limits.
- **Clean Service Layer Architecture:** All blockchain interactions are decoupled behind TypeScript interfaces so real data providers (Chainalysis, Elliptic, TRM Labs, Etherscan, TronGrid, etc.) can be plugged in without frontend modifications.

### 🔎 12. Live Global Search
- Real-time search in Topbar querying across **Case IDs, Wallet Addresses, Transaction Hashes, VASPs, and Blockchains** with instant categorized dropdown results.

---

## 3. Technology Stack

| Layer | Technology / Library | Purpose |
|---|---|---|
| **Framework** | Next.js 14 (App Router) | Enterprise React framework with server-side routing & API handlers |
| **Language** | TypeScript 5 | Strict static typing across domain models and service interfaces |
| **Styling** | Tailwind CSS + PostCSS | Custom cyber-forensics design system & responsive layout tokens |
| **Graph Visualization** | React Flow (`reactflow` v11) | Interactive node-edge transaction graph with custom rendering |
| **Analytics Charts** | Recharts v2 | Area charts, bar charts, and pie charts for forensic statistics |
| **Icons** | Lucide React | Clean, minimalist enterprise iconography |
| **State & Context** | React Context + Hooks | Session management, global search, and real-time modal state |
| **Backend API** | Next.js Route Handlers | RESTful API endpoints with JSON serialization |

---

## 4. Project File Structure

```
vasp-intelligence/
├── package.json                          # Project dependencies and run scripts
├── tsconfig.json                         # TypeScript compiler configuration with @/* alias
├── tailwind.config.js                    # Design tokens (brand, surface, risk, confidence)
├── postcss.config.js                     # PostCSS processing pipeline
├── next.config.js                        # Next.js configuration
├── README.md                             # Platform documentation
├── PROJECT_DOCUMENTATION.md              # Comprehensive technical report (this file)
└── src/
    ├── app/
    │   ├── globals.css                   # Global styling and custom design rules
    │   ├── layout.tsx                    # Root HTML layout
    │   ├── page.tsx                      # Root route (redirects to /login)
    │   ├── login/
    │   │   └── page.tsx                  # LEA secure authentication portal
    │   ├── (dashboard)/
    │   │   ├── layout.tsx                # Authenticated dashboard wrapper with auth guard
    │   │   ├── dashboard/page.tsx        # Overview dashboard with KPIs and analytics
    │   │   ├── investigations/
    │   │   │   ├── page.tsx              # All cases table with search and filtering
    │   │   │   └── [id]/page.tsx         # Detailed case workspace with tabs & disclosure modal
    │   │   ├── wallet/page.tsx           # Deep wallet analysis & transaction ledger
    │   │   ├── graph/page.tsx            # Interactive React Flow blockchain graph
    │   │   ├── vasp/page.tsx             # Automated VASP attribution & scoring breakdown
    │   │   ├── cross-chain/page.tsx      # Cross-chain bridge tracking & network monitor
    │   │   ├── risk/page.tsx             # Risk intelligence & 8-factor score breakdown
    │   │   ├── alerts/page.tsx           # Incident alert stream with severity filters
    │   │   ├── reports/page.tsx          # Forensic report generator with export buttons
    │   │   ├── api-integrations/page.tsx # API node health, rate limits, and latency monitor
    │   │   └── settings/page.tsx         # User profile, RBAC matrix, and audit log
    │   └── api/
    │       ├── investigations/
    │       │   ├── route.ts              # GET all cases, POST new investigation
    │       │   └── [id]/route.ts         # GET specific investigation by ID
    │       ├── wallet/
    │       │   ├── analyze/route.ts      # POST wallet address for analysis
    │       │   └── [address]/
    │       │       ├── route.ts          # GET wallet details
    │       │       ├── transactions/route.ts # GET wallet transaction history
    │       │       └── graph/route.ts    # GET graph nodes and edges for wallet
    │       ├── vasp/
    │       │   ├── attribute/route.ts    # POST wallet for VASP attribution
    │       │   └── [id]/route.ts         # GET VASP profile details
    │       ├── risk/
    │       │   └── score/route.ts        # POST compute risk profile
    │       ├── cross-chain/
    │       │   └── [wallet]/route.ts     # GET cross-chain transfer events
    │       ├── reports/
    │       │   └── generate/route.ts     # POST compile full investigation report
    │       ├── disclosure-requests/route.ts # GET and POST lawful disclosure notices
    │       └── system/
    │           └── health/route.ts       # GET system and API health status
    ├── components/
    │   ├── layout/
    │   │   ├── Sidebar.tsx               # Fixed desktop navigation sidebar
    │   │   └── Topbar.tsx                # Top header with live search, API badge, and profile
    │   ├── ui/
    │   │   ├── Badge.tsx                 # Generic badge tag
    │   │   ├── Card.tsx                  # Card, CardHeader, CardBody components
    │   │   ├── KpiCard.tsx               # Top-level metric card
    │   │   ├── RiskBadge.tsx             # Color-coded risk status badge
    │   │   ├── ConfidenceBadge.tsx       # Confidence percentage badge & progress bar
    │   │   ├── Modal.tsx                 # Accessible modal dialog
    │   │   ├── PageHeader.tsx            # Standardized page title header
    │   │   └── Tabs.tsx                  # Tabbed navigation container
    │   ├── investigations/
    │   │   └── NewInvestigationModal.tsx # 9-step animated investigation wizard
    │   └── disclosure/
    │       └── NewDisclosureModal.tsx    # Lawful VASP disclosure request creation modal
    ├── services/
    │   ├── index.ts                      # Barrel export for all services
    │   ├── BlockchainService.ts          # Multi-chain network status & address validation
    │   ├── WalletAnalysisService.ts      # Wallet intelligence & entity classification
    │   ├── TransactionService.ts         # Ledger querying & transaction filtering
    │   ├── GraphAnalysisService.ts       # Node-edge graph generation & cluster detection
    │   ├── VASPAttributionService.ts     # 5-factor mathematical attribution engine
    │   ├── RiskScoringService.ts         # Risk scoring & factor weighting
    │   ├── ReportService.ts              # Formal dossier compilation & JSON/CSV export
    │   └── DisclosureRequestService.ts   # Statutory disclosure request lifecycle manager
    ├── data/
    │   └── mockData.ts                   # Realistic synthetic LEA cases, wallets, txs, & VASPs
    ├── types/
    │   └── index.ts                      # Complete TypeScript interfaces and domain types
    └── lib/
        ├── auth.tsx                      # React authentication context & session management
        └── utils.ts                      # Formatting helpers, color mappers, and address shorteners
```

---

## 5. Demonstration Flow & Walkthrough Guide

To present this project effectively for evaluations, presentations, or LEA workflow showcases:

1. **Step 1: Sign In (`/login`)**
   - Official ID: `LEA-IN-2024-7821`
   - Password: `admin123` *(or any text)*
   - Click **"Secure Sign In"**.

2. **Step 2: Executive Dashboard (`/dashboard`)**
   - Showcase the 6 key metrics, the 7-day volume chart, and multi-chain distribution.
   - Click **"+ New Investigation"** in the top right.

3. **Step 3: Create an Investigation Case**
   - Enter suspect wallet: `0x7a9164e8c42f8d6b3a91bf99e0f12c8d5e3a4b71`.
   - Select Crime Category: *Ransomware* or *Cyber Fraud*.
   - Click **"Start Investigation Analysis"**.
   - Watch the realistic 9-step automated analysis animation execute.
   - Click **"View Investigation"** to jump into `CASE-2026-0412`.

4. **Step 4: Case Workspace (`/investigations/[id]`)**
   - Switch between **Case Overview**, **Transactions**, **VASP Attribution**, **Disclosure Requests**, and **Audit Log**.
   - Under **VASP Attribution**, inspect the 94% attribution score for Binance.
   - Click **"Create VASP Disclosure Request"** to draft a Section 91 CrPC / PMLA 2002 preservation notice.

5. **Step 5: Interactive Transaction Graph (`/graph`)**
   - Explore the multi-hop fund flow from Suspect Wallet $\rightarrow$ Intermediary Wallets $\rightarrow$ Deposit Address $\rightarrow$ Binance Hot Wallet.
   - Click any node to open the **Node Intelligence Panel** on the right.

6. **Step 6: VASP Attribution Engine (`/vasp`)**
   - Review the ranked VASP matches (Binance 94%, OKX 72%, Bybit 48%).
   - Explain the 5-factor mathematical formula breakdown shown in the progress bars.

7. **Step 7: Cross-Chain & Risk Analysis (`/cross-chain` & `/risk`)**
   - Review the visual cross-chain movement from Ethereum to TRON via Stargate Bridge.
   - Review the 87/100 risk score breakdown across 8 exposure vectors.

8. **Step 8: Generate Report (`/reports`)**
   - Select a case, click **"Generate Investigation Report"**, and showcase the ready-to-export dossier with export buttons for PDF, JSON, CSV, and Print.

---

## 6. How to Run Locally

```bash
# 1. Navigate to the project directory
cd c:\Users\CHINMAY\OneDrive\Desktop\cybersecurity\vasp-intelligence

# 2. Install all dependencies
npm install

# 3. Start the Next.js development server
npm run dev
```

Open **`http://localhost:3000`** in your browser.
