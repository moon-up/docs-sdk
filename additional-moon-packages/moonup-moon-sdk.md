# @moonup/moon-sdk

## @moonup/moon-sdk Package Documentation

## **About Moon SDK:**

The `@moonup/moon-sdk` package is a comprehensive SDK that provides easy access to various blockchain functionalities. It supports multiple chains such as Ethereum, Solana, Bitcoin, Cosmos, EOS, Litecoin, Ripple, Tron, Bitcoincash, and Dogecoin. The SDK includes functionalities for managing accounts, interacting with DeFi protocols like Aave, Uniswap, and Yearn, and working with NFTs (ERC-20, ERC-721, and ERC-1155).

## **Installing Moon SDK:**

To utilize the Moon SDK package, first install it to the desired directory of the project:

#### To install Moon SDK:

{% tabs %}
{% tab title="npm" %}
```bash
npm install @moonup/moon-sdk
```
{% endtab %}

{% tab title="yarn" %}
```bash
yarn add @moonup/moon-sdk
```
{% endtab %}

{% tab title="pnpm" %}
```bash
pnpm add @moonup/moon-sdk
```
{% endtab %}
{% endtabs %}

### Usage

Here's a basic example of how to use the SDK:

```javascript
import { MoonSDK } from '@moonup/moon-sdk';

const moonSDK = new MoonSDK({ apiKey: 'your-api-key' });

// List accounts
const accounts = await moonSDK.listAccounts();
console.log(accounts);

// Create a new account
const newAccount = await moonSDK.createAccount();
console.log(newAccount);

// Sign a transaction
const signedTx = await moonSDK.SignTransaction(wallet, transaction);
console.log(signedTx);

// Broadcast a transaction
const txHash = await moonSDK.SendTransaction(wallet, signedTx, chain_id);
console.log(txHash);
```

### Events

The `MoonSDK` class emits various events that you can listen to in order to handle specific actions or errors. Here's an example of how to listen to events:

```javascript
import { MoonSDK } from '@moonup/moon-sdk';

const moonSDK = new MoonSDK();

moonSDK.on('accountCreated', (account) => {
  console.log(`Account created: ${account}`);
});

moonSDK.on('transactionSigned', (signedTransaction) => {
  console.log(`Transaction signed: ${signedTransaction}`);
});

moonSDK.on('messageSigned', (signedMessage) => {
  console.log(`Message signed: ${signedMessage}`);
});

moonSDK.on('typedDataSigned', (signedTypedData) => {
  console.log(`Typed data signed: ${signedTypedData}`);
});

moonSDK.on('transactionSent', (transactionHash) => {
  console.log(`Transaction sent: ${transactionHash}`);
});

moonSDK.on('chainsFetched', (chains) => {
  console.log(`Chains fetched: ${JSON.stringify(chains)}`);
});

moonSDK.on('chainFetched', (chain) => {
  console.log(`Chain fetched: ${JSON.stringify(chain)}`);
});

moonSDK.on('error', (error) => {
  console.error(`An error occurred: ${error.message}`);
});
```

The available events are:

* `accountCreated`: Emitted when a new account is created.
* `transactionSigned`: Emitted when a transaction is signed.
* `messageSigned`: Emitted when a message is signed.
* `typedDataSigned`: Emitted when typed data is signed.
* `transactionSent`: Emitted when a transaction is sent.
* `chainsFetched`: Emitted when the list of supported chains is fetched.
* `chainFetched`: Emitted when a specific chain is fetched.
* `error`: Emitted when an error occurs.

### API Reference

#### `MoonSDK` Class

**Constructor**

* `new MoonSDK(config?: MoonSDKConfig)`
  * `config` (optional): Configuration object for the SDK.
    * `apiKey` (string): Your API key for authentication.
    * `authInstance` (SupabaseClient): An existing Supabase client instance for authentication.
    * `httpParams` (ApiConfig): Configuration for the HTTP client.
    * `httpInstance` (HttpClient): An existing HttpClient instance.

**Methods**

* `connect(accessToken?: string, refreshToken?: string)`: Establishes a connection to the Moon API.
  *   Example:

      ```javascript
      await moonSDK.connect('access-token', 'refresh-token');
      ```
* `disconnect()`: Disconnects from the Moon API.
  *   Example:

      ```javascript
      await moonSDK.disconnect();
      ```
* `getMoonAuth()`: Returns the Supabase client instance for authentication.
  *   Example:

      ```javascript
      const authClient = moonSDK.getMoonAuth();
      ```
* `getUserSession()`: Returns the current user session.
  *   Example:

      ```javascript
      const session = await moonSDK.getUserSession();
      ```
* `getSolanaSDK()`: Returns the Solana SDK instance.
  *   Example:

      ```javascript
      const solanaSDK = moonSDK.getSolanaSDK();
      ```
