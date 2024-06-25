# @moonup/moon-sdk

## @moonup/moon-sdk Package Documentation

## **About Moon SDK:**

The @moonup/moon-sdk package is a comprehensive SDK that provides easy access to various blockchain functionalities. It supports multiple chains such as Ethereum, Solana, Bitcoin, Cosmos, EOS, Litecoin, Ripple, Tron, Bitcoincash, and Dogecoin. The SDK includes functionalities for managing accounts, interacting with DeFi protocols like Aave, Uniswap, and Yearn, and working with NFTs (ERC-20, ERC-721, and ERC-1155).

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

The MoonSDK class emits various events that you can listen to in order to handle specific actions or errors. Here's an example of how to listen to events:

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

#### MoonSDK Class

**Constructor**

```javascript
new MoonSDK(config?: MoonSDKConfig)
```

* `config` (optional): Configuration object for the SDK.
  * `apiKey` (string): Your API key for authentication.
  * `authInstance` (SupabaseClient): An existing Supabase client instance for authentication.
  * `httpParams` (ApiConfig): Configuration for the HTTP client.
  * `httpInstance` (HttpClient): An existing HttpClient instance.
  * clientId (string): Moon oauth2 client id param

**Methods**

*   `connect(accessToken?: string, refreshToken?: string)`: Establishes a connection to the Moon API.

    ```javascript
    await moonSDK.connect('access-token', 'refresh-token');
    ```
*   `disconnect()`: Disconnects from the Moon API.

    ```javascript
    await moonSDK.disconnect();
    ```
*   `getMoonAuth()`: Returns the Supabase client instance for authentication.

    ```javascript
    const authClient = moonSDK.getMoonAuth();
    ```
*   `getUserSession()`: Returns the current user session.

    ```javascript
    const session = await moonSDK.getUserSession();
    ```
*   `getSolanaSDK()`: Returns the Solana SDK instance.

    ```javascript
    const solanaSDK = moonSDK.getSolanaSDK();
    ```
*   `getBitcoinSDK()`: Returns the Bitcoin SDK instance.

    ```javascript
    const bitcoinSDK = moonSDK.getBitcoinSDK();
    ```
*   `getCosmosSDK()`: Returns the Cosmos SDK instance.

    ```javascript
    const cosmosSDK = moonSDK.getCosmosSDK();
    ```
*   `getEosSDK()`: Returns the EOS SDK instance.

    ```javascript
    const eosSDK = moonSDK.getEosSDK();
    ```
*   `getLitecoinSDK()`: Returns the Litecoin SDK instance.

    ```javascript
    const litecoinSDK = moonSDK.getLitecoinSDK();
    ```
*   `getRippleSDK()`: Returns the Ripple SDK instance.

    ```javascript
    const rippleSDK = moonSDK.getRippleSDK();
    ```
*   `getTronSDK()`: Returns the Tron SDK instance.

    ```javascript
    const tronSDK = moonSDK.getTronSDK();
    ```
*   `getBitcoincashSDK()`: Returns the Bitcoincash SDK instance.

    ```javascript
    const bitcoincashSDK = moonSDK.getBitcoincashSDK();
    ```
*   `getDogecoinSDK()`: Returns the Dogecoin SDK instance.

    ```javascript
    const dogecoinSDK = moonSDK.getDogecoinSDK();
    ```
*   `getAccountsSDK()`: Returns the Accounts SDK instance.

    ```javascript
    const accountsSDK = moonSDK.getAccountsSDK();
    ```
*   `getAaveSDK()`: Returns the Aave SDK instance.

    ```javascript
    const aaveSDK = moonSDK.getAaveSDK();
    ```
*   `getConveyorfinanceSDK()`: Returns the Conveyorfinance SDK instance.

    ```javascript
    const conveyorfinanceSDK = moonSDK.getConveyorfinanceSDK();
    ```
*   `getENSSDK()`: Returns the ENS SDK instance.

    ```javascript
    const ensSDK = moonSDK.getENSSDK();
    ```
