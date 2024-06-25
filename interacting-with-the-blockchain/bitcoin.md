# Bitcoin

Sure, here's a basic guide on how to interact with the Bitcoin blockchain using the Moon SDK in Markdown format.

### Initialization

Firstly, you need to import the necessary modules and initialize the MoonSDK:

```javascript
import { MoonSDK } from '@moonup/moon-api';

const moonSDK = new MoonSDK({
  apiKey: 'your-api-key',
});
```

Replace `'your-api-key'` with your actual API key.

### List Bitcoin Accounts

To list Bitcoin accounts:

```javascript
async function listBitcoinAccounts() {
  try {
    const response = await moonSDK.getBitcoinSDK().listBitcoinAccounts();
    console.log(response.data);
  } catch (error) {
    console.error(error);
  }
}

listBitcoinAccounts();
```

### Create a Bitcoin Account

To create a new Bitcoin account:

```javascript
async function createBitcoinAccount() {
  try {
    const response = await moonSDK.getBitcoinSDK().createBitcoinAccount({
      network: 'testnet', // or 'mainnet'
    });
    console.log(response.data);
  } catch (error) {
    console.error(error);
  }
}

createBitcoinAccount();
```

The `createBitcoinAccount` function will return an object containing the address and private key of the newly created account.

### Sign a Bitcoin Transaction

To sign a Bitcoin transaction:

```javascript
async function signBitcoinTransaction(accountName, toAddress, amount) {
  try {
    const response = await moonSDK.getBitcoinSDK().signBitcoinTransaction(accountName, {
      network: 'testnet', // or 'mainnet'
      to: toAddress,
      value: amount,
    });
    console.log(response.data);
  } catch (error) {
    console.error(error);
  }
}

signBitcoinTransaction('your-account-name', 'recipient-address', 0.001);
```

Replace `'your-account-name'`, `'recipient-address'`, and `0.001` with the appropriate values. The `signBitcoinTransaction` function will return an object containing the signed transaction (`signedTx`) and the transaction hash (`transaction_hash`).

### Extra Notes

* Always remember to handle errors properly in your production code.
* This guide assumes that you're running in a Node.js environment. If you're running in a browser, you'll need to use a library like `bitcoinjs-lib` to sign transactions, as the browser doesn't have access to the file system to store private keys.
* This guide uses the testnet network for demonstration purposes. When you're ready to use the mainnet, make sure to change the `network` parameter to `'mainnet'`.