* `getBitcoinSDK()`: Returns the Bitcoin SDK instance.
  *   Example:

      ```javascript
      const bitcoinSDK = moonSDK.getBitcoinSDK();
      ```
* `getCosmosSDK()`: Returns the Cosmos SDK instance.
  *   Example:

      ```javascript
      const cosmosSDK = moonSDK.getCosmosSDK();
      ```
* `getEosSDK()`: Returns the EOS SDK instance.
  *   Example:

      ```javascript
      const eosSDK = moonSDK.getEosSDK();
      ```
* `getLitecoinSDK()`: Returns the Litecoin SDK instance.
  *   Example:

      ```javascript
      const litecoinSDK = moonSDK.getLitecoinSDK();
      ```
* `getRippleSDK()`: Returns the Ripple SDK instance.
  *   Example:

      ```javascript
      const rippleSDK = moonSDK.getRippleSDK();
      ```
* `getTronSDK()`: Returns the Tron SDK instance.
  *   Example:

      ```javascript
      const tronSDK = moonSDK.getTronSDK();
      ```
* `getBitcoincashSDK()`: Returns the Bitcoincash SDK instance.
  *   Example:

      ```javascript
      const bitcoincashSDK = moonSDK.getBitcoincashSDK();
      ```
* `getDogecoinSDK()`: Returns the Dogecoin SDK instance.
  *   Example:

      ```javascript
      const dogecoinSDK = moonSDK.getDogecoinSDK();
      ```
* `getAccountsSDK()`: Returns the Accounts SDK instance.
  *   Example:

      ```javascript
      const accountsSDK = moonSDK.getAccountsSDK();
      ```
* `getAaveSDK()`: Returns the Aave SDK instance.
  *   Example:

      ```javascript
      const aaveSDK = moonSDK.getAaveSDK();
      ```
* `getConveyorfinanceSDK()`: Returns the Conveyorfinance SDK instance.
  *   Example:

      ```javascript
      const conveyorfinanceSDK = moonSDK.getConveyorfinanceSDK();
      ```
* `getENSSDK()`: Returns the ENS SDK instance.
  *   Example:

      ```javascript
      const ensSDK = moonSDK.getENSSDK();
      ```
* `getErc20SDK()`: Returns the ERC-20 SDK instance.
  *   Example:

      ```javascript
      const erc20SDK = moonSDK.getErc20SDK();
      ```
* `getErc1155SDK()`: Returns the ERC-1155 SDK instance.
  *   Example:

      ```javascript
      const erc1155SDK = moonSDK.getErc1155SDK();
      ```
* `getErc721SDK()`: Returns the ERC-721 SDK instance.
  *   Example:

      ```javascript
      const erc721SDK = moonSDK.getErc721SDK();
      ```
* `getOneinchSDK()`: Returns the 1inch SDK instance.
  *   Example:

      ```javascript
      const oneinchSDK = moonSDK.getOneinchSDK();
      ```
* `getUniswapSDK()`: Returns the Uniswap SDK instance.
  *   Example:

      ```javascript
      const uniswapSDK = moonSDK.getUniswapSDK();
      ```
* `getYearnSDK()`: Returns the Yearn SDK instance.
  *   Example:

      ```javascript
      const yearnSDK = moonSDK.getYearnSDK();
      ```
* `listAccounts()`: Lists all available accounts.
  *   Example:

      ```javascript
      const accounts = await moonSDK.listAccounts();
      ```
* `createAccount()`: Creates a new account.
  *   Example:

      ```javascript
      const newAccount = await moonSDK.createAccount();
      ```
* `SignTransaction(wallet: string, transaction: InputBody)`: Signs a transaction.
  *   Example:

      ```javascript
      const signedTx = await moonSDK.SignTransaction(wallet, transaction);
      ```
* `SignMessage(wallet: string, message: BytesLike)`: Signs a message.
  *   Example:

      ```javascript
      const signedMessage = await moonSDK.SignMessage(wallet, message);
      ```
* `SignTypedData(wallet: string, domain: TypedDataDomain, types: Record<string, Array<TypedDataField>>, value: Record<string, string>)`: Signs typed data.
  *   Example:

      ```javascript
      const signedTypedData = await moonSDK.SignTypedData(wallet, domain, types, value);
      ```
* `SendTransaction(wallet: string, rawTransaction: string, chain_id: string)`: Broadcasts a transaction.
  *   Example:

      ```javascript
      const txHash = await moonSDK.SendTransaction(wallet, signedTx, chain_id);
      ```
* `getChains()`: Retrieves a list of supported chains.
  *   Example:

      ```javascript
      const chains = await moonSDK.getChains();
      ```
* `getChainById(id: string)`: Retrieves a chain by its ID.
  *   Example:

      ```javascript
      const chain = await moonSDK.getChainById('chain-id');
      ```



###
