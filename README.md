# 🚀 CrewHouz3.0_Mythical_Puffs

Welcome to **CrewHouz3.0_Mythical_Puffs**, your next-gen decentralized app (dApp) built on the Internet Computer Protocol (ICP). This project template helps you get started quickly with canister development using Rust for the backend and a modern frontend stack.

Whether you're building a marketplace, a gaming ecosystem, a social platform, or anything in between — this template sets you up with the right tools and structure.

---

## 📁 Project Structure Overview

```
CrewHouz3.0_Mythical_Puffs/
├── src/
│   ├── backend/        # Rust-based canister logic
│   └── frontend/       # HTML/CSS/JS or React-based frontend
├── .dfx/               # Local network build artifacts
├── dfx.json            # Project configuration
├── package.json        # Frontend project config
├── tsconfig.json       # TypeScript config (if using TS)
└── README.md           # You're here!
```

---

## 🧠 Learn Before You Build

Get familiar with the core tools and frameworks used in this project:

- **[Quick Start](#-quick-start)**
- **[Developer Tools](#️-developer-tools)**
- **[Rust Canister Guide](#-rust-canister-guide)**
- **[ic-cdk Docs](https://docs.rs/ic-cdk/)**
- **[ic-cdk-macros](https://docs.rs/ic-cdk-macros/)**
- **[Candid Language Guide](https://internetcomputer.org/docs/current/developer-docs/candid/candid-intro/)**

---

## 🛠 Getting Started

### ✅ Prerequisites

- Node.js (v16+ recommended)
- Rust (via [rustup](https://rustup.rs/))

---

## ⚙️ Local Development Workflow

```bash
# Navigate to your project directory
cd CrewHouz3.0_Mythical_Puffs/

# Start the local Internet Computer replica
dfx start --background

# Deploy your backend and frontend canisters
dfx deploy
```

🔗 Once deployed, access your app locally:  
[http://localhost:4943/?canisterId={asset_canister_id}](http://localhost:4943/?canisterId={asset_canister_id})

---

## 🎨 Frontend Development

Before starting the frontend server, ensure candid declarations are up to date:

```bash
npm run generate
```

Then run the development server:

```bash
npm start
```

- 📍 Opens at [http://localhost:8080](http://localhost:8080)
- 🔁 Proxies backend API requests to [http://localhost:4943](http://localhost:4943)

---

## 🌐 Deployment Notes

If you're deploying the frontend outside of DFX (e.g., Netlify, Vercel, etc.), consider:

- Setting the `DFX_NETWORK` environment variable to `ic`
- Updating `dfx.json` with a `declarations -> env_override` key for `process.env.DFX_NETWORK`
- Or writing a custom `createActor` function for your backend interface

---

## 🧪 Helpful Commands

```bash
# List all canister commands
dfx canister --help

# Redeploy canisters
dfx deploy

# Clean all build artifacts
dfx stop && dfx cache delete && dfx start --background
```

---

## 🧙 Project Goals

CrewHouz3.0_Mythical_Puffs aims to explore:

- Identity-based access to digital spaces
- NFT-style collectibles or game items
- Secure on-chain state handling
- Mythical theme interactions powered by canisters

---

## 📬 Need Help?

- 📚 [Internet Computer Docs](https://internetcomputer.org/docs/current/)
- 💬 [Join the DFINITY Developer Discord](https://internetcomputer.org/discord)
- 🐞 Found a bug or have a suggestion? Open an issue in your project repo!

---

Let the myths unfold! 🌀