# VASP Attribution Intelligence Engine (VASP-AIE)
> **Automated Blockchain Forensics & Virtual Asset Service Provider Attribution Platform with Explainable AI**

[![Next.js](https://img.shields.io/badge/Next.js-14.2.5-black?style=flat&logo=next.js)](https://nextjs.org/)
[![TypeScript](https://img.shields.io/badge/TypeScript-5.0-blue?style=flat&logo=typescript)](https://www.typescriptlang.org/)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-3.4-38bdf8?style=flat&logo=tailwind-css)](https://tailwindcss.com/)
[![React Flow](https://img.shields.io/badge/React_Flow-11.11-ff0072?style=flat)](https://reactflow.dev/)
[![Google Gemini](https://img.shields.io/badge/Google_Gemini-Explainable_AI-8e75ff?style=flat&logo=google)](https://ai.google.dev/)

Designed for **Law Enforcement Agencies (LEAs)**, Financial Intelligence Units (FIUs), and Cyber Crime Investigation Units to investigate unknown cryptocurrency wallets, trace fund layering flows, and automatically attribute transactions to the nearest likely Virtual Asset Service Provider (VASP), centralized exchange, custodial wallet provider, or deposit wallet cluster.

---

## 🏛️ System Overview

The **VASP Attribution Intelligence Engine** is a specialized cyber forensics platform structured specifically for investigative rigor. Unlike retail cryptocurrency explorers or trading dashboards, VASP-AIE enforces strict segregation between:

- **FACT**: Confirmed on-chain transactions, timestamped ledger entries, and verifiable blockchain hashes.
- **INFERENCE**: Graph proximity, clustering heuristics, counterparty velocity, and layering indicators.
- **AUTOMATED ATTRIBUTION**: Algorithmic, deterministic probabilistic confidence scoring.
- **AI SCORE REASONING**: Evidence-grounded natural language explanations powered by **Google Gemini** explaining *why* the score was awarded without altering the score.
- **INVESTIGATOR VERIFICATION**: Manual validation workflows required before statutory disclosure filing or judicial submission.

---

## 🚀 Key Modules & Capabilities

### 1. Grounded Intelligence Dashboard (`/dashboard`)
- Realistic caseload monitoring: Active Investigations, Wallets Analyzed, VASPs Identified, High-Risk Wallets, Cross-Chain Transfers, and Pending Disclosure Requests.
- Multi-chain activity distribution (Ethereum, Bitcoin, TRON, BNB Chain, Solana, Polygon).
- Real-time incident alert stream and daily volume analytics.

### 2. Automated VASP Attribution Engine (`/vasp`)
- **5-Factor Mathematical Scoring Model**:
  $$\text{Confidence} = (\text{Cluster Match} \times 30\%) + (\text{Deposit Rel.} \times 25\%) + (\text{Graph Prox.} \times 20\%) + (\text{Tx Pattern} \times 15\%) + (\text{Temporal Corr.} \times 10\%)$$
- Ranked VASP attribution classifications:
  - **90% – 100%**: Very High Match (e.g. Direct exchange deposit address match)
  - **75% – 89%**: High Match (e.g. Close graph proximity with strong behavioral pattern)
  - **50% – 74%**: Medium Match (e.g. Related cluster with intermediary hops)
  - **< 50%**: Low Match (e.g. Distant proximity, requires further tracing)

### 3. AI Score Reasoning (Powered by Google Gemini)
- **Explainability Layer**: Converts mathematical scoring factors, graph distance, and cluster heuristics into concise, investigator-ready explanations (maximum 2 sentences, ~45 words).
- **Integrity Rule**: Deterministic mathematical scoring remains the sole source of truth. Gemini **never** calculates, alters, or overrides the score.
- **Evidence-Grounded**: Uses only confirmed transaction paths, hop counts, and verified cluster metrics. Never hallucinates counterparties or labels.
- **Failure-Resilient**: Seamless fallback to offline explanations (`AI reasoning unavailable`) if the API key is missing or the network times out. Client bundles never expose API keys.

### 4. Interactive Transaction Graph (`/graph`)
- Full interactive **React Flow** canvas rendering token flows:
  $$\text{Suspect Wallet} \longrightarrow \text{Intermediary Wallets} \longrightarrow \text{Exchange Deposit Addresses} \longrightarrow \text{Exchange Cluster} \longrightarrow \text{VASP Hot Wallets}$$
- Node inspection drawer with risk scores, transaction counts, historical volume, and entity labels.
- Animated, risk-weighted edges highlighting illicit fund layering.

### 5. Multi-Chain & Cross-Chain Intelligence (`/cross-chain`)
- Cross-chain bridge & swap tracker:
  $$\text{Source Chain} \longrightarrow \text{Bridge Protocol} \longrightarrow \text{DEX} \longrightarrow \text{Destination Chain} \longrightarrow \text{Centralized Exchange}$$
- Multi-network monitoring across Bitcoin, Ethereum, TRON, BNB Chain, Solana, and Polygon.

### 6. Comprehensive Risk Intelligence (`/risk`)
- 0–100 Weighted Risk Score with breakdown across 8 threat vectors:
  - Fraud Exposure (20%)
  - Ransomware Exposure (20%)
  - Darknet Exposure (15%)
  - Sanctions Exposure (15%)
  - High-Risk VASP Exposure (10%)
  - Mixer / Tumbler Exposure (10%)
  - Rapid Fund Movement / Velocity (5%)
  - Cross-Chain Layering Activity (5%)

### 7. Statutory Lawful Disclosure Request Generator (`/disclosure`)
- Standardized legal request compiler compliant with statutory authorities:
  - **Section 91 CrPC** (India)
  - **PMLA 2002** (Prevention of Money Laundering Act)
  - **18 U.S.C. § 2703** (Stored Communications Act / St. Cloud Orders)
- Supports request types: KYC Records, Account Details, Transaction History, Wallet Ownership Verification, Asset Freeze Orders, and Preservation Notices.

### 8. Case Workspace & Forensics Pipeline (`/investigations` & `/investigations/[id]`)
- Comprehensive case management workspace with evidence references and status lifecycles (`pending`, `investigating`, `tracing`, `attributed`, `closed`).
- **9-Stage Forensics Pipeline Simulator**: Validates wallet format, identifies chain, ingests history, builds graph, detects layering, isolates exchange clusters, queries intelligence DB, calculates confidence, and compiles forensic dossiers.
- Formal dossier export options: **PDF**, **JSON**, **CSV**, and **Print view**.

### 9. RBAC & Immutable Audit Logging (`/settings` & `/api-integrations`)
- Role-Based Access Control matrix (*Administrator, Senior Investigator, Investigator, Analyst, Viewer*).
- Tamper-evident audit log tracking every query, wallet analysis, and report generation action with timestamp and IP address.
- Live API integration and blockchain RPC node health monitoring.

---

## 🛠️ Architecture & Tech Stack

```
vasp-intelligence/
├── src/
│   ├── app/
│   │   ├── (dashboard)/
│   │   │   ├── dashboard/          # Intelligence Dashboard
│   │   │   ├── investigations/     # Case workspace & details ([id])
│   │   │   ├── wallet/             # Deep wallet forensic analysis
│   │   │   ├── graph/              # Interactive React Flow transaction graph
│   │   │   ├── vasp/               # Automated VASP attribution & AI reasoning
│   │   │   ├── cross-chain/        # Cross-chain bridging tracker
│   │   │   ├── risk/               # Risk matrix & 8-factor score breakdown
│   │   │   ├── alerts/             # Real-time incident alert stream
│   │   │   ├── reports/            # Forensic dossier generator
│   │   │   ├── api-integrations/   # Data feed health & RPC node status
│   │   │   └── settings/           # RBAC & system audit logging
│   │   ├── api/                    # Modular REST API route handlers
│   │   │   ├── vasp/
│   │   │   │   ├── attribute/      # VASP attribution endpoint
│   │   │   │   ├── explain-score/  # Gemini Explainable VASP score endpoint
│   │   │   │   └── [id]/           # VASP details endpoint
│   │   │   ├── wallet/             # Wallet query & graph endpoints
│   │   │   ├── risk/               # Risk scoring endpoints
│   │   │   ├── disclosure-requests/# Statutory disclosure endpoints
│   │   │   └── reports/            # Report compiler endpoints
│   │   ├── login/                  # LEA authentication portal
│   │   ├── globals.css             # Enterprise design tokens
│   │   └── layout.tsx
│   ├── components/
│   │   ├── layout/                 # Sidebar, Topbar with live global search
│   │   ├── ui/                     # Badges, Cards, Modals, Tabs, Gauges
│   │   ├── investigations/         # 9-stage forensics pipeline wizard
│   │   ├── disclosure/             # Statutory disclosure modal
│   │   └── vasp/                   # AiScoreReasoning explainability widget
│   ├── services/                   # Typed Service Layer (Blockchain, VASP, Risk, Report)
│   ├── data/                       # Grounded LEA case mock dataset
│   ├── types/                      # TypeScript domain & AI definitions
│   └── lib/                        # Formatting, auth & mathematical scoring helpers
├── .env.example                    # Environment variable documentation
├── .gitignore                      # Git safety configuration
├── package.json                    # Project dependencies & scripts
└── tsconfig.json                   # TypeScript configuration
```

| Layer | Technology | Version | Purpose |
| :--- | :--- | :--- | :--- |
| **Framework** | Next.js (App Router) | `14.2.5` | Full-stack React architecture |
| **Runtime** | Node.js | `v20+` | Server execution environment |
| **Language** | TypeScript | `^5.0.0` | End-to-end static type safety |
| **Styling** | Tailwind CSS + PostCSS | `^3.4.1` | Dark-accented government enterprise styling |
| **AI Explainability**| Google Gemini REST API | `v1beta` | Explainable AI reasoning layer (`gemini-2.5-flash` / `gemini-1.5-flash`) |
| **Graph Engine** | React Flow (`reactflow`) | `^11.11.4`| Interactive node-and-edge transaction graph |
| **Charts** | Recharts | `^2.12.7` | Area, Bar, and Pie data visualizations |
| **Data Tables** | TanStack Table | `^8.19.3` | Forensic data grid with column sorting |
| **Icons & Time** | Lucide React + Date-fns | `^0.400` / `^3.6` | Security iconography & timestamp utilities |

---

## 💻 Running the Application

### 1. Prerequisites
- **Node.js**: `v18.17.0` or higher (Node `v20+` recommended)
- **npm**: `v9+`

### 2. Installation
Clone the repository and install dependencies:
```bash
git clone <repo-url>
cd vasp-intelligence
npm install
```

### 3. Environment Configuration (Optional)
To enable live **Google Gemini AI Score Reasoning**, create a `.env.local` file in the project root:
```bash
cp .env.example .env.local
```
Add your Google AI Studio API key:
```env
GEMINI_API_KEY=your_actual_gemini_api_key_here
```
> *Note: If `GEMINI_API_KEY` is not provided, the platform automatically utilizes a built-in deterministic fallback engine or displays `"AI reasoning unavailable"` without impacting core functionality.*

### 4. Run the Development Server
```bash
npm run dev
```
Open [http://localhost:4132](http://localhost:4132) in your browser.

### 5. Build and Run in Production Mode
For instant, pre-compiled page navigation (<50ms):
```bash
npm run build
npm run start
```
The production server will listen on [http://localhost:4132](http://localhost:4132).

### 6. Sign In Credentials
This environment utilizes role-based simulation access:
- **Official ID**: Any identifier (e.g. `LEA-IN-2024-7821` or `ADMIN`)
- **Password**: Any password (e.g. `password` or `admin123`)

---

## 📡 API Endpoints Reference

| Method | Endpoint | Description |
| :--- | :--- | :--- |
| `POST` | `/api/vasp/attribute` | Compute probabilistic VASP attribution for a target wallet |
| `POST` | `/api/vasp/explain-score` | **Gemini AI Explainability**: Generate evidence-grounded explanation for a confidence score |
| `GET` | `/api/vasp/[id]` | Fetch profile, jurisdiction, and historical evidence for a specific VASP |
| `GET` | `/api/wallet/[address]` | Retrieve wallet balance, transaction volume, and risk profile |
| `GET` | `/api/wallet/[address]/graph` | Fetch nodes and edges for the transaction graph |
| `POST` | `/api/risk/score` | Compute 8-vector weighted risk score for an address |
| `POST` | `/api/disclosure-requests` | Generate formal statutory legal disclosure notices |
| `POST` | `/api/reports/generate` | Compile formal intelligence dossier (PDF, JSON, CSV) |
| `GET` | `/api/system/health` | Query status of connected blockchain RPC nodes and APIs |

### Example AI Score Reasoning Request
```bash
curl -X POST http://localhost:4132/api/vasp/explain-score \
  -H "Content-Type: application/json" \
  -d '{
    "vasp": "Binance",
    "confidenceScore": 94,
    "chain": "Ethereum",
    "hops": 2,
    "evidence": {
      "relationship": "Direct Deposit",
      "clusterMatch": 92,
      "depositRelationship": 100
    }
  }'
```

**Response**:
```json
{
  "success": true,
  "data": {
    "reasoning": "High confidence because the wallet follows a short 2-hop transaction path to a known Binance deposit cluster with a 92% cluster match.",
    "confidence_level": "High",
    "source": "gemini",
    "factors_highlighted": [
      "2-hop path",
      "Binance cluster match",
      "Confidence: 94%"
    ]
  }
}
```

---

## ⚖️ Evidentiary Standards & Legal Notice

> **INVESTIGATIVE DISCLAIMER**
> Automated VASP attribution scores, graph cluster heuristics, and AI-generated reasoning are **probabilistic intelligence indicators** designed to assist cybercrime investigators and intelligence analysts. They do not constitute judicial proof or verified legal identity. Independent on-chain validation and statutory disclosures must be executed prior to court submission.
