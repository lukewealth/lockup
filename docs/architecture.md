# 🏗️ LockUps Architecture

## Overview
LockUps is designed as a **multi-layer system** combining frontend apps, backend services, blockchain infrastructure, and integrations with fiat on/off-ramps.

## Layers
1. **Frontend**
   - Next.js web app
   - Tailwind CSS + Shadcn UI
   - Mobile-first PWA with USSD/SMS fallback

2. **Backend**
   - Node.js / Express API
   - GraphQL for optimized queries
   - MongoDB / PostgreSQL (user data, off-chain credit scoring)

3. **Blockchain Layer**
   - Smart Contracts (Rust/Anchor for Solana)
   - Stablecoin settlement contracts
   - Wallet Adapter SDK (multi-chain support)

4. **Integration Layer**
   - Mobile money APIs (cash in/out)
   - SMS/USSD gateways
   - Cloud hosting on AWS/GCP

## Data Flow
- User → Frontend (Web/Mobile/USSD)
- Frontend → Backend (APIs/GraphQL/MogoDB)
- Backend → Smart Contracts (P2P Transfers, Credit Scoring)
- Blockchain → Confirmations → User
