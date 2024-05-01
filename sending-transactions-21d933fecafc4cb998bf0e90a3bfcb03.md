# Sending Transactions

**MoonSDK** offers an easy way to send transactions using just the SDK and API package. However, we recommend using helper packages such as **ethers** to assist in converting between types.

Below is a tutorial on how to send a transaction using **MoonSDK**.

1️⃣ \*\*Step 1: Prepare the transaction data:\*\*

*   Store data pertaining to the transaction in an **`InputBody`** object:

    ```tsx
    import {InputBody} from '@moonup/moon-api';

    // Prepare transaction data
    const amountInWei = ethers.utils.parseUnits(amountEth, 'ether');
    const transactionData: InputBody = {
      to: toAddress,
      value: amountInWei.toString(),
      chain_id: chainId,
      encoding: 'utf-8',
    };
    ```

2️⃣ \*\*Step 2: Sign the transaction:\*\*

*   Next, use the `signTransaction` function to sign the transaction and get the **raw transaction string** to broadcast the transaction.

    ```tsx
    import { MoonSDK, CreateAccountInput } from '@moonup/moon-sdk';

    // Sign and send the transaction
    // moonInstance should be your working instance of MoonSDK
    const signedTransactionData = await moonInstance.getAccountsSDK().signTransaction(account, transactionData);
    const rawTransaction = signedTransactionData.data.data.transactions[0].raw_transaction;

    ```

3️⃣ \*\*Step 3: Broadcast the signed message to the blockchain:\*\*

*   Finally, broadcast the signed message to the blockchain. To do this, **first**, store the raw signed transaction string into a `BroadcastInput` object.

    Then, use the input object to broadcast the transaction using `broadcastTx` .

    ```tsx
    import {BroadcastInput} from '@moonup/moon-api';

    //store signed transaction into 
    const broadcastInput: BroadcastInput = {
      chainId: chainId,
      rawTransaction: rawTransaction
    }
    ```
*   Then, use the input object to broadcast the transaction using `broadcastTx` .

    ```tsx
    //broadcast the signed transaction
    const broadcastResponse = await moonInstance.getAccountsSDK().broadcastTx(account, broadcastInput);
    ```

### Full example of a function that sends transactions:

```tsx
// utils/moonSDKUtil.ts
import { MoonSDK, CreateAccountInput } from '@moonup/moon-sdk';
import { ethers } from 'ethers'; 
import {InputBody, BroadcastInput} from '@moonup/moon-api';

export const sendCoin = async (moonInstance: MoonSDK, account: string, toAddress: string, chainId: string, amountEth: string) => {
  try {
    // Prepare transaction data
    const amountInWei = ethers.utils.parseUnits(amountEth, 'ether');
    const transactionData: InputBody = {
      to: toAddress,
      value: amountInWei.toString(),
      chain_id: chainId,
      encoding: 'utf-8',
    };
  
    // Sign and send the transaction
    const signedTransactionData = await moonInstance.getAccountsSDK().signTransaction(account, transactionData);
    const rawTransaction = signedTransactionData.data.data.transactions[0].raw_transaction;
    
    //(optional) store additional information into variables to display to user
    const transactionHash = signedTransactionData.data.data.transactions[0].transaction_hash;
    const transactionValueWei =  signedTransactionData.data.data.transactions[0].transaction.value;
    const transactionValueEth = ethers.utils.formatEther(transactionValueWei);
    
    // Now, broadcast the signed transaction
    // Make sure the `broadcastTx` method accepts the signed transaction in the format returned by `signTransaction`
    const broadcastInput = {
      chainId: chainId,
      rawTransaction: rawTransaction
    }
    const broadcastResponse = await moonInstance.getAccountsSDK().broadcastTx(account, broadcastInput);
    console.log("Transaction signed and sent: ", signedTransactionData);
    return [transactionHash, transactionValueEth];
  } catch (error) {
    console.error("Error sending coin:", error);
    throw error;
  }
};
```
