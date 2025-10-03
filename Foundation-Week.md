# Foundation Week: Build Your First CLI Wallet# Ethereum CLI Wallet Guide



This is where you actually get your hands dirty. No more theory - you're going to create wallets, generate keys, and send transactions. All from the command line like a proper developer.## Step 1: Create a CLI Wallet



## What You're Building### Install Geth (Go Ethereum)



By the end of this guide, you'll have:First, you need to install Geth, which is a popular Ethereum node implementation. Follow the installation instructions for your operating system from the [official documentation](https://geth.ethereum.org/docs/install-and-build/installing-geth).

1. Your own Ethereum CLI wallet

2. Generated keypairs from scratch```sh

3. Gotten testnet ETH# For Debian-based systems:

4. Sent transactions via command linesudo apt-get install software-properties-common

5. Tracked everything on a block explorersudo add-apt-repository -y ppa:ethereum/ethereum

sudo apt-get update

Let's go.sudo apt-get install ethereum

```

---

```sh

## Method 1: Using Geth (The OG Way)# For macOS:

brew tap ethereum/ethereum

Geth (Go Ethereum) is the original Ethereum client. It's overkill for this, but you should know it exists.brew install ethereum

```

### Install Geth

## Step 2: Generate Private and Public Keys

**On Ubuntu/Debian:**

```bash### Using Geth

sudo apt-get install software-properties-common

sudo add-apt-repository -y ppa:ethereum/ethereum```sh

sudo apt-get update# Initialize a new Ethereum account

sudo apt-get install ethereumgeth account new

```

# You will be prompted to enter a passphrase to encrypt your private key.

**On macOS:**```

```bash

brew tap ethereum/ethereumThis will generate a new account and display the public address. The private key is stored encrypted in the keystore directory.

brew install ethereum

```### Using eth-keygen



**On Windows:**Alternatively, you can use `eth-keygen`, a simple tool to generate Ethereum keys.

