# @moonup/moon-sdk

### Moon SDK

## **About Moon SDK:**

**Moon API provides low level API endpoint wrappers with expected input and output data types**

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

```typescript
import { MoonSDK } from '@moonup/moon-sdk';

// Create an instance of the MoonSDK class
const moonSDK = new MoonSDK();

// Connect to the Moon API
await moonSDK.connect();

// Disconnect from the Moon API
await moonSDK.disconnect();

// Get the Moon API client
const moonAuth = moonSDK.getMoonAuth();

// Get the user session
const userSession = await moonSDK.getUserSession();

// Get the Solana SDK
const solanaSDK = moonSDK.getSolanaSDK();

// Get the Bitcoin SDK
const bitcoinSDK = moonSDK.getBitcoinSDK();

// Get the Cosmos SDK
const cosmosSDK = moonSDK.getCosmosSDK();

// Get the Eos SDK
const eosSDK = moonSDK.getEosSDK();

// Get the Litecoin SDK
const litecoinSDK = moonSDK.getLitecoinSDK();

// Get the Ripple SDK
const rippleSDK = moonSDK.getRippleSDK();

// Get the Tron SDK
const tronSDK = moonSDK.getTronSDK();

// Get the Bitcoincash SDK
const bitcoincashSDK = moonSDK.getBitcoincashSDK();

// Get the Dogecoin SDK
const dogecoinSDK = moonSDK.getDogecoinSDK();

// Get the Accounts SDK
const accountsSDK = moonSDK.getAccountsSDK();

// Get the Aave SDK
const aaveSDK = moonSDK.getAaveSDK();

// Get the Conveyorfinance SDK
const conveyorfinanceSDK = moonSDK.getConveyorfinanceSDK();

// Get the ENS SDK
const ensSDK = moonSDK.getENSSDK();

// Get the Erc20 SDK
const erc20SDK = moonSDK.getErc20SDK();

// Get the Erc1155 SDK
const erc1155SDK = moonSDK.getErc1155SDK();

// Get the Erc721 SDK
const erc721SDK = moonSDK.getErc721SDK();

// Get the Oneinch SDK
const oneinchSDK = moonSDK.getOneinchSDK();

// Get the Uniswap SDK
const uniswapSDK = moonSDK.getUniswapSDK();

// Get the Yearn SDK
const yearnSDK = moonSDK.getYearnSDK();

// List all accounts
const accounts = await moonSDK.listAccounts();

// Create a new account
const newAccount = await moonSDK.createAccount();

// Sign a transaction
const signedTransaction = await moonSDK.SignTransaction('wallet', { /* transaction data */ });

// Sign a message
const signedMessage = await moonSDK.SignMessage('wallet', 'message');

// Sign typed data
const signedTypedData = await moonSDK.SignTypedData('wallet', { /* domain data */ }, { /* types data */ }, { /* value data */ });

// Send a transaction
const transactionResponse = await moonSDK.SendTransaction('wallet', 'rawTransaction', 'chain_id');

// Get all chains
const chains = await moonSDK.getChains();

// Get a chain by its ID
const chain = await moonSDK.getChainById('id');
```

### MoonSDK class

#### `connect()`

Returns a `Promise<void>`. Establishes a connection.

#### `disconnect()`

Returns a `Promise<void>`. Closes the established connection.

#### `getUserSession()`

Returns a `Promise` that resolves to the user's session data or an error.

#### `getSolanaSDK()`

Returns an instance of the Solana SDK.

#### `getBitcoinSDK()`

Returns an instance of the Bitcoin SDK.

#### `getCosmosSDK()`

Returns an instance of the Cosmos SDK.

#### `getEosSDK()`

Returns an instance of the EOS SDK.

#### `getLitecoinSDK()`

Returns an instance of the Litecoin SDK.

#### `getRippleSDK()`

Returns an instance of the Ripple SDK.

#### `getTronSDK()`

Returns an instance of the Tron SDK.

#### `getBitcoincashSDK()`

Returns an instance of the Bitcoin Cash SDK.

#### `getDogecoinSDK()`

Returns an instance of the Dogecoin SDK.

#### `getAccountsSDK()`

Returns an instance of the Accounts SDK.

#### `getAaveSDK()`

Returns an instance of the Aave SDK.

#### `getConveyorfinanceSDK()`

Returns an instance of the Conveyor Finance SDK.

#### `getENSSDK()`

Returns an instance of the ENS SDK.

#### `getErc20SDK()`

Returns an instance of the ERC20 SDK.

#### `getErc1155SDK()`

Returns an instance of the ERC1155 SDK.

#### `getErc721SDK()`

Returns an instance of the ERC721 SDK.

#### `getOneinchSDK()`

Returns an instance of the 1inch SDK.

#### `getUniswapSDK()`

Returns an instance of the Uniswap SDK.

#### `getYearnSDK()`

Returns an instance of the Yearn Finance SDK.

#### `listAccounts()`

Returns a `Promise<string[]>` that resolves to a list of accounts.

#### `createAccount()`

Returns a `Promise<string>` that resolves to the created account.

#### `moonTransactionResponseToTransactions(tx: Transaction)`

Converts a moon transaction response to transactions data.

#### `SignTransaction(wallet: string, transaction: InputBody)`

Signs a transaction and returns a `Promise<string>` that resolves to the signed transaction.

#### `SignMessage(wallet: string, message: BytesLike)`

Signs a message and returns a `Promise<string>` that resolves to the signed message.

#### `SignTypedData(wallet: string, domain: TypedDataDomain, types: Record<string, Array<TypedDataField>>, value: Record<string, string>)`

Signs typed data and returns a `Promise<string>` that resolves to the signed data.

#### `SendTransaction(wallet: string, rawTransaction: string, chain_id: string)`

Sends a transaction and returns a `Promise<string>` that resolves to the transaction hash.

#### `getChains()`

Returns a `Promise<Chains[]>` that resolves to a list of supported chains.

#### `getChainById(id: string)`

Returns a `Promise<Chains>` that resolves to the chain with the specified ID
