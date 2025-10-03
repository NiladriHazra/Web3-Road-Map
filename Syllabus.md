# Web3 Learning Syllabus# Web3 Learning Syllabus# 100xDevs Web3.0 Roadmap



Your complete roadmap from zero to Web3 developer. No fluff, just what you actually need to learn.



**Total time:** 4-6 months of consistent workThis is your actual learning path. Not some vague "learn blockchain" BS - this is week-by-week what you need to build and understand.## 0 - 1



**Visual Roadmap:** [Open in Excalidraw](https://excalidraw.com/#json=U8y1RGjo_ONJB96VgrOql,hRKEgq7z6k3FK-6NUivERQ)



---Total time: **4-6 months** if you're serious about it.### Foundation (~2 Weeks):



## Phase 1: Foundations (0 → 1)



### Weeks 1-2: Blockchain Fundamentals---1. Why blockchains? What do they provide?



**Core Concepts:**2. What is decentralization?

- Why blockchains exist and what problems they solve

- How decentralization works## Phase 1: Zero to One (8-12 Weeks)3. RPC’s, Common RPC methods.

- RPC methods and connecting to networks

- Understanding Wei/Ether and Lamports/SOL4. Wei vs Ether, lamports vs SOL.

- Cryptography basics (Keccak-256, Ed25519)

- Gas fees and transactionsThis is the foundation. Skip any of this and you'll be lost later. Trust me.5. Cryptography, hashing, Encryption - Keccak-256, Ed25119.

- Public/private keys and mnemonic phrases

- Tokens vs NFTs6. Gas & Transactions.

- Signing messages with private keys

- Devnet vs Mainnet---7. Public and private keys, mnemonic phrases, creating your own private keys.

- Using block explorers (Etherscan, Solscan)

8. What are Tokens, Non Fungible Tokens.

**Build:**

- CLI wallet that generates keys### Week 1-2: Blockchain Fundamentals9. Basic cryptography.

- Airdrop testnet tokens

- Send transactions from command line10. Signing messages using private keys.

- Track transactions on explorers

**What you'll learn:**11. Devnet vs Mainnet environments.

---

- Why blockchains exist (it's not just for crypto bros)12. Airdropping.

### Weeks 3-6: Wallets

- How decentralization actually works13. Understanding block explorers (etherscan, solscan).

**Core Concepts:**

- How wallet extensions work (MetaMask, Phantom)- What the hell RPC methods are and why you need them

- Private key security

- RPC connections from wallets- Wei vs Ether, lamports vs SOL (unit conversions that'll save you from embarrassing mistakes)**End Goal:**

- Native tokens vs ERC-20/SPL tokens

- Wallet-dApp communication- Cryptography basics: Keccak-256, Ed25119

- Signing messages vs signing transactions

- HD wallets and derivation paths- Gas fees and why your transaction costs $50 sometimes1. Create a CLI wallet.



**Build:**- Public/private keys, mnemonic phrases (this is life-or-death important)2. Generate private and public keys using CLI’s.

- React app for creating and managing wallets

- Wallet impersonator tool (for testing)- Tokens vs NFTs (the actual technical difference)3. Airdrop some native token.

- Clone of [mynearwallet.com](https://www.mynearwallet.com/)

- How to sign messages with private keys4. Do some transactions using CLI (Send Tokens).

---

- Devnet vs Mainnet (never test on mainnet, seriously)5. Explore transactions on explorers.

### Weeks 7-10: dApps & Transaction Parsing

- Using block explorers (Etherscan, Solscan)

**Core Concepts:**

- Common transaction types (sends, swaps, contract calls)============================================

- Parsing transaction data

- Ethereum logs, events, and indexed parameters**What you'll build:**

- Building aggregators

1. **CLI Wallet** - No fancy UI, just command line## Wallets (~3-4 Weeks):

**Build:**

- Portfolio tracker (show all wallet assets)2. Generate your own keypairs from scratch

- Airdrop notifier

- Transaction history viewer3. Airdrop testnet tokens1. Why do you need a wallet? What are wallet extensions?



**Examples:** [matrica.io](https://matrica.io/), [assetdash.com](https://www.assetdash.com/)4. Send transactions via CLI2. How do they secure your private key?



---5. Track everything on block explorers3. Connecting to RPCs from wallets.



### Weeks 11-12: DEXs & Swaps4. Native tokens vs ERC20 (or token program)



**Core Concepts:****Reality check:** This seems basic but you need to understand this cold. If you don't get public/private key cryptography, everything else will confuse you.5. Showing token balances, NFT balances.

- How decentralized exchanges work

- Liquidity pools and AMMs6. How do wallets interact with dApps (overview).

- Creating tokens and pools

- Swap functionality---7. Signing messages vs Signing transactions.



**Build:**8. Common Derivation Path.

- Your own ERC-20 token

- Liquidity pool for your token### Week 3-6: Wallets (How They Actually Work)9. Creating a website similar to https://www.mynearwallet.com/

- Swap feature in your wallet

- Transaction parser for swaps10. Create a wallet impersonator that lets you impersonate someone.



---**What you'll learn:**



## Phase 2: Smart Contracts (1 → 100)- Why wallet extensions exist (MetaMask isn't magic)**End Goal:**



### Weeks 13-14: Solidity- How wallets secure private keys without sending them everywhere



**Core Concepts:**- Connecting to RPC nodes1. Use an existing wallet, get comfortable with its UX.

- Smart contract basics

- Solidity syntax and data structures- Native tokens vs ERC-20 tokens (huge difference)2. Create a React app that lets you create wallets and impersonate them.

- Development tools (Remix, Foundry, Hardhat)

- OpenZeppelin libraries- How wallets display token/NFT balances

- ABIs and EVM

- Security best practices- Wallet-dApp communication (the connection flow)============================================



**Build:**- Signing messages vs signing transactions (different things!)

- ERC-20 token from scratch

- ERC-721 NFT with custom logic- Derivation paths (HD wallets explained)## dApps and Transactions (~5-6 Weeks):

- Escrow contract

- Restricted NFT mint with allowlist- Building wallet UIs



---1. Understanding commonly done transactions on chain:



### Weeks 15-18: Ethereum dApps**What you'll build:**   a. Sents.



**Core Concepts:**1. **React wallet app** - Create and manage multiple wallets   b. Swaps.

- React + Web3 integration

- Wallet adapters2. **Wallet impersonator** - Tool to impersonate any address (for testing)   c. Smart contract interactions.

- Backend verification

- Transaction handling3. Clone something like [mynearwallet.com](https://www.mynearwallet.com/)2. Parsing transactions to show data in a wallet.



**Build:**3. Logs, events, and indexed parameters in Ethereum.

- NFT minting website with allowlist

- Escrow dApp with frontend**Resources to use:**4. Create a wallet aggregator/portfolio tracker/airdrop notifier.

- Web2 backend with signature verification

- Study MetaMask's open-source code   - Examples: https://matrica.io/ OR https://www.assetdash.com/

**Stack:** React/Next.js + Ethers.js + Node.js/Python

- Use existing wallet UX as reference

---

**End Goal:**

### Weeks 19-26: Rust & Solana

**Why this matters:** Every dApp needs wallet integration. If you don't understand how wallets work, you can't build good dApps.

**Core Concepts:**

- Rust programming language1. Understanding a lot of common transaction formats, parsing them.

- Solana CLI and tooling

- Solana account model---2. Creating a portfolio/airdrop tracker.

- Program Derived Addresses (PDAs)

- Token program and associated accounts

- NFT metadata on Solana

### Week 7-10: dApps and Transaction Parsing============================================

**Build:**

- Escrow program in Rust

- Token minting program

- ICO contract**What you'll learn:**## DEXs and Swap Functionality (~7-8 Weeks):

- Frontend for ICO with Solana wallet adapter

- Common on-chain transactions:

**Resources:**

- [Solana Program Library](https://github.com/solana-labs/solana-program-library)  - Simple sends1. Understanding what are DEXs.

- [Soldev Course](https://www.soldev.app/course)

  - Token swaps2. Liquidity pools.

---

  - Smart contract interactions3. Automated market makers.

### Weeks 27-28: Indexing & Payments

- How to parse transactions to extract meaningful data4. Creating your own token & Creating a pool for it.

**Core Concepts:**

- Why blockchain indexing is needed- Ethereum logs, events, and indexed parameters5. Adding swap functionality to your wallet, letting users choose from popular markets.

- Event indexing on Ethereum

- Sweeping wallets- Reading transaction data programmatically

- Gas optimization

- Accepting crypto payments properly**End Goal:**



**Build:****What you'll build:**

- Payment processor for web2 apps

- Custom event indexer1. **Portfolio tracker** - Show all assets for any wallet1. Adding swap functionality to your wallet.

- Wallet sweeper with gas optimization

2. **Airdrop notifier** - Alert users when they get airdrops2. Adding transaction parsing so all swaps are visible in your wallet.

**Tools:** The Graph, Alchemy webhooks

3. **Transaction aggregator** - Parse and display transaction history

---

============================================

### Weeks 29-32: Production Project

**Examples to study:**

**Choose One:**

- [matrica.io](https://matrica.io/)## 1 - 100

**Option A: Decentralized Exchange**

- Order book logic- [assetdash.com](https://www.assetdash.com/)

- Deposits and withdrawals

- Hot/cold wallet management### Solidity and Smart Contracts (~2 Weeks):

- Shamir's Secret Sharing for key security

- Trading pairs and matching engine**The grind:** You'll spend a lot of time debugging why transactions look weird. This is normal. Web3 data is messy.



**Option B: Gaming/Gambling Platform**1. What are smart contracts?

- Game logic (dice, poker, etc.)

- Deposit/withdrawal system---2. Solidity syntax, data model on ETH.

- Provably fair algorithms

- Bankroll management3. Remix vs Truffle, Ganache vs Foundry.



Both projects teach you production-level security and architecture.### Week 11-12: DEXs and Swaps4. OpenZeppelin.



---5. Bytecode, ABIs and EVM.



## Learning Resources**What you'll learn:**6. Writing contracts:



**Courses:**- How decentralized exchanges work   a. Creating ERC20

- [Alchemy University](https://www.alchemy.com/university/courses/ethereum) - Free Ethereum course

- [Soldev](https://www.soldev.app/course) - Free Solana course- Liquidity pools explained properly   b. Extending ERC721



**Documentation:**- Automated Market Makers (AMM) math   c. Writing an Escrow contract

- Ethereum.org docs

- Solidity docs- Creating your own token   d. Creating a restricted NFT mint.

- Ethers.js docs

- OpenZeppelin contracts- Creating liquidity pools7. Exploring common contracts.



**Code Examples:**- Implementing swap functionality

- [Solana Program Library](https://github.com/solana-labs/solana-program-library)

- OpenZeppelin GitHub**End Goal:**

- Uniswap contracts

**What you'll build:**

**This Repo:**

- [GitHub Repository](https://github.com/NiladriHazra/Web3-Road-Map)1. **Your own ERC-20 token**1. Writing smart contracts.



---2. **Liquidity pool** for your token2. Local development of Solidity.



## How to Follow This3. **Swap feature** in your wallet app3. Web2 + Web3 use case of adding custom minting logic.



1. **Follow the order** - Each week builds on previous weeks4. **Transaction parser** for swap transactions

2. **Actually build** - Don't just read, code everything

3. **Test on testnets** - Never deploy to mainnet while learning============================================

4. **Ask when stuck** - Don't waste days on one bug

5. **Share your progress** - Post on Twitter/GitHub**Tools you'll use:**



---- Uniswap/PancakeSwap code as reference### Creating a dApp (~3-4 Weeks)



## Reality Check- OpenZeppelin contracts



**Weeks 1-6:** Feels overwhelming, that's normal1. Creating a React project with web3 signing, learn about adapters, connecting to dApps.



**Weeks 7-12:** Things start making sense**Pro tip:** Start with testnet. Don't waste real money learning this.2. Creating a web2 backend with verification (Python/Node.js)



**Weeks 13-18:** You think you know stuff (you don't yet)3. Create frontend for NFT mint with allowlist.



**Weeks 19-26:** Hardest part - Solana is tough---4. Create frontend for escrow contract.



**Weeks 27-32:** If you reach here, you're in top 5%



Most people quit around week 8-10. Don't be them.## Phase 2: One to Hundred (12-16 Weeks)**End Goal:**



---



## What You'll KnowNow you're building real shit. This is where it gets interesting.1. Adding frontends to your dApps.



After completing this:2. ETH adapters.

- Build full-stack dApps on Ethereum and Solana

- Write and audit smart contracts---

- Implement proper security practices

- Integrate crypto into any web2 app============================================

- Be job-ready as a Web3 developer

### Week 13-14: Solidity and Smart Contracts

---

### Rust and Solana Smart Contracts (~5-8 Weeks):

## Contributing

**What you'll learn:**

Found better resources? Spot an error? 

- What smart contracts actually are1. Rust complete bootcamp.

1. Fork [this repo](https://github.com/NiladriHazra/Web3-Road-Map)

2. Make your changes- Solidity syntax and data structures2. Solana CLI, Solana token program.

3. Submit a PR

- Development tools: Remix, Truffle, Foundry (pick Foundry)3. Data model in Solana, PDAs.

---

- OpenZeppelin contract library4. PDAs in action, creating a web2 use case in web3. Postgres tables vs PDAs.

**Found this helpful?** ⭐ Star the [repo](https://github.com/NiladriHazra/Web3-Road-Map)

- Bytecode, ABIs, and how the EVM works5. Create an escrow contract.

**Support this project:** [Buy me a coffee](https://buymeacoffee.com/niladri)

- Writing secure contracts6. Deep dive into the Solana token program, associated token account program.

Good luck. Discipline beats motivation. Now start building.

7. Attaching metadata to tokens and NFTs.

**What you'll build:**8. Exploring common contracts.

1. **ERC-20 token contract** from scratch

2. **Extended ERC-721** (NFT with custom logic)**End Goal:**

3. **Escrow contract** (holds funds until conditions met)

4. **Restricted NFT mint** (whitelist/allowlist logic)1. Writing smart contracts in Solana.

2. Local Solana development.

**Study these:**

- OpenZeppelin's implementations============================================

- Etherscan verified contracts

- Audit reports (learn from others' mistakes)### Creating a dApp (~9-10 Weeks):



**Warning:** Smart contract bugs cost real money. Test everything. Then test again.1. Creating a React project with web3 signing.

2. Solana wallet adapter.

---3. Create an Initial coin offering contract.

4. Create a frontend that lets users get a token allocation based on their share of the launch investment.

### Week 15-18: Building Full dApps (Ethereum)

**End Goal:**

**What you'll learn:**

- React + Web3 integration1. Adding frontend to your dApps.

- Wallet adapters and connection flows

- Backend verification (Node.js/Python)============================================

- Frontend for contract interactions

- Transaction handling and error states### Indexing Blockchains (~11-12 Weeks):



**What you'll build:**1. Understanding how to get payments the right way in web2 app.

1. **NFT mint site** with allowlist functionality2. Understanding indexing of the blockchain on ETH.

2. **Escrow dApp** with full frontend3. Sweeping wallets, gas optimisations.

3. **Web2 backend** that verifies on-chain signatures

**End Goal:**

**The stack:**

- React/Next.js frontend1. Indexing blockchain

- Ethers.js for blockchain interaction2. Accepting payments the right way.

- Node.js/Python backend

- Your smart contracts from previous weeks============================================



**Common issues you'll face:**### Building an Exchange/Gambling Website:

- Wallet connection bugs

- Transaction failures1. Creating an order-book/create game logic.

- Gas estimation problems2. Allowing deposit and withdrawal logic.

- Race conditions3. Storing the private key, hot and cold wallets, sweeping deposits, Shamir's secret sharing.



Deal with it. This is the learning process.**End Goal:**



---1. Creating an exchange like Binance.

   OR

### Week 19-26: Rust and Solana (The Deep End)2. Creating a gambling website like Stake.com



**What you'll learn:**============================================

- Rust programming language (full bootcamp)

- Solana CLI and tooling## Free Resources

- Solana's account model (very different from Ethereum)

- Program Derived Addresses (PDAs)1. [Alchemy University Courses](https://www.alchemy.com/university/courses/ethereum)

- Token program on Solana2. [Solana Program Library](https://github.com/solana-labs/solana-program-library)

- Associated Token Accounts3. [Soldev App Course](https://www.soldev.app/course)
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

## Reality Check Part 2

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

Good luck. You'll need discipline, not motivation. Motivation fades. Discipline gets you through week 20 when Rust is kicking your ass.

Now start building.