Download from [geth.ethereum.org](https://geth.ethereum.org/downloads) (or just use WSL)

```sh

### Create Your Wallet# Install eth-keygen

npm install -g eth-keygen

```bash

geth account new# Generate a new key pair

```eth-keygen



It'll ask for a password. **Don't forget this password.** There's no "reset password" button in crypto.# This will output the private and public keys.

```

**What just happened?**

- Geth generated a private key## Step 3: Airdrop Some Native Tokens

- Encrypted it with your password

- Stored it in `~/.ethereum/keystore/`To airdrop tokens, you need to have access to an Ethereum testnet or mainnet where you have some ETH. For test purposes, use a testnet like Sepolia or Holešky.

- Gave you a public address

1. **Obtain Testnet ETH**: Use a faucet to get some testnet ETH. For Sepolia, you can use [this faucet](https://cloud.google.com/application/web3/faucet/ethereum/sepolia).

**Example output:**

```2. **Send ETH to New Account**:

Your new account is locked with a password. Please give a password. Do not forget this password.

Password: ```sh

Repeat password:    # Unlock your account

   geth --Sepolia account unlock [your_main_account_address]

Your new key was generated

   # Send ETH using Geth console

Public address of the key:   0x742d35Cc6634C0532925a3b844Bc9e7595f0Humi   geth attach

Path of the secret key file: /home/humi/.ethereum/keystore/UTC--2025-10-03T10-30-45.123456789Z--742d35cc6634c0532925a3b844bc9e7595f0humi   > eth.sendTransaction({from: 'your_main_account_address', to: 'new_account_address', value: web3.toWei(1, "ether")})

``````



That long `0x742d35...` address? That's your public address. Share it freely. The file in keystore? That's your encrypted private key. **Never share that.**## Step 4: Perform Transactions Using CLI (Send Tokens)



---### Using Geth



## Method 2: Using eth-keygen (The Simple Way)1. **Start Geth Console**:



If Geth feels like too much, use this.```sh

geth attach

### Install```

```bash

npm install -g eth-keygen2. **Unlock the Sender Account:**:

```

```sh

### Generate Keyspersonal.unlockAccount('new_account_address', 'password')

```bash```

eth-keygen

```3. **Send ETH:**:



**Output:**```sh

```eth.sendTransaction({from: 'new_account_address', to: 'recipient_address', value: web3.toWei(0.1, "ether")})

Address: 0x742d35Cc6634C0532925a3b844Bc9e7595f0Humi```

Private Key: 0xac0974bec39a17e36ba4a6b4d238ff944bacb478cbed5efcae784d7bf4f2ff80

```### Using ethers.js



**Save these somewhere safe.** Like actually safe. Not in a file called `my_private_keys.txt` on your Desktop.1. **Install ethers.js**:



---```sh

npm install ethers

## Method 3: Using ethers.js (The Modern Way)```



This is what you'll actually use in real projects.2. **Create a Script:**:



### Create a Script```js

// send-tokens.js

```bashconst { ethers } = require("ethers");

# Create project folder

mkdir humi-wallet// Connect to the network

cd humi-walletconst provider = new ethers.providers.InfuraProvider(

npm init -y  "rinkeby",

npm install ethers  "your_infura_project_id"

```);



**Create `generate-wallet.js`:**// Private key of the sender

```javascriptconst privateKey = "your_private_key";

const { ethers } = require("ethers");const wallet = new ethers.Wallet(privateKey, provider);



// Generate a random wallet// Define the transaction

const wallet = ethers.Wallet.createRandom();const tx = {

  to: "recipient_address",

console.log("\n Wallet Created!\n");  value: ethers.utils.parseEther("0.1"),

console.log("Address:", wallet.address);};

console.log("Private Key:", wallet.privateKey);

console.log("Mnemonic:", wallet.mnemonic.phrase);// Send the transaction

console.log("\n⚠️  SAVE THESE SOMEWHERE SAFE!\n");wallet.sendTransaction(tx).then((txObj) => {

```  console.log("txHash", txObj.hash);

});

**Run it:**```

```bash

node generate-wallet.js3. **Run the Script:**:

```

```sh

**Output:**node send-tokens.js

``````

🎉 Wallet Created!

### Summary

Address: 0x742d35Cc6634C0532925a3b844Bc9e7595f0Humi

Private Key: 0xac0974bec39a17e36ba4a6b4d238ff944bacb478cbed5efcae784d7bf4f2ff80- **Create CLI Wallet**: Use geth account new or eth-keygen.

Mnemonic: test test test test test test test test test test test humi- **Generate Keys**: Automatically done when creating the wallet.

- **Airdrop Tokens**: Use a faucet for testnet ETH and eth.sendTransaction in the Geth console.

⚠️  SAVE THESE SOMEWHERE SAFE!- **Send Transactions**: Use Geth console commands or a script with ethers.js.

```

## Summary

**Pro tip:** The mnemonic is 12 words that can restore your wallet. It's more portable than the private key.

- **Create CLI Wallet**: Use `geth account new` or `eth-keygen`.

---- **Generate Keys**: Automatically done when creating the wallet.

- **Airdrop Tokens**: Use a faucet for testnet ETH and `eth.sendTransaction` in the Geth console.

## Get Testnet ETH (The Faucet)- **Send Transactions**: Use Geth console commands or a script with ethers.js.

You need ETH to send transactions. But we're not using real ETH yet - we're using testnet ETH (fake money for testing).

### Testnets to Use:
- **Sepolia** (recommended - most stable)
- **Holesky** (newer)
- **Goerli** (being phased out, but still works)

### Get Free Testnet ETH:

**Sepolia Faucet:**
1. Go to [Google Cloud Sepolia Faucet](https://cloud.google.com/application/web3/faucet/ethereum/sepolia)
2. Paste your address: `0x742d35Cc6634C0532925a3b844Bc9e7595f0Humi`
3. Complete the CAPTCHA
4. Wait 30 seconds
5. Check your balance on [Sepolia Etherscan](https://sepolia.etherscan.io/)

**Alternative Faucets:**
- [Alchemy Sepolia Faucet](https://sepoliafaucet.com/)
- [Infura Faucet](https://www.infura.io/faucet/sepolia)

**If faucets are being stingy:**
- Some require you to tweet about them
- Some need you to connect with GitHub
- Some have daily limits

Just try multiple ones until you get some ETH.

---

## Send Your First Transaction

Now the fun part - actually sending ETH.

### Using ethers.js (Recommended)

**Create `send-transaction.js`:**
```javascript
const { ethers } = require("ethers");

