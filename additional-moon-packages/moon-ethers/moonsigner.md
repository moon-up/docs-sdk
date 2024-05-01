# MoonSigner

`MoonSigner` is an [Ethers signer](https://docs.ethers.org/v5/api/signer/#Signer) works with Moon’s wallet infrastructure..

“A **Signer** in \*ethers\* is an abstraction of an Ethereum Account, which can be used to sign messages and transactions and send signed transactions to the Ethereum Network to execute state changing operations.” -Ethers docs

**TLDR:** MoonSigner is mainly for **signing**, **creating**, and **sending transactions** over the blockchain

### Configuration:

Below is an example of how to configure `MoonSigner` for a project:

```tsx
import {MoonSigner, MoonSignerConfig } from '@moonup/ethers';
import { MoonSDK } from '@moonup/moon-sdk'; 

// Function to initialize MoonSigner
export const initializeMoonSigner = (moon: MoonSDK, address: string): MoonSigner => {
  const options: MoonSignerConfig = {
    chainId: "1891",
    SDK: moon,
    address: address
  };
  const moonEthersSigner = new MoonSigner(options);
  return moonEthersSigner;
};
```

### Example usage:

Below is an example of a `MoonSigner` instance:

```tsx
//initialize the signer
const moonSigner = initializeMoonSigner(moonSDKInstance, your_address);

//examples of signer use
const signedTransaction = await moonSigner.signTransaction(transactionRequest);
console.log("Signed Transaction:", signedTransaction);

const transactionResponse = await moonSigner.sendTransaction(transactionRequest);
console.log("Transaction Response:", transactionResponse);
```

### MoonSigner functions:

* **`updateConfig(config: MoonSignerConfig)`:** a function which updates the MoonSigner to change the Signer.
* etc.
