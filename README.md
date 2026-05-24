# Blockchain-Based Property Ownership Transfer System

**University of Newcastle · Business Analytics · 2024**  
`Blockchain` `Smart Contracts` `Data Governance` `Process Improvement` `JavaScript` `Escrow System` `Security`

---

## 📌 Project Overview

Real estate property transfers involve multiple intermediaries — solicitors, banks, land registries, and settlement agents — creating a process that is slow, expensive, paper-heavy, and vulnerable to fraud. This project proposes and designs a **blockchain-based escrow system for property ownership transfer**, using smart contracts to automate key process steps, improve data integrity, and eliminate unnecessary intermediary dependency.

The project demonstrates the application of **data governance, process improvement, and emerging technology** thinking to a high-value real-world business problem — directly relevant to government, legal, and financial services digitalisation agendas.

---

## 🎯 Business Problem

The current property transfer process suffers from systemic inefficiencies:

| Problem | Impact |
|---|---|
| Multiple intermediaries required | Increases cost, delays settlement timelines (weeks to months) |
| Paper-based documentation | High risk of loss, fraud, and data entry errors |
| Lack of transaction transparency | Buyers and sellers have limited real-time visibility into settlement progress |
| Manual verification at each stage | Slows the process and creates bottlenecks |
| Fragmented data across parties | Each party maintains their own records — no single source of truth |

**Opportunity:** A blockchain-based system can automate verification, enforce contractual obligations via smart contracts, and provide all parties with a transparent, tamper-proof shared ledger — dramatically improving process efficiency, security, and trust.

---

## 📂 Repository Contents

| File | Description |
|---|---|
| `*.js` | Smart contract code — escrow logic, ownership transfer conditions, event triggers |
| `*.pdf` | Full project report — system design, blockchain architecture, process modelling, data governance framework, and security analysis |
| Supporting documentation | Process flow diagrams, stakeholder analysis, data governance considerations |

---

## 🔧 System Design & Methodology

### 1. Current-State Process Analysis (AS-IS)
- Mapped the existing property transfer process across all stakeholders: buyer, seller, solicitors, bank/lender, land registry, and settlement agent
- Identified key pain points: manual document exchange, sequential approval delays, duplication of data across parties, and fraud vulnerability

### 2. Blockchain Architecture Design
The proposed system is built on three core components:

**Component 1 — Smart Contract Escrow**
- Buyer funds are held in a smart contract escrow — released automatically only when predefined conditions are met (e.g. title verified, all parties signed, settlement date reached)
- Eliminates the need for a human escrow agent; contract logic is transparent and auditable by all parties

**Component 2 — Distributed Ledger**
- All property ownership records, transaction history, and document verification events are recorded on an immutable blockchain ledger
- Each party (buyer, seller, bank, land registry) has read access appropriate to their role — no single party controls the record
- Eliminates the risk of data tampering, document loss, or fraudulent alteration

**Component 3 — Automated Verification & Event Triggers**
- Smart contracts automatically verify conditions (identity verification, loan approval, title search clearance) before advancing the transaction
- Event triggers notify all parties of status changes in real time — eliminating manual status chasing

### 3. Data Governance Framework
- Defined data ownership, access controls, and audit trail requirements for each party in the transaction
- Applied data governance principles: accuracy, completeness, consistency, auditability, and security
- Addressed GDPR/Privacy Act compliance: personal data (buyer/seller identity) is stored off-chain with only hashed references on the ledger

### 4. Security Analysis
- Identified key threat vectors: 51% attacks, smart contract vulnerabilities, private key management, and oracle manipulation
- Recommended mitigation strategies: formal smart contract auditing, multi-signature wallets for fund release, and use of established oracle providers for off-chain data feeds

---

## 🗺️ Process Comparison

| Stage | Current Process | Blockchain System |
|---|---|---|
| Contract signing | Physical documents, courier/post | Digital signatures recorded on-chain |
| Fund holding | Human escrow agent | Smart contract escrow — automatic, transparent |
| Title verification | Manual land registry search | Automated on-chain title record check |
| Settlement | Manual coordination across 5–7 parties | Automated trigger when all conditions met |
| Record update | Land registry manually updated | Ownership transfer written to ledger automatically |
| Timeline | 4–12 weeks | Potential reduction to days |

---

## 💡 Business Value

- **Cost reduction:** Eliminates escrow agent fees, reduces solicitor involvement, and cuts administrative overhead
- **Speed:** Automated condition verification and smart contract execution dramatically reduces settlement timelines
- **Security:** Immutable ledger and cryptographic verification eliminate document fraud and data tampering
- **Transparency:** All parties have real-time, role-appropriate visibility into transaction status — reducing disputes
- **Auditability:** Complete, tamper-proof transaction history supports regulatory compliance and dispute resolution

---

## 🛠️ Tools & Technologies

| Category | Details |
|---|---|
| Smart Contracts | JavaScript (Solidity-compatible logic) |
| Blockchain Concepts | Distributed ledger, consensus mechanisms, immutability, cryptographic hashing |
| Data Governance | Access control design, audit trails, privacy compliance |
| Process Modelling | AS-IS / TO-BE analysis, stakeholder mapping |
| Security | Threat modelling, smart contract audit considerations |

---

## ⚠️ Limitations & Considerations

- Blockchain adoption in property transfer requires significant regulatory reform and industry coordination — this is a design and feasibility project, not a production deployment
- Smart contract bugs can be exploited and are difficult to patch post-deployment — formal auditing is essential before any real-world use
- Not all property markets have digitised title records — blockchain adoption depends on prior land registry digitalisation
- User adoption requires accessible interfaces for non-technical stakeholders (buyers, sellers, agents)

---

*Project completed as part of the Bachelor of Business Analytics at the University of Newcastle, 2024.*
