# Solana

## Interacting with the Blockchain using MoonSDK on Solana

This tutorial will guide you through the process of initializing the MoonSDK, creating a Solana transaction, signing the transaction, and sending it to the Solana network.

### Prerequisites

* Node.js installed on your machine
* A Solana account with some SOL balance
* Moon API key (optional, but required for some features)

### Installation

First, install the required dependencies:

```bash
npm install @solana/web3.js @moonup/moon-sdk
```

### Initialization

Create a new file, `solana_transaction.js`, and import the necessary modules:

```javascript
import web3, { PublicKey, Transaction } from '@solana/web3.js';
import { MoonSDK } from '@moonup/moon-sdk';
```

Initialize the MoonSDK with your API key (if you have one):

```javascript
const sdk = new MoonSDK({
  apiKey: 'your_moon_api_key',
});
```

### Creating a Solana Transaction

Connect to the Solana network:

```javascript
const connection = new web3.Connection(
  web3.clusterApiUrl('devnet'),
  'confirmed'
);
```

List your Solana accounts using the MoonSDK:

```javascript
const accounts = await sdk.getSolanaSDK().listAccounts();
console.log(accounts);
```

Or create a new solana account using the MoonSDK\


```typescript
const accounts = await sdk.getSolanaSDK().createAccount({});
console.log(accounts);
```

Select the first account as the payer and create a new Solana account as the recipient:

```javascript
const payer = new PublicKey(accounts[0]);
const toAccount = new PublicKey("toAccount");
```

Manually construct the transaction:

```javascript
const recentBlockhash = await connection.getLatestBlockhash();
const manualTransaction = new Transaction({
  recentBlockhash: recentBlockhash.blockhash,
  feePayer: payer,
});
manualTransaction.add(
  web3.SystemProgram.transfer({
    fromPubkey: payer,
    toPubkey: toAccount.publicKey,
    lamports: 1,
  })
);
```

### Signing the Transaction

Serialize the transaction and sign it using the MoonSDK:

```javascript
const serialise = manualTransaction.serialize({
  verifySignatures: false,
  requireAllSignatures: false,
});
const signature = await sdk.getSolanaSDK().signTransaction(accounts[0], {
  unsigned_tx: serialise.toString('base64'),
  network: 'devnet',
});
```

### Sending the Transaction

Send the signed transaction to the Solana network:

```javascript
const hash = await connection.sendRawTransaction(signature.signed_tx);
console.log(hash);
```

### Full Example

```typescript
import web3, { PublicKey, Transaction } from '@solana/web3.js';
import { MoonSDK } from '@moonup/moon-sdk';

export const signAndSend = async () => {
  // const payer = web3.Keypair.generate();
  const connection = new web3.Connection(
    web3.clusterApiUrl('devnet'),
    'confirmed'
  );

  const sdk = new MoonSDK();

  const accounts = await sdk.getSolanaSDK().listAccounts();
  console.log(accounts);
  const payer = new PublicKey(accounts[0]);
  const toAccount = new PublicKey("toAccount");

  // Alternatively, manually construct the transaction
  const recentBlockhash = await connection.getLatestBlockhash();
  const manualTransaction = new Transaction({
    recentBlockhash: recentBlockhash.blockhash,
    feePayer: payer,
  });
  manualTransaction.add(
    web3.SystemProgram.transfer({
      fromPubkey: payer,
      toPubkey: toAccount.publicKey,
      lamports: 1,
    })
  );

  const serialise = manualTransaction.serialize({
    verifySignatures: false,
    requireAllSignatures: false,
  });
  const signature = await sdk.getSolanaSDK().signTransaction(accounts[0], {
    unsigned_tx: serialise.toString('base64'),
    network: 'devnet',
  });
  const hash = await connection.sendRawTransaction(signature.signed_tx);
  console.log(hash);
};
```

### Conclusion

You have successfully created a Solana transaction, signed it using the MoonSDK, and sent it to the Solana network. You can now use the MoonSDK to interact with other blockchain networks and services as well.
