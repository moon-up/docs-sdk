# Creation and Retrieval of Wallets

> Moon facilitates wallet initialization using the **`createAccount`** API. Moon APIs are again integrated into the SDKs of multiple chains such as Ethereum, Bitcoin, Solana, Ripple, Litecoin, and more. Various code examples are demonstrated below:
> 

```
//Ethereum
const newEthWallet = await moon.getAccountsSDK().createAccount({});

// Bitcoin
const newBitcoinWallet = await moon.getBitcoinSDK().createAccount({});

// Solana
const newSolanaWallet = await moon.getSolanaSDK().createAccount({});

// Ripple
const newRippleWallet = await moon.getRippleSDK().createAccount({});

// Litecoin
const newLitecoinWallet = await moon.getLitecoinSDK().createAccount({});
```

> In addition to wallet creation, Moon offers APIs for retrieving a wallet address (**`getAccount`**) and listing existing accounts (**`listAccounts`**). Various code examples are demonstrated below:
> 

```
// Ethereum
const listEthAccounts = await moon.getAccountsSDK().listAccounts({});
const getEthAccounts = await moon.getAccountsSDK().getAccount({});

// Bitcoin
const listBitcoinAccounts = await moon.getBitcoinAccountsSDK().listAccounts({});
const getBitcoinAccounts = await moon.getBitcoinAccountsSDK().getAccount({});

// Solana
const listSolanaAccounts = await moon.getSolanaSDK().listAccounts({});
const getSolanaAccounts = await moon.getSolanaSDK().getAccount({});

// Litecoin
const listLitecoinAccounts = await moon.getLitecoinSDK().listAccounts({});
const getLitecoinAccounts = await moon.getLitecoinSDK().getAccount({});

// Ripple
const listRippleAccounts = await moon.getRippleSDK().listAccounts({});
const getRippleAccounts = await moon.getRippleSDK().getAccount({});
```