*   `getErc20SDK()`: Returns the ERC-20 SDK instance.

    ```javascript
    const erc20SDK = moonSDK.getErc20SDK();
    ```
*   `getErc1155SDK()`: Returns the ERC-1155 SDK instance.

    ```javascript
    const erc1155SDK = moonSDK.getErc1155SDK();
    ```
*   `getErc721SDK()`: Returns the ERC-721 SDK instance.

    ```javascript
    const erc721SDK = moonSDK.getErc721SDK();
    ```
*   `getOneinchSDK()`: Returns the 1inch SDK instance.

    ```javascript
    const oneinchSDK = moonSDK.getOneinchSDK();
    ```
*   `getUniswapSDK()`: Returns the Uniswap SDK instance.

    ```javascript
    const uniswapSDK = moonSDK.getUniswapSDK();
    ```
*   `getYearnSDK()`: Returns the Yearn SDK instance.

    ```javascript
    const yearnSDK = moonSDK.getYearnSDK();
    ```
*   `listAccounts()`: Lists all available accounts.

    ```javascript
    const accounts = await moonSDK.listAccounts();
    ```
*   `createAccount()`: Creates a new account.

    ```javascript
    const newAccount = await moonSDK.createAccount();
    ```
*   `SignTransaction(wallet: string, transaction: InputBody)`: Signs a transaction.

    ```javascript
    const signedTx = await moonSDK.SignTransaction(wallet, transaction);
    ```
*   `SignMessage(wallet: string, message: BytesLike)`: Signs a message.

    ```javascript
    const signedMessage = await moonSDK.SignMessage(wallet, message);
    ```
*   `SignTypedData(wallet: string, domain: TypedDataDomain, types: Record<string, Array<TypedDataField>>, value: Record<string, string>)`: Signs typed data.

    ```javascript
    const signedTypedData = await moonSDK.SignTypedData(wallet, domain, types, value);
    ```
*   `SendTransaction(wallet: string, rawTransaction: string, chain_id: string)`: Broadcasts a transaction.

    ```javascript
    const txHash = await moonSDK.SendTransaction(wallet, signedTx, chain_id);
    ```
*   `getChains()`: Retrieves a list of supported chains.

    ```javascript
    const chains = await moonSDK.getChains();
    ```
*   `getChainById(id: string)`: Retrieves a chain by its ID.

    ```javascript
    const chain = await moonSDK.getChainById('chain-id');
    ```



### Authentication Methods

The Moon SDK supports various authentication methods to provide secure access to the blockchain functionalities. The following authentication methods are available:

### Usage

Here's a basic example of how to use the SDK:

```javascript
import { MoonSDK } from '@moonup/moon-sdk';

const moonSDK = new MoonSDK({ clientId: 'your-client-id' });

// Discord OAuth
await moonSDK.performDiscordOAuth();
// After obtaining the authorization code, exchange it for an access token and refresh token
const discordToken = await moonSDK.performDiscordOauthCodeExchange(code);

// GitHub OAuth
await moonSDK.performGithubOAuth();
// After obtaining the authorization code, exchange it for an access token and refresh token
const githubToken = await moonSDK.performGithubOauthCodeExchange(code);

// Google OAuth
await moonSDK.performGoogleOAuth();
// After obtaining the authorization code, exchange it for an access token and refresh token
const googleToken = await moonSDK.performGoogleOauthCodeExchange(code);

// Twitter OAuth
await moonSDK.performTwitterOauth();
// After obtaining the authorization code, exchange it for an access token and refresh token
const twitterToken = await moonSDK.performTwitterOauthCodeExchange(code);

// Magic Link
await moonSDK.sendMagicLink(email, redirectTo);

// Email and Password
await moonSDK.signUp(email, password);
await moonSDK.signInWithPassword(email, password);

// Phone and Password
await moonSDK.signInWithPhone(phone, password);

// Passkey
const passkeyOptions = await moonSDK.handlePassKeyLogin(email);
// Use the passkeyOptions to authenticate the user using their passkey
const passkeyResponse = await moonSDK.handlePasskeyLoginVerify(email, credential);

// SIWE (Sign-In with Ethereum)
const nonce = await moonSDK.getSIWENonce(address);
// Sign the SIWE message using the Ethereum wallet
const siweResponse = await moonSDK.verifySIWESignature(address, signedMessage, nonce, message);

// Embedded Account
const session = await moonSDK.embeddedAccount(email, uuid, domain);
```

