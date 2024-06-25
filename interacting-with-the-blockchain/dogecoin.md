# Dogecoin

Sure, here's a basic guide on how to interact with the Dogecoin blockchain using the Moon SDK in Markdown format.

### Initialization

Firstly, you need to import the necessary modules and initialize the MoonSDK:

```javascript
import { MoonSDK } from '@moonup/moon-api';

const moonSDK = new MoonSDK({
  apiKey: 'your-api-key',
});
```

Replace `'your-api-key'` with your actual API key.

### List Dogecoin Accounts

To list Dogecoin accounts:

```javascript
async function listDogeCoinAccounts() {
  try {
    const response = await moonSDK.getDogecoinSDK().listDogeCoinAccounts();
    console.log(response.data);
  } catch (error) {
    console.error(error);
  }
}

listDogeCoinAccounts();
```

### Create a Dogecoin Account

To create a new Dogecoin account:

```javascript
async function createDogeCoinAccount() {
  try {
    const response = await moonSDK.getDogecoinSDK().createDogeCoinAccount({
      network: 'testnet', // or 'mainnet'
    });
    console.log(response.data);
  } catch (error) {
    console.error(error);
  }
}

createDogeCoinAccount();
```

The `createDogeCoinAccount` function will return an object containing the address and private key of the newly created account.

### Sign a Dogecoin Transaction

To sign a Dogecoin transaction:

```javascript
async function signDogeCoinTransaction(accountName, toAddress, amount) {
  try {
    const response = await moonSDK.getDogecoinSDK().signDogeCoinTransaction(accountName, {
      network: 'testnet', // or 'mainnet'
      to: toAddress,
      value: amount,
    });
    console.log(response.data);
  } catch (error) {
    console.error(error);
  }
}

signDogeCoinTransaction('your-account-name', 'recipient-address', 1);
```

Replace `'your-account-name'`, `'recipient-address'`, and `1` with the appropriate values. The `signDogeCoinTransaction` function will return an object containing the signed transaction (`signedTx`) and the transaction hash (`transaction_hash`).

### Extra Notes

* Always remember to handle errors properly in your production code.
* This guide assumes that you're running in a Node.js environment. If you're running in a browser, you'll need to use a library like `dogecoinjs-lib` to sign transactions, as the browser doesn't have access to the file system to store private keys.
* This guide uses the testnet network for demonstration purposes. When you're ready to use the mainnet, make sure to change the `network` parameter to `'mainnet'`.
* Dogecoin uses a different unit of account than Bitcoin. One Dogecoin is equal to 100,000,000 Dogecoin coins, so you'll need to specify the amount in Dogecoin coins when sending a transaction.
