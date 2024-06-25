# Bitcoin cash

Sure, here's a basic guide on how to interact with the Bitcoin Cash blockchain using the Moon SDK in Markdown format.

### Initialization

Firstly, you need to import the necessary modules and initialize the MoonSDK:

```javascript
import { MoonSDK } from '@moonup/moon-api';

const moonSDK = new MoonSDK({
  apiKey: 'your-api-key',
});
```

Replace `'your-api-key'` with your actual API key.

### List Bitcoin Cash Accounts

To list Bitcoin Cash accounts:

```javascript
async function listBitcoinCashAccounts() {
  try {
    const response = await moonSDK.getBitcoincashSDK().listBitcoinCashAccounts();
    console.log(response.data);
  } catch (error) {
    console.error(error);
  }
}

listBitcoinCashAccounts();
```

### Create a Bitcoin Cash Account

To create a new Bitcoin Cash account:

```javascript
async function createBitcoinCashAccount() {
  try {
    const response = await moonSDK.getBitcoincashSDK().createBitcoinCashAccount({
      network: 'testnet', // or 'mainnet'
    });
    console.log(response.data);
  } catch (error) {
    console.error(error);
  }
}

createBitcoinCashAccount();
```

The `createBitcoinCashAccount` function will return an object containing the address and private key of the newly created account.

### Sign a Bitcoin Cash Transaction

To sign a Bitcoin Cash transaction:

```javascript
async function signBitcoinCashTransaction(accountName, toAddress, amount) {
  try {
    const response = await moonSDK.getBitcoincashSDK().signBitcoinCashTransaction(accountName, {
      network: 'testnet', // or 'mainnet'
      to: toAddress,
      value: amount,
    });
    console.log(response.data);
  } catch (error) {
    console.error(error);
  }
}

signBitcoinCashTransaction('your-account-name', 'recipient-address', 0.001);
```

Replace `'your-account-name'`, `'recipient-address'`, and `0.001` with the appropriate values. The `signBitcoinCashTransaction` function will return an object containing the signed transaction (`signedTx`) and the transaction hash (`transaction_hash`).

### Extra Notes

* Always remember to handle errors properly in your production code.
* This guide assumes that you're running in a Node.js environment. If you're running in a browser, you'll need to use a library like `bitcoincashjs-lib` to sign transactions, as the browser doesn't have access to the file system to store private keys.
* This guide uses the testnet network for demonstration purposes. When you're ready to use the mainnet, make sure to change the `network` parameter to `'mainnet'`.
