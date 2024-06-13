# Solana

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
  const toAccount = web3.Keypair.generate();

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
