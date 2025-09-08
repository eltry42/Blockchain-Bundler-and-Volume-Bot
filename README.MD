# 🐶 Bonk.fun Multi-Wallet Bundle Trading Bot

A fast and reliable Solana bundle trading bot for **bonkfun** and **bonk.fun**-style token launches. This bot uses **Jito bundles** to create tokens and execute **multi-wallet buys in a single atomic block**. Built with **Raydium SDK v2**, it's designed for seamless one-block execution and fast inclusion.

## 🚀 Features

- ✅ Supports **dynamic multi-wallet bundling** (12+ wallets)
- ✅ Atomically creates tokens and buys from multiple wallets in **one block**
- ✅ Uses **Jito** relayer for secure and efficient bundle submission
- ✅ Executes trades via **Raydium SDK v2**
- ✅ Optimized for priority compute unit pricing

---

## ⚙️ How It Works

1. Creates a new token (like BONK)
2. Prepares swap transactions from multiple wallets
3. Wraps them into a **single atomic bundle** using Jito
4. Submits the bundle for inclusion in the same block

---

## 🛠 Tech Stack

- [Solana Web3.js](https://solana-labs.github.io/solana-web3.js/)
- [Raydium SDK v2](https://github.com/raydium-io/raydium-sdk)
- [Jito-Solana](https://jito.network/)
- Custom bundler and transaction coordinator

---

## ⚡ Performance Tuning

Boost confirmation speed by adjusting compute unit pricing:

```ts
ComputeBudgetProgram.setComputeUnitPrice({ microLamports: 200_000 }); // High priority
```

Use higher values during congestion, or lower for savings.

---
