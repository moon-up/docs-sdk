# EOS

Sure, here's a basic guide on how to interact with the EOS blockchain using the Moon SDK in Markdown format.

### Initialization

Firstly, you need to import the necessary modules and initialize the MoonSDK:

```javascript
import { MoonSDK } from '@moonup/moon-api';

const moonSDK = new MoonSDK({
  apiKey: 'your-api-key',
});
```

Replace `'your-api-key'` with your actual API key.

### List EOS Accounts

To list EOS accounts:

```javascript
async function listEosAccounts() {
  try {
    const response = await moonSDK.getEosSDK().listEosAccounts();
    console.log(response.data);
  } catch (error) {
    console.error(error);
  }
}

listEosAccounts();
```

### Create an EOS Account

To create a new EOS account:

```javascript
async function createEosAccount() {
  try {
    const response = await moonSDK.getEosSDK().createEosAccount({
      network: 'testnet', // or 'mainnet'
    });
    console.log(response.data);
  } catch (error) {
    console.error(error);
  }
}

createEosAccount();
```

The `createEosAccount` function will return an object containing the account name and private key of the newly created account.

### Sign an EOS Transaction

To sign an EOS transaction:

```javascript
async function signEosTransaction(accountName, toAccount, quantity, symbol) {
  try {
    const response = await moonSDK.getEosSDK().signEosTransaction(accountName, {
      network: 'testnet', // or 'mainnet'
      to: toAccount,
      quantity: quantity,
      symbol: symbol,
    });
    console.log(response.data);
  } catch (error) {
    console.error(error);
  }
}

signEosTransaction('your-account-name', 'recipient-account', '1.0000', 'EOS');
```

Replace `'your-account-name'`, `'recipient-account'`, `'1.0000'`, and `'EOS'` with the appropriate values. The `signEosTransaction` function will return an object containing the signed transaction (`signedTx`) and the transaction hash (`transaction_hash`).

### Extra Notes

* Always remember to handle errors properly in your production code.
* This guide assumes that you're running in a Node.js environment. If you're running in a browser, you'll need to use a library like `eosjs` to sign transactions, as the browser doesn't have access to the file system to store private keys.
* This guide uses the testnet network for demonstration purposes. When you're ready to use the mainnet, make sure to change the `network` parameter to `'mainnet'`.
* EOS uses a different unit of account than Bitcoin. One EOS is equal to 1 EOS token, so you'll need to specify the amount in EOS tokens when sending a transaction.
