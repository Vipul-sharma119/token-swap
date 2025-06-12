# 🪙 Token Swap on Solana using Anchor

This project implements a **Token Swap** smart contract on the **Solana blockchain** using the [Anchor framework](https://book.anchor-lang.com/) in **Rust**, with tests written in **TypeScript**.

The program allows users to swap between two SPL tokens securely and efficiently on-chain.

---

## 📦 Tech Stack

- **Solana** – Blockchain platform
- **Rust** – Smart contract logic
- **Anchor** – Framework for Solana smart contracts
- **TypeScript** – Test scripting using Anchor’s TypeScript client

---

## 📁 Project Structure

```
token-swap/
├── programs/
│   └── token_swap/
│       └── src/
│           └── lib.rs         # Anchor program logic
├── tests/
│   └── token_swap.ts          # TypeScript tests
├── Anchor.toml                # Anchor configuration
├── package.json               # TypeScript dependencies for tests
```

---

## 🚀 Features

- Initialize a token swap pool
- Swap between two SPL tokens
- Enforces checks with Anchor constraints
- End-to-end testing in TypeScript

---

## 🔧 Setup & Usage

### 1. Clone the repository

```bash
git clone https://github.com/Vipul-sharma119/token-swap.git
cd token-swap
```

### 2. Install dependencies

Install Rust & Anchor CLI:

```bash
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
cargo install --git https://github.com/coral-xyz/anchor anchor-cli --locked
```

Install Node.js dependencies for tests:

```bash
npm install
```

### 3. Build and deploy the program

```bash
anchor build
anchor deploy
```

### 4. Run tests

```bash
anchor test
```

---

## 🧪 Testing

Tests are written in TypeScript using the Anchor testing framework. They simulate:

- Pool initialization
- Token swapping
- Authority and account checks

Example test command:

```bash
anchor test --provider.cluster devnet
```

---

