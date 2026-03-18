

# 🛡️ Philanthrovia Ops  

### Enterprise CDP & Identity Resolution Engine

Philanthrovia Ops is a custom-built Customer Data Platform (CDP) designed to eliminate data silos and provide a unified, 360° view of leads across distributed systems.

This is not a traditional CRM.  
It is a decoupled system that resolves identity, tracks behavior, and turns fragmented data into actionable intelligence.

---
## 🔐 Note

This repository showcases the architecture and system design.

Core implementation and business logic are kept private due to the nature of the system.

## 🧩 The Problem

Modern organizations operate across multiple touchpoints:

- Forms  
- Booking systems  
- Offline events  
- Marketing tools  

This creates:

- Fragmented identities (same lead, multiple records)  
- Context-less outreach  
- Expensive, rigid SaaS dependencies  

---

## 🚀 The Approach — "Golden Record" Architecture

At the core of this system is an **Identity Resolution Engine** built around a universal correlation key (email).

Instead of siloed records, every interaction contributes to a single evolving profile:

> One lead → One unified record → Continuous enrichment

---

## ⚙️ Core Capabilities

### Identity Resolution & Progressive Profiling
- Merges multi-source data into a single "Golden Record"  
- Continuously enriches profiles as new interactions occur  

### Multi-Source Ingestion
- Handles data from forms, bookings, and offline inputs  
- Routes structured data into a unified relational schema  

### Behavioral Intent Tracking
- Tracks interaction-level attribution  
- Reconstructs full conversion journeys  

### Offline-to-Online Sync
- Manual entries pass through the same resolution logic  
- Prevents duplication across channels  

### Reverse ETL (Activation Layer)
- Pushes segmented data to external tools (email, analytics, etc.)  
- Enables automated, high-context campaigns  

---

## 🏗️ Architecture Overview

This system is built as a **decoupled integration platform**, not just a dashboard.

### 1. Ingestion & Governance Engine (Backend)

Handles:

- Data collection from multiple sources  
- Input validation and normalization  
- Structured storage with referential integrity  

---

### 2. Identity Resolution Layer (CDP Core)

Where the core logic lives:

- Identity merging  
- Behavioral interpretation  
- Profile unification  

---

### 3. Analytics & Dashboard (Frontend)

The visible layer:

- 360° lead view  
- Behavioral insights  
- Decision support  

> The dashboard is only the surface. The system is driven by the backend architecture.

---

## 🔄 Integration Model

### Outbound (Reverse ETL)
- Segment users inside the CDP  
- Push to external platforms via APIs  
- Trigger automated campaigns  

### Inbound (Data Sync)
- Pull engagement data from third-party tools  
- Feed it back into the system  
- Close the analytics loop  

---

## 🛠️ Tech Stack

**Integration & Backend**
- Node.js  
- Relational Database (optimized for identity correlation)  

**Frontend**
- React / Next.js  
- Tailwind CSS  

**Infrastructure**
- Docker  
- Railway  

**Security**
- RBAC (Role-Based Access Control)  
- Cryptographic hashing  

---

## 📈 Impact

- Eliminated dependency on expensive SaaS tools  
- Reduced lead-to-outreach time through automation  
- Enabled full ownership of data and business logic  

---

## 🎥 Demo

https://github.com/user-attachments/assets/a055c74a-333f-44bf-a1ff-99379c747de3
---

## 📸 Screenshots
<img width="1583" height="1129" alt="login page" src="https://github.com/user-attachments/assets/2a96520c-4c9a-4f6e-9568-97e285b8c0c5" />
<img width="3166" height="2258" alt="dashboard" src="https://github.com/user-attachments/assets/b0ddb3ce-c71e-477c-88d5-626d490f5146" />
<img width="1583" height="1129" alt="manual entry" src="https://github.com/user-attachments/assets/d5ca8ec4-e173-4d5c-9e1c-4ec3e20df3ca" />
<img width="1583" height="1129" alt="analytics page" src="https://github.com/user-attachments/assets/75a6060b-f6e3-4795-9de3-405721e49c45" />
<img width="1583" height="1129" alt="command center" src="https://github.com/user-attachments/assets/a70db517-47fd-45d8-8ec7-10626ae4f571" />




---

## 🧠 Key Insight

Owning the integration layer changes everything.

Instead of relying on third-party middleware:
- Systems communicate directly  
- Latency is reduced  
- Costs are eliminated  
- Control is absolute  

---