async function sendTransaction() {
  // Connect to Sepolia testnet
  const provider = new ethers.JsonRpcProvider(
    "https://eth-sepolia.g.alchemy.com/v2/YOUR_ALCHEMY_KEY"
  );

  // Your wallet
  const privateKey = "0xac0974bec39a17e36ba4a6b4d238ff944bacb478cbed5efcae784d7bf4f2ff80";
  const wallet = new ethers.Wallet(privateKey, provider);

  console.log("Sending from:", wallet.address);

  // Transaction details
  const tx = {
    to: "0x8626f6940E2eb28930eFb4CeF49B2d1F2C9C1199", // Random address
    value: ethers.parseEther("0.01"), // 0.01 ETH
  };

  try {
    console.log("Sending transaction...");
    const txResponse = await wallet.sendTransaction(tx);
    
    console.log("Transaction sent! Hash:", txResponse.hash);
    console.log("Waiting for confirmation...");
    
    const receipt = await txResponse.wait();
    console.log("Transaction confirmed in block:", receipt.blockNumber);
    console.log("Gas used:", receipt.gasUsed.toString());
    
  } catch (error) {
    console.error("Error:", error.message);
  }
}

sendTransaction();
```

**Get an Alchemy Key:**
1. Sign up at [alchemy.com](https://www.alchemy.com/)
2. Create a new app
3. Select "Ethereum" and "Sepolia"
4. Copy your API key
5. Replace `YOUR_ALCHEMY_KEY` in the code

**Run it:**
```bash
node send-transaction.js
```

**Output:**
```
Sending from: 0x742d35Cc6634C0532925a3b844Bc9e7595f0Humi
Sending transaction...
Transaction sent! Hash: 0x123abc...
Waiting for confirmation...
Transaction confirmed in block: 4567890
Gas used: 21000
```

---

## Using Geth Console (The Hard Way)

If you want to feel like a hacker in a movie:

```bash
# Connect to Sepolia
geth --sepolia console
```

**In the console:**
```javascript
// Check your balance
eth.getBalance("0x742d35Cc6634C0532925a3b844Bc9e7595f0Humi")

// Unlock your account (needed to send transactions)
personal.unlockAccount("0x742d35Cc6634C0532925a3b844Bc9e7595f0Humi", "your_password", 300)

