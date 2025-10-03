# 100xDevs Web3.0 Roadmap

Your complete roadmap from zero to Web3 developer. No fluff, just what you actually need to learn.

**Total time:** 4-6 months of consistent work

**Visual Roadmap:** [Open in Excalidraw](https://excalidraw.com/#json=U8y1RGjo_ONJB96VgrOql,hRKEgq7z6k3FK-6NUivERQ)

---

## Phase 1: Zero to One (8-12 Weeks)

This is the foundation. Skip any of this and you'll be lost later. Trust me.

### Week 1-2: Blockchain Fundamentals

**What you'll learn:**
- Why blockchains exist (it's not just for crypto bros)
- How decentralization actually works
- What the hell RPC methods are and why you need them
- Wei vs Ether, lamports vs SOL (unit conversions that'll save you from embarrassing mistakes)
- Cryptography basics: Keccak-256, Ed25119
- Gas fees and why your transaction costs $50 sometimes
- Public/private keys, mnemonic phrases (this is life-or-death important)
- Tokens vs NFTs (the actual technical difference)
- How to sign messages with private keys
- Devnet vs Mainnet (never test on mainnet, seriously)
- Using block explorers (Etherscan, Solscan)

**What you'll build:**
1. **CLI Wallet** - No fancy UI, just command line
2. Generate your own keypairs from scratch
3. Airdrop testnet tokens
4. Send transactions via CLI
5. Track everything on block explorers

**Reality check:** This seems basic but you need to understand this cold. If you don't get public/private key cryptography, everything else will confuse you.

---

### Week 3-6: Wallets (How They Actually Work)

**What you'll learn:**
- Why wallet extensions exist (MetaMask isn't magic)
- How wallets secure private keys without sending them everywhere
- Connecting to RPC nodes
- Native tokens vs ERC-20 tokens (huge difference)
- How wallets display token/NFT balances
- Wallet-dApp communication (the connection flow)
- Signing messages vs signing transactions (different things!)
- Derivation paths (HD wallets explained)

**What you'll build:**
1. **React wallet app** - Create and manage multiple wallets
2. **Wallet impersonator** - Tool to impersonate any address (for testing)
3. Clone something like [mynearwallet.com](https://www.mynearwallet.com/)

**Stack:** React/Next.js + Ethers.js + Node.js/Python

**End Goal:**
- Use existing wallet UX as reference

**Why this matters:** Every dApp needs wallet integration. If you don't understand how wallets work, you can't build good dApps.

---

### Week 7-10: dApps and Transaction Parsing

**What you'll learn:**
- Common on-chain transactions:
  - Simple sends
  - Token swaps
  - Smart contract interactions
- How to parse transactions to extract meaningful data
- Ethereum logs, events, and indexed parameters
- Reading transaction data programmatically

**What you'll build:**
1. **Portfolio tracker** - Show all assets for any wallet
2. **Airdrop notifier** - Alert users when they get airdrops
3. **Transaction aggregator** - Parse and display transaction history

**Examples to study:**
- [matrica.io](https://matrica.io/)
- [assetdash.com](https://www.assetdash.com/)

**The grind:** You'll spend a lot of time debugging why transactions look weird. This is normal. Web3 data is messy.

---

### Week 11-12: DEXs and Swaps

**What you'll learn:**
- How decentralized exchanges work
- Liquidity pools explained properly
- Automated Market Makers (AMM) math
- Creating your own token
- Creating liquidity pools
- Implementing swap functionality

**What you'll build:**
1. **Your own ERC-20 token**
2. **Liquidity pool** for your token
3. **Swap feature** in your wallet app
4. **Transaction parser** for swap transactions

**Tools you'll use:**
- Uniswap/PancakeSwap code as reference
- OpenZeppelin contracts

**Pro tip:** Start with testnet. Don't waste real money learning this.

---

## Phase 2: One to Hundred (12-16 Weeks)

Now you're building real shit. This is where it gets interesting.

### Week 13-14: Solidity and Smart Contracts

**What you'll learn:**
- What smart contracts actually are
- Solidity syntax and data structures
- Development tools: Remix, Truffle, Foundry (pick Foundry)
- OpenZeppelin contract library
- Bytecode, ABIs, and how the EVM works
- Writing secure contracts

**What you'll build:**
1. **ERC-20 token contract** from scratch
2. **Extended ERC-721** (NFT with custom logic)
3. **Escrow contract** (holds funds until conditions met)
4. **Restricted NFT mint** (whitelist/allowlist logic)

**Study these:**
- OpenZeppelin's implementations
- Etherscan verified contracts
- Audit reports (learn from others' mistakes)

**Warning:** Smart contract bugs cost real money. Test everything. Then test again.

---

### Week 15-18: Building Full dApps (Ethereum)

**What you'll learn:**
- React + Web3 integration
- Wallet adapters and connection flows
- Backend verification (Node.js/Python)
- Frontend for contract interactions
- Transaction handling and error states

**What you'll build:**
1. **NFT mint site** with allowlist functionality
2. **Escrow dApp** with full frontend
3. **Web2 backend** that verifies on-chain signatures

**The stack:**
- React/Next.js frontend
- Ethers.js for blockchain interaction
- Node.js/Python backend
- Your smart contracts from previous weeks

**Common issues you'll face:**
- Wallet connection bugs
- Transaction failures
- Gas estimation problems
- Race conditions

Deal with it. This is the learning process.

---

### Week 19-26: Rust and Solana (The Deep End)

**What you'll learn:**
- Rust programming language (full bootcamp)
- Solana CLI and tooling
- Solana's account model (very different from Ethereum)
- Program Derived Addresses (PDAs)
- Token program on Solana
- Associated Token Accounts
- Attaching metadata to tokens/NFTs

**What you'll build:**
1. **Escrow program** in Rust
2. **Token minting program**
3. **ICO contract** (Initial Coin Offering)
4. **Frontend for ICO** with wallet adapter

**Resources:**
- [Solana Program Library](https://github.com/solana-labs/solana-program-library) (mandatory reading)
- [Soldev.app course](https://www.soldev.app/course)
- Anchor framework docs

**Reality check:** Solana is harder than Ethereum. The account model will confuse you. PDAs will make you question life. But once you get it, you're golden.

**Why learn both?** Ethereum has the ecosystem, Solana has the speed. Know both, you're marketable.

---

### Week 27-28: Blockchain Indexing

**What you'll learn:**
- Why you can't just query blockchain data directly
- Event indexing on Ethereum
- Building indexers for transaction tracking
- Sweeping wallets (collecting funds from many addresses)
- Gas optimization techniques
- Accepting crypto payments properly

**What you'll build:**
1. **Payment processor** for your web2 app
2. **Indexer** that tracks specific events
3. **Wallet sweeper** with gas optimization

**Tools:**
- The Graph protocol
- Alchemy webhooks
- Custom indexer with Node.js

**Use case:** Your e-commerce site needs to accept crypto. This is how you do it right.

---

### Week 29-32: Building Production Apps

**Pick ONE:**

#### Option A: Build an Exchange
- Order book logic
- Deposit/withdrawal system
- Hot and cold wallet management
- Private key security (Shamir's Secret Sharing)
- Sweeping deposits
- Trading pairs and matching engine

**Example:** Like Binance but simpler

#### Option B: Build a Gambling/Gaming Platform
- Game logic (dice, cards, whatever)
- Deposit system
- Withdrawal system
- Provably fair algorithms
- Bankroll management

**Example:** Like Stake.com but you own it

**Why these projects?**
Both require you to:
- Handle real money securely
- Manage private keys properly
- Build complex backend logic
- Deal with edge cases
- Think about security constantly

This is senior-level stuff. If you can build either of these, you're job-ready.

---

## Free Resources (Actually Good Ones)

**Courses:**
- [Alchemy University](https://www.alchemy.com/university/courses/ethereum) - Comprehensive Ethereum course
- [Soldev Course](https://www.soldev.app/course) - Best Solana course, period

**Code to Study:**
- [Solana Program Library](https://github.com/solana-labs/solana-program-library) - Official Solana programs
- OpenZeppelin contracts
- Uniswap V2/V3 contracts
- Audited contracts on GitHub

**Communities:**
- BuildSpace (for project-based learning)
- Developer DAOs
- Protocol Discord servers (Uniswap, Aave, etc.)

---

## How to Actually Follow This

1. **Don't skip weeks** - Each builds on the previous
2. **Build everything** - Reading won't cut it
3. **Break things** - Best way to learn
4. **Ask for help** - When you're stuck for >2 hours
5. **Share your work** - Twitter, GitHub, wherever

---

## Reality Check

- **Week 1-6:** You'll feel overwhelmed. Normal.
- **Week 7-12:** Things start clicking. Keep going.
- **Week 13-18:** You'll think you know stuff. You don't yet.
- **Week 19-26:** This is the hardest part. Push through.
- **Week 27-32:** If you get here, you're in the top 5%.

Most people quit around week 8-10. Don't be most people.

---

## What Success Looks Like

After completing this:
- You can build full-stack dApps on Ethereum and Solana
- You understand security best practices
- You can read and audit smart contracts
- You can integrate crypto into any web2 app
- You're employable as a Web3 developer

---

## Contributing

Found better resources? Spot an error?

1. Fork [this repo](https://github.com/NiladriHazra/Web3-Road-Map)
2. Make your changes
3. Submit a PR

**Found this helpful?** ⭐ Star the [repo](https://github.com/NiladriHazra/Web3-Road-Map)

**Support this project:** [Buy me a coffee](https://buymeacoffee.com/niladri)

---

Good luck. You'll need discipline, not motivation. Motivation fades. Discipline gets you through week 20 when Rust is kicking your ass.

Now start building.