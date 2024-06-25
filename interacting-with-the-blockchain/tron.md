# Tron

Sure, here's a basic guide on how to interact with the Tron blockchain using the Moon SDK in Markdown format.

### Initialization

Firstly, you need to import the necessary modules and initialize the MoonSDK:

```javascript
import { MoonSDK } from '@moonup/moon-api';

const moonSDK = new MoonSDK({
  apiKey: 'your-api-key',
});
```

Replace `'your-api-key'` with your actual API key.

### List Tron Accounts

To list Tron accounts:

```javascript
async function listTronAccounts() {
  try {
    const response = await moonSDK.getTronSDK().listTronAccounts();
    console.log(response.data);
  } catch (error) {
    console.error(error);
  }
}

listTronAccounts();
```

### Create a Tron Account

To create a new Tron account:

```javascript
async function createTronAccount() {
  try {
    const response = await moonSDK.getTronSDK().createTronAccount({
      network: 'testnet', // or 'mainnet'
    });
    console.log(response.data);
  } catch (error) {
    console.error(error);
  }
}

createTronAccount();
```

The `createTronAccount` function will return an object containing the account name and private key of the newly created account.

### Sign a Tron Transaction

To sign a Tron transaction:

```javascript
async function signTronTransaction(accountName, toAddress, amount) {
  try {
    const response = await moonSDK.getTronSDK().signTronTransaction(accountName, {
      network: 'testnet', // or 'mainnet'
      to: toAddress,
      amount: amount,
    });
    console.log(response.data);
  } catch (error) {
    console.error(error);
  }
}

signTronTransaction('your-account-name', 'recipient-address', 100);
```

Replace `'your-account-name'`, `'recipient-address'`, and `100` with the appropriate values. The `signTronTransaction` function will return an object containing the signed transaction (`signedTx`) and the transaction hash (`transaction_hash`).

### Extra Notes

* Always remember to handle errors properly in your production code.
* This guide assumes that you're running in a Node.js environment. If you're running in a browser, you'll need to use a library like `tronweb` to sign transactions, as the browser doesn't have access to the file system to store private keys.
* This guide uses the testnet network for demonstration purposes. When you're ready to use the mainnet, make sure to change the `network` parameter to `'mainnet'`.
* Tron uses a different unit of account than Bitcoin. One TRX is equal to 1,000,000 TRX drops, so you'll need to specify the amount in TRX drops when sending a transaction.