// Send transaction
eth.sendTransaction({
  from: "0x742d35Cc6634C0532925a3b844Bc9e7595f0Humi",
  to: "0x8626f6940E2eb28930eFb4CeF49B2d1F2C9C1199",
  value: web3.toWei(0.01, "ether")
})
```

**Why this sucks:**
- You need to run a full node (or connect to one)
- The syntax is annoying
- Error messages are cryptic

Stick with ethers.js.

---

## Explore on Block Explorer

Every transaction is public. You can see everything on a block explorer.

### Go to Sepolia Etherscan
[https://sepolia.etherscan.io/](https://sepolia.etherscan.io/)

### Look Up Your Address
Paste `0x742d35Cc6634C0532925a3b844Bc9e7595f0Humi` in the search bar.

**You'll see:**
- Your ETH balance
- All transactions you've sent/received
- Gas fees paid
- Transaction timestamps
- Block numbers

### Look Up Your Transaction
Click on any transaction hash to see:
- **From:** Your address
- **To:** Recipient address
- **Value:** Amount sent
- **Gas Price:** How much you paid per unit of gas
- **Gas Used:** Total gas consumed (usually 21000 for simple transfers)
- **Transaction Fee:** Gas Price × Gas Used
- **Block:** Which block included your transaction
- **Status:** Success or Failed

---

## Common Issues and Fixes

### "Insufficient funds for gas"
**Problem:** You don't have enough ETH to cover gas fees.

**Solution:** Get more testnet ETH from a faucet. Even if you're sending 0.01 ETH, you need extra for gas.

### "Nonce too low"
**Problem:** You're trying to send a transaction with an outdated nonce.

**Solution:** Wait for pending transactions to confirm, or manually set the nonce.

### "Transaction underpriced"
**Problem:** Your gas price is too low.

**Solution:** Increase the gas price or wait for network congestion to clear.

### "Invalid sender"
**Problem:** Wrong private key or address format.

**Solution:** Double-check your private key. Make sure it starts with `0x`.

---

## Understanding What You Just Did

### Private Key
- 64 hexadecimal characters
- Think of it as your password
- Anyone with this can steal your funds
- **Never** share it, **never** commit it to GitHub

### Public Address
- Derived from your private key (one-way - can't reverse it)
- Safe to share publicly
- Like your bank account number
- Example: `0x742d35Cc6634C0532925a3b844Bc9e7595f0Humi`

### Mnemonic Phrase
- 12 or 24 words
- Can generate multiple private keys
- More portable than a private key
- Still need to keep it secret

### Gas
- Fee paid to validators for processing transactions
- Measured in Gwei (1 Gwei = 0.000000001 ETH)
- Simple transfers = 21,000 gas
- Complex smart contracts = way more

### Transaction Hash
- Unique identifier for your transaction
- Like a receipt number
- Use it to track transaction status

---

## Next Steps

Now that you can:
- Generate wallets
- Get testnet ETH
- Send transactions
- Track them on explorers

**Try these challenges:**

1. **Create 3 wallets** and send ETH between them
2. **Check balances** programmatically using ethers.js
3. **Send a transaction with a custom gas price**
4. **Parse a transaction** from Etherscan and understand every field
5. **Save your mnemonic** and restore your wallet from it

### Pro Task: Build a CLI App

Create a proper CLI wallet with commands like:
```bash
humi-wallet create
humi-wallet balance 0x742d35...
humi-wallet send 0x8626f6... 0.01
```

Use Node.js and the `commander` package to build it.

---

## Security Reminders (Read This)

1. **Never use testnet wallets for real money** - They're for learning
2. **Never reuse private keys** - Generate new ones for different purposes
3. **Never store private keys in plain text** - Encrypt them or use hardware wallets
4. **Never commit keys to GitHub** - Use `.env` files and `.gitignore`
5. **Always verify addresses** - One wrong character = lost funds forever

---

## Resources

**Official Docs:**
- [Ethers.js Documentation](https://docs.ethers.org/)
- [Geth Documentation](https://geth.ethereum.org/docs)

**Tools:**
- [Alchemy](https://www.alchemy.com/) - RPC provider
- [Infura](https://www.infura.io/) - Another RPC provider
- [Sepolia Etherscan](https://sepolia.etherscan.io/) - Block explorer

**Learning:**
- Read Etherscan for random addresses and figure out what they're doing
- Try to recreate transactions you see on explorers
- Break things on purpose to understand error messages

---

## You Made It

Congrats. You've done more than 90% of people who say they're "learning Web3."

You now understand:
- How wallets work under the hood
- The relationship between private keys and addresses
- How transactions actually get sent
- What gas fees are and why they exist

This foundation is crucial. Everything else builds on this.

Now go to Week 3 and learn how wallet extensions work.

Keep building, Humi. 