#### Discord OAuth

To authenticate using Discord OAuth, follow these steps:

1.  Initiate the Discord OAuth flow:

    ```javascript
    await moonSDK.performDiscordOAuth();
    ```
2. After the user is redirected to the Discord authorization page, obtain the authorization code from the URL.
3.  Exchange the authorization code for an access token and refresh token:

    ```javascript
    const token = await moonSDK.performDiscordOauthCodeExchange(code);
    ```

#### GitHub OAuth

To authenticate using GitHub OAuth, follow these steps:

1.  Initiate the GitHub OAuth flow:

    ```javascript
    await moonSDK.performGithubOAuth();
    ```
2. After the user is redirected to the GitHub authorization page, obtain the authorization code from the URL.
3.  Exchange the authorization code for an access token and refresh token:

    ```javascript
    const token = await moonSDK.performGithubOauthCodeExchange(code);
    ```

#### Google OAuth

To authenticate using Google OAuth, follow these steps:

1.  Initiate the Google OAuth flow:

    ```javascript
    await moonSDK.performGoogleOAuth();
    ```
2. After the user is redirected to the Google authorization page, obtain the authorization code from the URL.
3.  Exchange the authorization code for an access token and refresh token:

    ```javascript
    const token = await moonSDK.performGoogleOauthCodeExchange(code);
    ```

#### Twitter OAuth

To authenticate using Twitter OAuth, follow these steps:

1.  Initiate the Twitter OAuth flow:

    ```javascript
    await moonSDK.performTwitterOauth();
    ```
2. After the user is redirected to the Twitter authorization page, obtain the authorization code from the URL.
3.  Exchange the authorization code for an access token and refresh token:

    ```javascript
    const token = await moonSDK.performTwitterOauthCodeExchange(code);
    ```

#### Magic Link

To authenticate using a magic link, follow these steps:

1.  Send a magic link to the user's email address:

    ```javascript
    await moonSDK.sendMagicLink(email, redirectTo);
    ```
2. The user will receive an email with a magic link. After clicking the link, they will be redirected to the specified `redirectTo` URL.

#### Email and Password

To authenticate using email and password, follow these steps:

1.  Create a new user account:

    ```javascript
    await moonSDK.signUp(email, password);
    ```
2.  Sign in with the created account:

    ```javascript
    await moonSDK.signInWithPassword(email, password);
    ```

#### Phone and Password

To authenticate using phone and password, follow these steps:

1.  Sign in with the phone number and password:

    ```javascript
    await moonSDK.signInWithPhone(phone, password);
    ```

#### Passkey

To authenticate using a passkey, follow these steps:

1.  Initiate the passkey login flow:

    ```javascript
    const options = await moonSDK.handlePassKeyLogin(email);
    ```
2. Use the `options` to authenticate the user using their passkey.
3.  Verify the passkey login credentials:

    ```javascript
    const response = await moonSDK.handlePasskeyLoginVerify(email, credential);
    ```

#### SIWE (Sign-In with Ethereum)

To authenticate using SIWE, follow these steps:

1.  Retrieve a nonce for the Ethereum address:

    ```javascript
    const nonce = await moonSDK.getSIWENonce(address);
    ```
2. Sign the SIWE message using the Ethereum wallet.
3.  Verify the SIWE signature:

    ```javascript
    const response = await moonSDK.verifySIWESignature(address, signedMessage, nonce, message);
    ```

#### Embedded Account

To create an embedded account, follow these steps:

1.  Create an embedded account for the specified email address, UUID, and domain:

    ```javascript
    const session = await moonSDK.embeddedAccount(email, uuid, domain);
    ```
