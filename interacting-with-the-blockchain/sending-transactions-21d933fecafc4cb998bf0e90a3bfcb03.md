# EVM

## Interacting with EVM Transactions using MoonSDK

This tutorial will guide you through the process of sending an EVM transaction using MoonSDK. We will cover sending transactions with and without encoded ABI data, as well as creating and listing accounts.

### Prerequisites

* Node.js installed on your machine
* An EVM-compatible account with some balance
* Moon API key (optional, but required for some features)

### Installation

First, install the required dependencies:

```bash
npm install @moonup/moon-sdk ethers
```

### Initialization

Create a new file, `evm_transaction.ts`, and import the necessary modules:

```javascript
import { MoonSDK } from '@moonup/moon-sdk';
import { ethers } from 'ethers';
import { InputBody, BroadcastInput } from '@moonup/moon-api';
```

Initialize the MoonSDK with your API key (if you have one):

```javascript
const sdk = new MoonSDK({
  apiKey: 'your_moon_api_key',
});
```

### Sending a Transaction without Encoded ABI Data

To send a transaction without encoded ABI data, you need to prepare the transaction data, sign the transaction, and broadcast it to the blockchain.

#### Step 1: Prepare the Transaction Data

Store data pertaining to the transaction in an InputBody object:

```javascript
const amountInWei = ethers.utils.parseUnits(amountEth, 'ether');
const transactionData: InputBody = {
  to: toAddress,
  value: amountInWei.toString(),
  chain_id: chainId,
  encoding: 'utf-8',
};
```

#### Step 2: Sign the Transaction

Use the signTransaction function to sign the transaction and get the raw transaction string to broadcast the transaction:

```javascript
const signedTransactionData = await sdk.getAccountsSDK().signTransaction(account, transactionData);
const rawTransaction = signedTransactionData.data.data.transactions[0].raw_transaction;
```

#### Step 3: Broadcast the Signed Message to the Blockchain

Store the raw signed transaction string into a BroadcastInput object and use the input object to broadcast the transaction using broadcastTx:

```javascript
const broadcastInput: BroadcastInput = {
  chainId: chainId,
  rawTransaction: rawTransaction,
};
const broadcastResponse = await sdk.getAccountsSDK().broadcastTx(account, broadcastInput);
```

### Sending a Transaction with Encoded ABI Data

To send a transaction with encoded ABI data, you need to encode the data, prepare the transaction data, sign the transaction, and broadcast it to the blockchain.

#### Step 1: Encode the ABI Data

Encode the ABI data using ethers.js:

<pre class="language-typescript"><code class="lang-typescript"><strong>const abi = [{
</strong>	"constant": false,
	"inputs": [
		{
			"name": "_from",
			"type": "address"
		},
		{
			"name": "_to",
			"type": "address"
		},
		{
			"name": "_value",
			"type": "uint256"
		}
	],
	"name": "transferFrom",
	"outputs": [
		{
			"name": "success",
			"type": "bool"
		}
	],
	"payable": false,
	"stateMutability": "nonpayable",
	"type": "function"
}]
const functionName = "transferFrom"
const params = []


const encodedData = new ethers.utils.Interface(abi).encodeFunctionData(functionName, params);
</code></pre>

#### Step 2: Prepare the Transaction Data

Store data pertaining to the transaction in an InputBody object, including the encoded data:

```javascript
const transactionData: InputBody = {
  to: contractAddress,
  data: encodedData,
  chain_id: chainId,
  encoding: 'utf-8',
  value: "0",
  chain_id: chainId,
  encoding: 'utf-8',
};
```



#### Step 2: Sign the Transaction

Use the signTransaction function to sign the transaction and get the raw transaction string to broadcast the transaction:

```javascript
const signedTransactionData = await sdk.getAccountsSDK().signTransaction(account, transactionData);
const rawTransaction = signedTransactionData.data.data.transactions[0].raw_transaction;
```

#### Step 3: Broadcast the Signed Message to the Blockchain

Store the raw signed transaction string into a BroadcastInput object and use the input object to broadcast the transaction using broadcastTx:

```javascript
const broadcastInput: BroadcastInput = {
  chainId: chainId,
  rawTransaction: rawTransaction,
};
const broadcastResponse = await sdk.getAccountsSDK().broadcastTx(account, broadcastI
```

### Creating and Listing Accounts

You can create a new account using the createAccount function and list all accounts using the listAccounts function.

#### Creating an Account

To create a new account, use the createAccount function:

```javascript
const newAccount = await sdk.getAccountsSDK().createAccount({});
```

#### Listing Accounts

To list all accounts, use the listAccounts function:

```javascript
const accounts = await sdk.getAccountsSDK().listAccounts();
```

### Conclusion

You have successfully sent EVM transactions using MoonSDK, both with and without encoded ABI data, and created and listed accounts. You can now use MoonSDK to interact with various blockchain networks and services.
