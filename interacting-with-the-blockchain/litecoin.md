# Litecoin

Sure, here's a basic guide on how to interact with the Litecoin blockchain using the Moon SDK in Markdown format.

### Initialization

Firstly, you need to import the necessary modules and initialize the MoonSDK:

```javascript
import { MoonSDK } from '@moonup/moon-api';

const moonSDK = new MoonSDK({
  apiKey: 'your-api-key',
});
```

Replace `'your-api-key'` with your actual API key.

### List Litecoin Accounts

To list Litecoin accounts:

```javascript
async function listLitecoinAccounts() {
  try {
    const response = await moonSDK.getLitecoinSDK().listLitecoinAccounts();
    console.log(response.data);
  } catch (error) {
    console.error(error);
  }
}

listLitecoinAccounts();
```

### Create a Litecoin Account

To create a new Litecoin account:

```javascript
async function createLitecoinAccount() {
  try {
    const response = await moonSDK.getLitecoinSDK().createLitecoinAccount({
      network: 'testnet', // or 'mainnet'
    });
    console.log(response.data);
  } catch (error) {
    console.error(error);
  }
}

createLitecoinAccount();
```

The `createLitecoinAccount` function will return an object containing the address and private key of the newly created account.

### Sign a Litecoin Transaction

To sign a Litecoin transaction:

```javascript
async function signLitecoinTransaction(accountName, toAddress, amount) {
  try {
    const response = await moonSDK.getLitecoinSDK().signLitecoinTransaction(accountName, {
      network: 'testnet', // or 'mainnet'
      to: toAddress,
      value: amount,
    });
    console.log(response.data);
  } catch (error) {
    console.error(error);
  }
}

signLitecoinTransaction('your-account-name', 'recipient-address', 0.001);
```

Replace `'your-account-name'`, `'recipient-address'`, and `0.001` with the appropriate values. The `signLitecoinTransaction` function will return an object containing the signed transaction (`signedTx`) and the transaction hash (`transaction_hash`).

### Extra Notes

* Always remember to handle errors properly in your production code.
* This guide assumes that you're running in a Node.js environment. If you're running in a browser, you'll need to use a library like `bitcoincashjs-lib` to sign transactions, as the browser doesn't have access to the file system to store private keys.
* This guide uses the testnet network for demonstration purposes. When you're ready to use the mainnet, make sure to change the `network` parameter to `'mainnet'`.
