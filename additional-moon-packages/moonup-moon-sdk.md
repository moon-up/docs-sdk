# @moonup/moon-sdk

### Moon SDK



### Installation

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
import { MoonSDK } from '@moonup/moon-sdk'
const sdk = new MoonSDK()
```



### Functions

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
